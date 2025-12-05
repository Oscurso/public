# ECE - Emergent Curiosity Engine

## Wat is ECE?

ECE is een cognitieve module die **autonome nieuwsgierigheid** simuleert. Het systeem detecteert gaps in zijn eigen kennis en genereert vragen om die gaps te vullen.

**Kernprincipe:** Het systeem weet wat het niet weet. In plaats van te hallucineren of te gokken, stelt het vragen.

---

## Hoe werkt het?

1. **Kennis laden** - Concepten en relaties worden geladen uit een seed file
2. **Gap detectie** - Het systeem analyseert welke concepten onduidelijk zijn (lage clarity score)
3. **Vraag generatie** - Voor elke gap wordt een vraag gegenereerd
4. **Pursuit** - Het systeem probeert vragen te beantwoorden met bestaande kennis
5. **Blocked/Satisfied** - Vragen worden gemarkeerd als beantwoord of geblokkeerd (externe input nodig)

---

## Huidige Staat

| Component | Status |
|-----------|--------|
| Core engine | ✅ Werkend |
| CLI interface | ✅ Werkend |
| Demo modes | ✅ 5 modes (basic, extended, interactive, detailed, quick) |
| Seed files | ✅ 5 sectoren (biology, business, software, finance, medical) |
| State persistence | ✅ JSON export |

---

## Use Cases Per Sector

### 1. Biology / Research

**Gaps gedetecteerd:** 28

**Typische vragen:**
- "What exactly is consciousness?"
- "What exactly is life?"
- "How does intelligence relate to consciousness?"

**Toepassing:**
- Research planning - identificeer welke onderzoeksvragen nog open staan
- Literature review - detecteer gaps in bestaande kennis
- Hypothesis generatie - systeem stelt vragen die onderzoekers kunnen beantwoorden

**Voorbeeld gebruiker:** Universiteiten, R&D afdelingen, research labs

---

### 2. Business / Startup

**Gaps gedetecteerd:** 33

**Typische vragen:**
- "What exactly is competitive moat?"
- "What exactly is innovation?"
- "What exactly is product-market fit?"
- "What exactly is traction?"

**Toepassing:**
- Due diligence - identificeer onduidelijkheden in business plannen
- Strategy sessies - maak impliciete aannames expliciet
- Investor pitches - bereid je voor op vragen over vage concepten
- Onboarding - nieuwe medewerkers kunnen vragen stellen zonder "dom" te lijken

**Voorbeeld gebruiker:** Startups, VCs, accelerators, consultants

---

### 3. Software / Tech

**Gaps gedetecteerd:** 35

**Typische vragen:**
- "What exactly is architecture?"
- "What exactly is security?"
- "What exactly is scalability?"
- "What exactly is technical debt?"

**Toepassing:**
- Code reviews - identificeer onduidelijke design beslissingen
- Documentatie - vind gaps in technische docs
- Onboarding - nieuwe devs kunnen vragen stellen over onduidelijke systemen
- Architecture reviews - maak impliciete aannames expliciet

**Voorbeeld gebruiker:** Development teams, tech leads, software architects

---

### 4. Finance / Banking

**Gaps gedetecteerd:** 41

**Typische vragen:**
- "What exactly is fraud?"
- "What exactly is creditworthiness?"
- "What exactly is systemic risk?"
- "What exactly is anti-money laundering?"

**Toepassing:**
- Compliance - identificeer onduidelijkheden in regelgeving
- Risk assessment - vind gaps in risk modellen
- Audit voorbereiding - anticipeer op vragen van auditors
- Training - nieuwe medewerkers leren wat ze niet weten

**Waarom meer gaps dan andere sectoren:**
Finance heeft inherent meer onzekerheid - abstracte concepten, complexe regelgeving, verborgen risico's. Het systeem detecteert dit automatisch.

**Voorbeeld gebruiker:** Banken, verzekeraars, compliance afdelingen, auditors

---

### 5. Medical / Healthcare

**Gaps gedetecteerd:** 45 (hoogste)

**Typische vragen:**
- "What exactly is prognosis?"
- "What exactly is informed consent?"
- "What exactly is efficacy?"
- "What exactly is contraindication?"

**Toepassing:**
- Clinical decision support - systeem vraagt om verduidelijking voordat het adviseert
- Medical training - studenten leren wat ze nog niet weten
- Patient communicatie - identificeer wat patiënten niet begrijpen
- Research protocols - vind gaps in study designs

**Waarom meeste gaps:**
Medische beslissingen combineren biologie, statistiek, regelgeving en ethiek. Het systeem detecteert de inherente complexiteit en weigert te gokken waar levens op het spel staan.

**Voorbeeld gebruiker:** Ziekenhuizen, farmaceutische bedrijven, medical device companies, CROs

---

## Demo Modes

| Mode | Beschrijving | Beste voor |
|------|--------------|------------|
| `basic` | Standaard flow, 1 cycle | Snelle introductie |
| `extended` | 3 cycles, toont vraag accumulatie | Diepere demonstratie |
| `interactive` | Gebruiker typt zelf antwoorden | Hands-on ervaring |
| `detailed` | Extra stats: scores, coverage, gap analysis | Technisch publiek |
| `quick` | Geen pauzes, runt automatisch door | Video opnames, CI/CD |

**Gebruik:**
```bash
ece demo --seed data/seed_finance.json --mode detailed
```

---

## Waarom Dit Anders Is Dan LLMs

| Aspect | LLM (GPT, Claude) | ECE |
|--------|-------------------|-----|
| Bij onzekerheid | Hallucineert een antwoord | Stelt een vraag |
| Kennisstate | Onbekend (black box) | Volledig inzichtelijk |
| Gaps | Verborgen | Expliciet gedetecteerd |
| Traceability | Beperkt | 100% - elke vraag heeft ID, score, type |
| Gedrag | Probabilistisch | Deterministisch |

---

## Technische Specificaties

- **Taal:** Rust
- **Binary:** `ece` (standalone executable)
- **State format:** JSON
- **Input format:** JSON seed files
- **Output:** CLI + JSON state file

---

## Volgende Stappen

1. **ICS integratie** - Koppeling met andere cognitieve modules
2. **API endpoint** - REST API voor integratie in andere systemen
3. **Web UI** - Visuele interface voor niet-technische gebruikers
4. **Custom seed generator** - Tool om eigen sector seeds te maken

---

## Contact

Oscurso Research Labs
https://oscurso.com
