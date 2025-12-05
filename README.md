# Oscurso Labs - Cognitive Architecture

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active%20Development-green" alt="Status">
  <img src="https://img.shields.io/badge/Language-Rust-orange" alt="Rust">
  <img src="https://img.shields.io/badge/License-Proprietary-blue" alt="License">
  <img src="https://img.shields.io/badge/GDPR-Compliant-success" alt="GDPR">
</p>

## 🧠 What Is This?

**Oscurso** is building a **deterministic cognitive architecture** - an alternative approach to AI that prioritizes transparency, explainability, and European data sovereignty.

Unlike black-box neural networks where you can't see *why* a decision was made, Oscurso's cognitive modules are **fully traceable**. Every reasoning step, every decision, every insight can be audited and explained.

> **"Not just an answer, but the reasoning that led there."**

---

## 🏗️ Architecture Overview

The Oscurso cognitive stack consists of **5 interconnected modules**, each answering a fundamental cognitive question:

```
┌─────────────────────────────────────────────────────────────────┐
│                    OSCURSO COGNITIVE LOOP                        │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   ┌─────────┐     ┌─────────┐     ┌─────────┐                   │
│   │   ECE   │ ──▶ │  RSIR   │ ──▶ │   CDE   │                   │
│   │Curiosity│     │Reasoning│     │Critique │                   │
│   └─────────┘     └─────────┘     └─────────┘                   │
│        │                               │                         │
│        │         ┌─────────┐           │                         │
│        └───────▶ │   WIM   │ ◀─────────┘                         │
│                  │ Intent  │                                     │
│                  └─────────┘                                     │
│                       │                                          │
│                       ▼                                          │
│                  ┌─────────┐                                     │
│                  │   ODI   │                                     │
│                  │ Dreams  │                                     │
│                  └─────────┘                                     │
│                       │                                          │
│                       └──────────────▶ [feeds back to ECE]       │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

---

## 📦 The Modules

| Module | Full Name | Question | Purpose |
|--------|-----------|----------|---------|
| **[ECE](./ECE)** | Emergent Curiosity Engine | *"What do I want to know?"* | Generates questions, identifies knowledge gaps, drives exploration |
| **[RSIR](./RSIR)** | Recursive Self-Interrogating Reasoning | *"What can I conclude?"* | Multi-layer reasoning with self-critique and confidence tracking |
| **[CDE](./CDE)** | Critical Decision Engine | *"Does this make sense?"* | Validates conclusions, identifies logical flaws, stress-tests reasoning |
| **[WIM](./WIM)** | Working Intent Memory | *"What am I doing?"* | Manages active tasks, handles interruptions, preserves context |
| **[ODI](./ODI)** | Overnight Dream Integration | *"What have I learned?"* | Consolidates knowledge, finds patterns, generates insights |

---

## 🎯 Key Features

### Deterministic & Traceable
Every decision has a clear audit trail. No hidden layers, no unexplainable outputs.

### European Data Sovereignty
Built for GDPR compliance. Your data stays transparent and under your control.

### Real Working Systems
Not vaporware. Each module has working demos with real outputs you can run.

### Industry-Proven
Demos across Healthcare, Finance, Legal, Research, and Cybersecurity sectors.

---

## 📊 Real System Output

### ECE - Emergent Curiosity Engine
```
[CURIOSITY] Generated 12 questions about patient treatment patterns
[DEPTH 1] "What causes readmission within 30 days?"
[DEPTH 2] "Are there medication interaction patterns we're missing?"
[DEPTH 3] "Could lifestyle factors predict treatment resistance?"
```

### RSIR - Recursive Self-Interrogating Reasoning
```
[LAYER 1] Initial analysis: 3 hypotheses formed
[LAYER 2] Self-critique: Eliminated hypothesis B (insufficient evidence)
[LAYER 3] Confidence: 0.87 for remaining conclusions
[OUTPUT] Recommendation with full reasoning chain
```

### CDE - Critical Decision Engine
```
[ANALYSIS] Decision: Approve $2.4M infrastructure investment
[DEVIL'S ADVOCATE] Found 3 potential failure modes
[STRESS TEST] Scenario analysis: 2/5 edge cases need mitigation
[VERDICT] CONDITIONAL APPROVE with risk mitigations
```

### WIM - Working Intent Memory
```
[INTENT] Primary: Complete quarterly report (60% progress)
[INTERRUPT] Urgent: Production incident (urgency: 0.92)
[PRESERVE] Saved: cursor position, open files, mental model
[RESTORE] Context restored in 47 seconds (vs 15min manual)
```

### ODI - Overnight Dream Integration
```
[COLLECTING] Gathered 30 memories
[PATTERN FINDING] Found 30 patterns
[ASSOCIATING] Created 38 associations
[INSIGHT] Cross-domain connection discovered (novelty: 0.90)
```

> **Interested in a live demo?** [Contact us](mailto:contact@oscurso.com) to schedule a demonstration with your own data.

---

## 🏭 Industry Applications

| Industry | Use Case | Module Focus |
|----------|----------|--------------|
| **Healthcare** | Treatment pattern discovery, drug interactions | ECE, ODI |
| **Finance** | Risk analysis, market correlation discovery | CDE, ODI |
| **Legal** | Case precedent analysis, strategy optimization | RSIR, CDE |
| **Research** | Hypothesis generation, methodology patterns | ECE, RSIR |
| **Cybersecurity** | Threat intelligence consolidation | ODI, CDE |

---

## 📚 Documentation

### English
- [ECE Documentation](./ECE/docs/ece-documentation-EN.md)
- [RSIR Documentation](./RSIR/docs/rsir-documentation-EN.md)
- [CDE Documentation](./CDE/docs/cde-documentation-EN.md)
- [WIM Documentation](./WIM/docs/) (5 industry-specific docs)
- [ODI Documentation](./ODI/docs/odi-documentation-EN.md)

### Nederlands
- [ECE Documentatie](./ECE/docs/ece-documentation-NL.md)
- [RSIR Documentatie](./RSIR/docs/rsir-documentation-NL.md)
- [CDE Documentatie](./CDE/docs/cde-documentation-NL.md)
- [WIM Documentatie](./WIM/docs/) (5 industrie-specifieke docs)
- [ODI Documentatie](./ODI/docs/odi-documentation-NL.md)

---

## 🔧 Technical Stack

- **Language:** Rust (performance, safety, predictability)
- **State Management:** JSON-based knowledge graphs
- **Integration:** ICS (Integrated Cognitive System) orchestration
- **Deployment:** Standalone binaries, cross-platform
- **API:** REST endpoints (planned)

---

## 🌍 Why Oscurso?

### The Problem with Current AI

| Neural Networks | Oscurso Approach |
|-----------------|------------------|
| Black box decisions | Fully traceable reasoning |
| Can't explain "why" | Complete audit trail |
| Data sovereignty concerns | GDPR-compliant by design |
| Requires massive compute | Efficient, targeted processing |
| Hallucinations common | Deterministic, verifiable |

### European AI Sovereignty

We believe Europe needs its own approach to AI - one that aligns with European values of privacy, transparency, and individual rights. Oscurso is built from the ground up with these principles.

---

## 📈 Roadmap

- [x] ECE - Emergent Curiosity Engine
- [x] RSIR - Recursive Self-Interrogating Reasoning  
- [x] CDE - Critical Decision Engine
- [x] WIM - Working Intent Memory
- [x] ODI - Overnight Dream Integration
- [ ] ICS - Full cognitive loop integration
- [ ] API endpoints for enterprise integration
- [ ] Multi-agent collaboration
- [ ] Continuous learning without forgetting

---

## 🤝 Contact

**Oscurso Labs**

- 🌐 Website: [oscurso.com](https://oscurso.com)
- 📧 Email: [info@oscurso.com](mailto:info@oscurso.com)
- 🔗 LinkedIn: [Oscurso](https://linkedin.com/company/oscurso)

---

## 📜 License

Proprietary - All Rights Reserved

This repository contains public demonstrations and documentation. The underlying systems and algorithms are proprietary to Oscurso Labs.

---

<p align="center">
  <strong>Building Transparent AI for Europe</strong><br>
  <em>Not just intelligence. Understandable intelligence.</em>
</p>
