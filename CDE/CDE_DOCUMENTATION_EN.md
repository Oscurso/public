# CDE - Cognitive Dissonance Engine

## What is CDE?

CDE is a cognitive module that performs **critical analysis** on knowledge systems. It detects logical conflicts, challenges weak assumptions, generates edge cases, and calibrates confidence levels.

**Core principle:** The system finds where your knowledge contradicts itself or stands on shaky foundations. Instead of ignoring errors, it makes them explicit.

---

## How Does It Work?

1. **Load knowledge** - Concepts and relations are loaded from a knowledge file
2. **Contradiction detection** - The system finds where A→B and A→¬B exist simultaneously
3. **Assumption challenging** - Claims with little supporting evidence are questioned
4. **Edge case generation** - Boundary situations are tested ("What if X is extreme?")
5. **Confidence calibration** - Is the stated certainty supported by evidence?
6. **Dialectics** - Thesis → Antithesis → Synthesis for conflicts

---

## Current State

| Component | Status |
|-----------|--------|
| Core engine | ✅ Working |
| CLI interface | ✅ Working |
| Critique types | ✅ 4 types (contradiction, weak assumption, edge case, miscalibration) |
| Dialectics | ✅ Thesis-Antithesis-Synthesis |
| Knowledge files | ✅ 5 domains (medical, financial, software, legal, logic) |
| Workspace management | ✅ Save/load/reload |
| Output formats | ✅ Text, JSON, Markdown |

---

## Use Cases Per Sector

### 1. Medical / Healthcare

**Demo results:**
- Contradictions: 1
- Weak Assumptions: 7
- Edge Cases: 170

**Detected contradiction:**
> "Viral infections can lead to secondary bacterial infections" vs "Antibiotics are ineffective against viral infections"

This is exactly the tension clinicians face daily: you don't give antibiotics for viruses, but must stay alert for bacterial superinfection.

**Typical critiques:**
- "Antibiotic choice in pregnancy requires careful consideration of fetal safety - what's the evidence?"
- "Can Sepsis ever exist without Hospitalization?" (edge case: terminal patient at home)
- "Immunocompromised patients need empirical antibiotics - always? Or are there alternatives?"

**Applications:**
- Protocol review - find conflicts in treatment guidelines
- Clinical decision support - make implicit assumptions explicit
- Medical education - teach clinicians to think critically about protocols
- Compliance - audit trail for medical decisions

**Example users:** Hospitals, pharmaceutical companies, healthcare institutions, CROs

---

### 2. Financial / Banking

**Demo results:**
- Contradictions: 1
- Weak Assumptions: 8
- Edge Cases: 194

**Typical critiques:**
- "Near-retirement investors need bond allocation for stability - what supports this?"
- "Risk-averse investors should emphasize bonds - is this proven?"
- "Dollar-cost averaging reduces timing risk - assumption or fact?"
- "Can Bear Market Conditions exist without Cash Equivalents?" (edge case)

**Applications:**
- Advice validation - check if investment advice is consistent with client profile
- Compliance - automatic check for contradictory recommendations
- Risk assessment - find hidden assumptions in risk models
- Audit preparation - anticipate questions from regulators

**Why valuable:**
Finance has inherently many assumptions that are rarely made explicit. "Diversification reduces risk" sounds logical, but CDE asks: "Always? In all market conditions? For all investors?"

**Example users:** Banks, asset managers, compliance departments, regulators

---

### 3. Software / Architecture

**Demo results:**
- Contradictions: 0
- Weak Assumptions: 1
- Edge Cases: 92

**Typical critiques:**
- "Large organization implicitly requires independent deployment - is this proven?"
- "Can Microservices exist without Observability Tooling?" (edge case)
- "Is Monolithic Architecture alone sufficient to enable Rapid Initial Development?"
- "Saga pattern confidence 85% - evidence suggests 34%"

**Applications:**
- Architecture Decision Records (ADR) review - are our choices consistent?
- Technical debt identification - which assumptions were never validated?
- Onboarding - new architects understand why decisions were made
- Migration planning - which edge cases are we missing in our microservices transition?

**Why 0 contradictions:**
The improved knowledge file eliminated synonyms. This shows that CDE **rewards clean data** - no false positives.

**Example users:** Scale-ups, enterprise IT, software consultancies, CTOs

---

### 4. Legal / Contracts

**Demo results:**
- Contradictions: 0
- Weak Assumptions: 10
- Edge Cases: 150

**Typical critiques:**
- "Offer requires acceptance to form contract - is this assumed?"
- "Contracts for necessities valid even with minors - where does this come from?"
- "Oral contracts valid but harder to prove - is this verified?"
- "Fraud makes contract voidable - confidence 95%, evidence suggests 42%"

**Applications:**
- Contract review - find clauses that contradict each other
- Due diligence - identify hidden assumptions in agreements
- Legal education - teach lawyers to look critically at "obvious" principles
- Compliance - audit trail for contractual decisions

**Why many miscalibrations:**
Legal "truths" are often presented with high certainty, but CDE asks: "Is 95% confidence justified when there are jurisdiction-dependent exceptions?"

**Example users:** Law firms, legal tech, corporate legal, procurement

---

### 5. Logic / Argumentation

**Applications:**
- Report validation - find weak arguments in business cases
- Proposal review - check if conclusions follow from premises
- Debate preparation - anticipate counterarguments
- Critical thinking training - teach employees to recognize fallacies

**Example users:** Consultancies, research firms, universities, policy makers

---

## Critique Types

| Type | What it finds | Severity |
|------|---------------|----------|
| **Contradiction** | A→B and A→¬B simultaneously | 0.60-0.75 |
| **WeakAssumption** | Claims without supporting evidence | 0.50-0.65 |
| **EdgeCaseFailure** | Boundary situations that break rules | 0.35-0.40 |
| **ConfidenceMiscalibration** | Certainty ≠ evidence | 0.45-0.55 |

---

## Dialectical Reasoning

CDE applies dialectical reasoning to contradictions:

```
THESIS:      "Viral infections can lead to secondary bacterial infections"
             Confidence: 60%
             
ANTITHESIS:  "Antibiotics are ineffective against viral infections"
             Confidence: 95%
             
SYNTHESIS:   "Antibiotics should not be given for viral infections,
              but clinicians should monitor for secondary bacterial
              infection and start antibiotics if bacterial superinfection
              is suspected based on clinical deterioration or biomarkers."
```

This is not a compromise - it's a **higher truth** that integrates both perspectives.

---

## Why This Is Different From LLMs

| Aspect | LLM (GPT, Claude) | CDE |
|--------|-------------------|-----|
| With conflicts | Picks one side or gives vague answer | Makes conflict explicit |
| Assumptions | Hidden in training data | Explicitly detected |
| Edge cases | Often missed | Systematically generated |
| Confidence | "I think that..." | Calibrated against evidence |
| Traceability | Limited | 100% - every critique has ID, severity, resolution |
| Behavior | Probabilistic | Deterministic |

---

## Technical Specifications

- **Language:** Rust
- **Binary:** `cde` (standalone executable, cross-platform)
- **State format:** JSON
- **Input format:** JSON knowledge files
- **Output:** CLI + JSON + Markdown reports
- **Workspace:** Persistent state management

---

## CLI Commands

```bash
# Analysis
cde analyze -i knowledge.json

# View critiques
cde list --limit 10
cde list --critique-type contradiction
cde show CRT-ABC123

# Critique lifecycle
cde resolve CRT-ABC123 "Added missing evidence"
cde accept CRT-ABC123 "Known limitation, documented"
cde dismiss CRT-ABC123 "False positive due to synonym"

# Dialectics
cde dialectic list
cde dialectic show DIA-XYZ789

# Workspace
cde workspace save --name project-v1
cde workspace load project-v1
cde workspace list

# Reports
cde report -f markdown -o analysis.md
cde stats
```

---

## Next Steps

1. **ICS integration** - Connection with ECE, RSIR and other cognitive modules
2. **API endpoint** - REST API for integration into other systems
3. **Web UI** - Visual interface for non-technical users
4. **Custom knowledge generator** - Tool to create domain-specific knowledge files
5. **Evidence linking** - Connect claims to sources (papers, guidelines, regulations)

---

## Contact

Oscurso Labs
https://oscurso.com
