```
╔═══════════════════════════════════════════════════════╗
║  🏥 Medical Diagnosis Scenario                        ║
║  Patient with ambiguous respiratory symptoms          ║
╚═══════════════════════════════════════════════════════╝

This demo shows how RSIR handles:
  • Conflicting diagnostic possibilities
  • Self-interrogation when confidence is low
  • Backward propagation when new evidence arrives
  • Full explainability of reasoning chains

   [Press Enter to continue...]

╔═══════════════════════════════════════════════════════╗
║  PHASE 1: Initial Symptoms                            ║
╚═══════════════════════════════════════════════════════╝

Patient presents with symptoms that could indicate multiple conditions

📋 Adding observations:

   1. Patient has high fever
   2. Patient has persistent cough
   3. Patient has fatigue
   4. Patient has muscle aches

🧬 Loading reasoning rules (4 rules)...

   ✓ Rules loaded successfully

🧠 Analyzing...

📊 Processing Statistics:
   └─ Nodes created: 8
   └─ Cycles completed: 3
   └─ Overall confidence: 1.00

🎯 Conclusions:

   1. Possible diagnosis: Influenza (Flu) [Node 5]
      └─ Starting from Patient has muscle aches, we concluded that Possible ...
   2. Possible diagnosis: COVID-19 [Node 6]
      └─ Starting from Patient has fatigue, we concluded that Possible diagn...
   3. Multiple diagnoses possible - need more tests [Node 8]
   4. Possible diagnosis: Pneumonia [Node 7]
      └─ Starting from Patient has persistent cough, we concluded that Possi...

   [Press Enter to continue...]

╔═══════════════════════════════════════════════════════╗
║  PHASE 2: New Test Results                            ║
╚═══════════════════════════════════════════════════════╝

Lab tests provide definitive evidence

📋 Adding observations:

   1. COVID-19 test result is positive
   2. Influenza test result is negative

🧬 Loading reasoning rules (2 rules)...

   ✓ Rules loaded successfully

🧠 Analyzing...

📊 Processing Statistics:
   └─ Nodes created: 12
   └─ Cycles completed: 5
   └─ Overall confidence: 1.00

🎯 Conclusions:

   1. Possible diagnosis: Influenza (Flu) [Node 5]
      └─ Starting from Patient has muscle aches, we concluded that Possible ...
   2. Possible diagnosis: COVID-19 [Node 6]
      └─ Starting from Patient has fatigue, we concluded that Possible diagn...
   3. CONFIRMED DIAGNOSIS: COVID-19 [Node 11]
      └─ Starting from COVID-19 test result is positive, we concluded that C...
   4. Possible diagnosis: Pneumonia [Node 7]
      └─ Starting from Patient has persistent cough, we concluded that Possi...
   5. Multiple diagnoses possible - need more tests [Node 8]
   6. Influenza diagnosis excluded [Node 12]
      └─ Starting from Influenza test result is negative, we concluded that ...

💡 Insight: New evidence has significantly increased confidence.
   Previous uncertain conclusions have been updated.

   [Press Enter to continue...]

╔═══════════════════════════════════════════════════════╗
║  Final Explanation & Traceability                    ║
╚═══════════════════════════════════════════════════════╝

✅ Final Diagnosis Found:

   CONFIRMED DIAGNOSIS: COVID-19

📝 Reasoning Trace:

   Starting from COVID-19 test result is positive, we concluded that CONFIRMED DIAGNOSIS: COVID-19

   Reasoning chain (2 steps):
      1. COVID-19 test result is positive (confidence: 1.00)
      2. CONFIRMED DIAGNOSIS: COVID-19 (confidence: 1.00)

   This complete trace provides:
   ✓ Full accountability - every step is recorded
   ✓ Auditability - can review reasoning later
   ✓ Explainability - patient/doctor understands why
   ✓ Debuggability - if diagnosis was wrong, can find why

   [Press Enter to continue...]

╔═══════════════════════════════════════════════════════╗
║  'Why Not' Explanation                               ║
╚═══════════════════════════════════════════════════════╝

❓ Question: 'Why was it not Influenza?'

   No reasoning path was found that would lead to 'confirmed diagnosis is Influenza'

   Key reasons:
      • The premise 'confirmed diagnosis is Influenza' was never obser...


╔═══════════════════════════════════════════════════════╗
║  Demo Summary                                         ║
╚═══════════════════════════════════════════════════════╝

🎓 What This Demo Showed:

   1️⃣  CONFLICT DETECTION
      • Multiple diagnoses from ambiguous symptoms
      • System recognized uncertainty

   2️⃣  SELF-INTERROGATION
      • System questioned its own confidence
      • Identified need for more information

   3️⃣  BACKWARD PROPAGATION
      • New evidence invalidated old conclusions
      • All dependent reasoning updated automatically

   4️⃣  FULL EXPLAINABILITY
      • Complete reasoning trace available
      • Can answer 'why' and 'why not'

   5️⃣  UNCERTAINTY QUANTIFICATION
      • Confidence scores at every step
      • Transparent about what's known vs unknown

📊 Final Statistics:
   └─ Total observations: 6
   └─ Total rules loaded: 6
   └─ Total reasoning nodes: 12
   └─ Phases completed: 2
   └─ Final confidence: 1.00

╔═══════════════════════════════════════════════════════╗
║  🎉 Demo Complete!                                    ║
╚═══════════════════════════════════════════════════════╝

💡 TIP: You can modify the scenario by editing:
   data/scenarios/medical_diagnosis.json
   No Rust code changes needed!
```