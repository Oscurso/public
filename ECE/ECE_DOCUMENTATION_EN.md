# ECE - Emergent Curiosity Engine

## What is ECE?

ECE is a cognitive module that simulates **autonomous curiosity**. The system detects gaps in its own knowledge and generates questions to fill those gaps.

**Core principle:** The system knows what it doesn't know. Instead of hallucinating or guessing, it asks questions.

---

## How Does It Work?

1. **Load knowledge** - Concepts and relations are loaded from a seed file
2. **Gap detection** - The system analyzes which concepts are unclear (low clarity score)
3. **Question generation** - For each gap, a question is generated
4. **Pursuit** - The system attempts to answer questions using existing knowledge
5. **Blocked/Satisfied** - Questions are marked as answered or blocked (external input needed)

---

## Current State

| Component | Status |
|-----------|--------|
| Core engine | ✅ Working |
| CLI interface | ✅ Working |
| Demo modes | ✅ 5 modes (basic, extended, interactive, detailed, quick) |
| Seed files | ✅ 5 sectors (biology, business, software, finance, medical) |
| State persistence | ✅ JSON export |

---

## Use Cases By Sector

### 1. Biology / Research

**Gaps detected:** 28

**Typical questions:**
- "What exactly is consciousness?"
- "What exactly is life?"
- "How does intelligence relate to consciousness?"

**Application:**
- Research planning - identify which research questions remain open
- Literature review - detect gaps in existing knowledge
- Hypothesis generation - system poses questions researchers can answer

**Example users:** Universities, R&D departments, research labs

---

### 2. Business / Startup

**Gaps detected:** 33

**Typical questions:**
- "What exactly is competitive moat?"
- "What exactly is innovation?"
- "What exactly is product-market fit?"
- "What exactly is traction?"

**Application:**
- Due diligence - identify ambiguities in business plans
- Strategy sessions - make implicit assumptions explicit
- Investor pitches - prepare for questions about vague concepts
- Onboarding - new employees can ask questions without feeling "stupid"

**Example users:** Startups, VCs, accelerators, consultants

---

### 3. Software / Tech

**Gaps detected:** 35

**Typical questions:**
- "What exactly is architecture?"
- "What exactly is security?"
- "What exactly is scalability?"
- "What exactly is technical debt?"

**Application:**
- Code reviews - identify unclear design decisions
- Documentation - find gaps in technical docs
- Onboarding - new devs can ask questions about unclear systems
- Architecture reviews - make implicit assumptions explicit

**Example users:** Development teams, tech leads, software architects

---

### 4. Finance / Banking

**Gaps detected:** 41

**Typical questions:**
- "What exactly is fraud?"
- "What exactly is creditworthiness?"
- "What exactly is systemic risk?"
- "What exactly is anti-money laundering?"

**Application:**
- Compliance - identify ambiguities in regulations
- Risk assessment - find gaps in risk models
- Audit preparation - anticipate auditor questions
- Training - new employees learn what they don't know

**Why more gaps than other sectors:**
Finance has inherently more uncertainty - abstract concepts, complex regulations, hidden risks. The system detects this automatically.

**Example users:** Banks, insurers, compliance departments, auditors

---

### 5. Medical / Healthcare

**Gaps detected:** 45 (highest)

**Typical questions:**
- "What exactly is prognosis?"
- "What exactly is informed consent?"
- "What exactly is efficacy?"
- "What exactly is contraindication?"

**Application:**
- Clinical decision support - system asks for clarification before advising
- Medical training - students learn what they don't yet know
- Patient communication - identify what patients don't understand
- Research protocols - find gaps in study designs

**Why most gaps:**
Medical decisions combine biology, statistics, regulation, and ethics. The system detects the inherent complexity and refuses to guess where lives are at stake.

**Example users:** Hospitals, pharmaceutical companies, medical device companies, CROs

---

## Demo Modes

| Mode | Description | Best for |
|------|-------------|----------|
| `basic` | Standard flow, 1 cycle | Quick introduction |
| `extended` | 3 cycles, shows question accumulation | Deeper demonstration |
| `interactive` | User types their own answers | Hands-on experience |
| `detailed` | Extra stats: scores, coverage, gap analysis | Technical audience |
| `quick` | No pauses, runs automatically | Video recordings, CI/CD |

**Usage:**
```bash
ece demo --seed data/seed_finance.json --mode detailed
```

---

## Why This Is Different From LLMs

| Aspect | LLM (GPT, Claude) | ECE |
|--------|-------------------|-----|
| When uncertain | Hallucinates an answer | Asks a question |
| Knowledge state | Unknown (black box) | Fully transparent |
| Gaps | Hidden | Explicitly detected |
| Traceability | Limited | 100% - every question has ID, score, type |
| Behavior | Probabilistic | Deterministic |

---

## Technical Specifications

- **Language:** Rust
- **Binary:** `ece` (standalone executable)
- **State format:** JSON
- **Input format:** JSON seed files
- **Output:** CLI + JSON state file

---

## Next Steps

1. **ICS integration** - Connection with other cognitive modules
2. **API endpoint** - REST API for integration into other systems
3. **Web UI** - Visual interface for non-technical users
4. **Custom seed generator** - Tool to create custom sector seeds

---

## Contact

Oscurso Research Labs
https://oscurso.com
