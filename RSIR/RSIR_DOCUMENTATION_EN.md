# RSIR - Recursive Self-Interrogating Reasoning

## What is RSIR?

RSIR is a cognitive module that performs **knowledge-driven reasoning**. The system automatically builds a semantic network from knowledge and reasons toward conclusions on its own - without hardcoded if-else rules.

**Core principle:** Give the system only knowledge. RSIR derives the relationships and conclusions itself.

---

## How Does It Work?

1. **Load knowledge** - Text or JSON files with domain knowledge (definitions, symptoms, facts)
2. **Build network** - RSIR automatically builds relationships between concepts
3. **General rules** - No scenario-specific rules, but general reasoning patterns
4. **Automatic reasoning** - RSIR reasons toward conclusions on its own
5. **Full traceability** - Every conclusion can be traced back to its source

---

## The Difference: Hardcoded vs Knowledge-Driven

| Hardcoded (wrong) | Knowledge-Driven (correct) |
|-------------------|---------------------------|
| `if fever && cough → covid` | RSIR derives that fever+cough matches covid |
| Rules in JSON | Only knowledge in text files |
| Not extensible | Add knowledge, RSIR reasons automatically |
| Script that prints output | System that truly reasons |

---

## Current State

| Component | Status |
|-----------|--------|
| Core engine | ✅ Working |
| Definition Explorer | ✅ 2707 definitions, semantic network |
| Medical Demo | ✅ Knowledge-driven diagnosis |
| Detective Demo | ✅ Knowledge-driven investigation |
| Debugging Demo | ✅ Knowledge-driven bug analysis |
| State persistence | ✅ JSON/Text export |

---

## Use Cases By Sector

### 1. Healthcare / Medical Diagnosis

**What it does:**
- Loads medical knowledge (symptoms, diseases, tests)
- Receives patient observations
- Automatically reasons toward possible diagnoses
- Confirms/excludes based on test results

**Example output:**
```
🤔 Possible Diagnoses (before testing):
   • Possible diagnosis: influenza
   • Possible diagnosis: covid19

✅ Confirmed Diagnosis:
   • CONFIRMED: covid19
     └─ Based on positive covid_rapid_test

❌ Excluded:
   • EXCLUDED: influenza
```

**Why this is valuable:**
- System doesn't hallucinate - it reasons based on knowledge
- Full traceability for audits
- Doctors can add knowledge without changing code
- Transparent: you see exactly why a diagnosis was made

**Application:**
- Clinical decision support
- Medical training (students see the reasoning)
- Triage systems
- Second opinion tools

---

### 2. Legal / Criminal Investigation

**What it does:**
- Loads investigation knowledge (evidence types, suspect attributes)
- Receives case observations (testimonies, evidence, alibis)
- Reasons toward suspects with automatic revision when new evidence arrives

**Example output:**
```
🔍 Initial Conclusions:
   • Alibi provided - lower suspicion

🚨 NEW EVIDENCE: Alibi proven false

   • CRITICAL: False alibi - consciousness of guilt
   • STRONG EVIDENCE: Suspect lied to investigators
   • COMPELLING: Physical evidence places suspect at scene

🎯 Primary Suspect: Sarah (business partner)
   Strength of case: VERY STRONG
```

**Why this is valuable:**
- Automatic revision when evidence changes (backward propagation)
- No tunnel vision - system considers all possibilities
- Complete audit trail for legal review
- Can answer "why" and "why not" questions

**Application:**
- Investigation support for law enforcement
- Compliance investigations
- Fraud detection
- Due diligence

---

### 3. Software / Bug Analysis

**What it does:**
- Loads debugging knowledge (symptoms, causes, fix patterns)
- Receives bug observations (logs, errors, filesystem checks)
- Automatically traces from symptom to root cause
- Suggests fixes based on identified cause

**Example output:**
```
📖 The Story:
   1. Users reported broken images (http_404 errors)
   2. Database check: file metadata exists ✓
   3. Filesystem check: files NOT in expected location ✗
   4. Git history: recent code change modified upload path
   5. Root cause: Code changed but nginx config unchanged
   6. Fix: Update nginx config to match new upload path

🔧 Suggested Fixes:
   • sync_code_and_config
   • update_file_paths
```

**Why this is valuable:**
- Systematic debugging instead of random guessing
- Identifies which assumptions were wrong
- Finds related bugs before they cause problems
- New developers can debug complex systems

**Application:**
- Developer tooling
- Incident response
- Post-mortem analysis
- Onboarding new developers

---

## Technical Operation

### Knowledge Format

RSIR accepts simple text files:

```
# Medical Knowledge
SYMPTOM fever
  severity: mild_to_severe
  category: general

DISEASE covid19
  has_symptom: fever
  has_symptom: cough
  has_symptom: fatigue
  transmission: airborne

TEST covid_rapid_test
  detects: covid19
  accuracy: 0.95
```

### General Reasoning Rules

RSIR uses general rules that work for all cases:

```
1. Symptom Matching Rule
   IF patient has symptom S AND disease D has symptom S
   → Disease D is a possible diagnosis

2. Test Confirmation Rule
   IF test for disease D is positive
   → Confirm diagnosis D

3. Test Exclusion Rule
   IF test for disease D is negative
   → Exclude diagnosis D
```

These rules are **not scenario-specific** - they work for every disease, every test.

---

## Why This Is Different From LLMs

| Aspect | LLM (GPT, Claude) | RSIR |
|--------|-------------------|------|
| When uncertain | Hallucinates an answer | Shows what it doesn't know |
| Reasoning | Hidden in weights | Fully traceable |
| Updating knowledge | Requires retraining | Edit text file |
| New cases | May fail unexpectedly | Reasons consistently |
| Audit trail | Limited | 100% - every step documented |
| Backward propagation | Not possible | Automatic when new evidence arrives |

---

## The Power of Backward Propagation

When new evidence arrives that invalidates old conclusions:

1. **LLM:** Doesn't know earlier conclusion was wrong
2. **RSIR:** Automatically revises all dependent conclusions

Example Detective Case:
```
Initial: Sarah has alibi → low suspicion
New evidence: Alibi is false
RSIR: Automatically revises → high suspicion + "consciousness of guilt"
```

This is crucial for domains where information changes (investigations, diagnoses, debugging).

---

## Technical Specifications

- **Language:** Rust
- **Binaries:** `definition_demo`, `medical_knowledge_demo`, `detective_knowledge_demo`, `debugging_knowledge_demo`
- **Knowledge format:** Text files (custom format)
- **State format:** JSON
- **Semantic network:** 295,955 edges (with 2707 definitions)

---

## Next Steps

1. **API endpoint** - REST API for integration
2. **Web UI** - Visual interface for knowledge management
3. **Custom knowledge generator** - Tool to create custom domain knowledge
4. **ICS integration** - Connection with other cognitive modules

---

## Contact

Oscurso Labs
https://oscurso.com
