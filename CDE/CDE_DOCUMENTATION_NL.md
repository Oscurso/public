# CDE - Cognitive Dissonance Engine

## Wat is CDE?

CDE is een cognitieve module die **kritische analyse** uitvoert op kennissystemen. Het detecteert logische conflicten, bevraagt zwakke aannames, genereert edge cases en kalibreert confidence levels.

**Kernprincipe:** Het systeem vindt waar je kennis zichzelf tegenspreekt of op wankele fundamenten staat. In plaats van fouten te negeren, maakt het ze expliciet.

---

## Hoe werkt het?

1. **Kennis laden** - Concepten en relaties worden geladen uit een knowledge file
2. **Contradiction detectie** - Het systeem vindt waar A→B en A→¬B tegelijk bestaan
3. **Assumption challenging** - Claims met weinig onderbouwing worden bevraagd
4. **Edge case generatie** - Grenssituaties worden getest ("Wat als X extreem is?")
5. **Confidence calibratie** - Wordt de zekerheid ondersteund door bewijs?
6. **Dialectiek** - Thesis → Antithesis → Synthesis voor conflicten

---

## Huidige Staat

| Component | Status |
|-----------|--------|
| Core engine | ✅ Werkend |
| CLI interface | ✅ Werkend |
| Critique types | ✅ 4 types (contradiction, weak assumption, edge case, miscalibration) |
| Dialectics | ✅ Thesis-Antithesis-Synthesis |
| Knowledge files | ✅ 5 domeinen (medical, financial, software, legal, logic) |
| Workspace management | ✅ Save/load/reload |
| Output formats | ✅ Text, JSON, Markdown |

---

## Use Cases Per Sector

### 1. Medical / Healthcare

**Resultaten uit demo:**
- Contradictions: 1
- Weak Assumptions: 7
- Edge Cases: 170

**Gevonden contradiction:**
> "Viral infections can lead to secondary bacterial infections" vs "Antibiotics are ineffective against viral infections"

Dit is precies de spanning die artsen dagelijks ervaren: je geeft geen antibiotica voor virussen, maar moet alert zijn op bacteriële superinfectie.

**Typische critiques:**
- "Antibiotic choice in pregnancy requires careful consideration of fetal safety - wat is het bewijs?"
- "Can Sepsis ever exist without Hospitalization?" (edge case: terminale patiënt thuis)
- "Immunocompromised patients need empirical antibiotics - altijd? Of zijn er alternatieven?"

**Toepassing:**
- Protocol review - vind conflicten in behandelrichtlijnen
- Clinical decision support - maak impliciete aannames expliciet
- Medical education - leer artsen kritisch denken over protocollen
- Compliance - audit trail voor medische beslissingen

**Voorbeeld gebruiker:** Ziekenhuizen, farmaceutische bedrijven, zorginstellingen, CROs

---

### 2. Financial / Banking

**Resultaten uit demo:**
- Contradictions: 1
- Weak Assumptions: 8
- Edge Cases: 194

**Typische critiques:**
- "Near-retirement investors need bond allocation for stability - wat ondersteunt dit?"
- "Risk-averse investors should emphasize bonds - is dit bewezen?"
- "Dollar-cost averaging reduces timing risk - aanname of feit?"
- "Can Bear Market Conditions exist without Cash Equivalents?" (edge case)

**Toepassing:**
- Advies validatie - check of beleggingsadvies consistent is met klantprofiel
- Compliance - automatische controle op tegenstrijdige aanbevelingen
- Risk assessment - vind verborgen aannames in risk modellen
- Audit voorbereiding - anticipeer op vragen van toezichthouders

**Waarom waardevol:**
Finance heeft inherent veel aannames die zelden expliciet gemaakt worden. "Diversificatie reduceert risico" klinkt logisch, maar CDE vraagt: "Altijd? In alle marktcondities? Voor alle beleggers?"

**Voorbeeld gebruiker:** Banken, vermogensbeheerders, compliance afdelingen, AFM/DNB

---

### 3. Software / Architecture

**Resultaten uit demo:**
- Contradictions: 0
- Weak Assumptions: 1
- Edge Cases: 92

**Typische critiques:**
- "Large organization implicitly requires independent deployment - is dit bewezen?"
- "Can Microservices exist without Observability Tooling?" (edge case)
- "Is Monolithic Architecture alone sufficient to enable Rapid Initial Development?"
- "Saga pattern confidence 85% - bewijs suggereert 34%"

**Toepassing:**
- Architecture Decision Records (ADR) review - zijn onze keuzes consistent?
- Technical debt identificatie - welke aannames zijn nooit gevalideerd?
- Onboarding - nieuwe architecten begrijpen waarom beslissingen genomen zijn
- Migratie planning - welke edge cases missen we in onze microservices transitie?

**Waarom 0 contradictions:**
De verbeterde knowledge file heeft synoniemen geëlimineerd. Dit toont dat CDE **schone data beloont** - geen valse positieven.

**Voorbeeld gebruiker:** Scale-ups, enterprise IT, software consultancies, CTOs

---

### 4. Legal / Contracts

**Resultaten uit demo:**
- Contradictions: 0
- Weak Assumptions: 10
- Edge Cases: 150

**Typische critiques:**
- "Offer requires acceptance to form contract - wordt dit aangenomen?"
- "Contracts for necessities valid even with minors - waar komt dit vandaan?"
- "Oral contracts valid but harder to prove - is dit geverifieerd?"
- "Fraud makes contract voidable - confidence 95%, bewijs suggereert 42%"

**Toepassing:**
- Contract review - vind clausules die elkaar tegenspreken
- Due diligence - identificeer verborgen aannames in overeenkomsten
- Legal education - leer juristen kritisch naar "vanzelfsprekende" principes te kijken
- Compliance - audit trail voor contractuele beslissingen

**Waarom veel miscalibrations:**
Juridische "waarheden" worden vaak met hoge zekerheid gepresenteerd, maar CDE vraagt: "Is 95% confidence gerechtvaardigd als er jurisdictie-afhankelijke uitzonderingen zijn?"

**Voorbeeld gebruiker:** Advocatenkantoren, legal tech, corporate legal, procurement

---

### 5. Logic / Argumentation

**Toepassing:**
- Rapport validatie - vind zwakke argumenten in business cases
- Proposal review - check of conclusies volgen uit premissen
- Debat voorbereiding - anticipeer op tegenargumenten
- Critical thinking training - leer medewerkers drogredenen herkennen

**Voorbeeld gebruiker:** Consultancies, research firms, universiteiten, policy makers

---

## Critique Types

| Type | Wat het vindt | Severity |
|------|---------------|----------|
| **Contradiction** | A→B en A→¬B tegelijk | 0.60-0.75 |
| **WeakAssumption** | Claims zonder onderbouwing | 0.50-0.65 |
| **EdgeCaseFailure** | Grenssituaties die regels breken | 0.35-0.40 |
| **ConfidenceMiscalibration** | Zekerheid ≠ bewijs | 0.45-0.55 |

---

## Dialectical Reasoning

CDE past dialectisch redeneren toe op contradictions:

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

Dit is geen compromis - het is een **hogere waarheid** die beide perspectieven integreert.

---

## Waarom Dit Anders Is Dan LLMs

| Aspect | LLM (GPT, Claude) | CDE |
|--------|-------------------|-----|
| Bij conflicten | Kiest één kant of geeft vaag antwoord | Maakt conflict expliciet |
| Aannames | Verborgen in training data | Expliciet gedetecteerd |
| Edge cases | Vaak gemist | Systematisch gegenereerd |
| Confidence | "Ik denk dat..." | Gekalibreerd tegen bewijs |
| Traceability | Beperkt | 100% - elke critique heeft ID, severity, resolution |
| Gedrag | Probabilistisch | Deterministisch |

---

## Technische Specificaties

- **Taal:** Rust
- **Binary:** `cde` (standalone executable, cross-platform)
- **State format:** JSON
- **Input format:** JSON knowledge files
- **Output:** CLI + JSON + Markdown reports
- **Workspace:** Persistent state management

---

## CLI Commands

```bash
# Analyse
cde analyze -i knowledge.json

# Critiques bekijken
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

## Volgende Stappen

1. **ICS integratie** - Koppeling met ECE, RSIR en andere cognitieve modules
2. **API endpoint** - REST API voor integratie in andere systemen
3. **Web UI** - Visuele interface voor niet-technische gebruikers
4. **Custom knowledge generator** - Tool om eigen domein knowledge files te maken
5. **Evidence linking** - Koppel claims aan bronnen (papers, guidelines, regulations)

---

## Contact

Oscurso Labs
https://oscurso.com
