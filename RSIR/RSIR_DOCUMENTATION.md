# RSIR - Recursive Self-Interrogating Reasoning

## Wat is RSIR?

RSIR is een cognitieve module die **kennisgedreven redenering** uitvoert. Het systeem bouwt automatisch een semantisch netwerk van kennis en redeneert zelf naar conclusies - zonder hardcoded if-else regels.

**Kernprincipe:** Geef het systeem alleen kennis. RSIR leidt zelf de relaties en conclusies af.

---

## Hoe werkt het?

1. **Kennis laden** - Text of JSON files met domeinkennis (definities, symptomen, feiten)
2. **Netwerk bouwen** - RSIR bouwt automatisch relaties tussen concepten
3. **Algemene regels** - Geen scenario-specifieke regels, maar algemene reasoning patterns
4. **Automatische reasoning** - RSIR redeneert zelf naar conclusies
5. **Volledige traceerbaarheid** - Elke conclusie is te traceren naar de bron

---

## Het Verschil: Hardcoded vs Knowledge-Driven

| Hardcoded (fout) | Knowledge-Driven (correct) |
|------------------|---------------------------|
| `if fever && cough → covid` | RSIR leidt zelf af dat fever+cough past bij covid |
| Rules in JSON | Alleen kennis in text files |
| Niet uitbreidbaar | Voeg kennis toe, RSIR redeneert automatisch |
| Script dat output print | Systeem dat echt redeneert |

---

## Huidige Staat

| Component | Status |
|-----------|--------|
| Core engine | ✅ Werkend |
| Definition Explorer | ✅ 2707 definities, semantisch netwerk |
| Medical Demo | ✅ Knowledge-driven diagnose |
| Detective Demo | ✅ Knowledge-driven onderzoek |
| Debugging Demo | ✅ Knowledge-driven bug analyse |
| State persistence | ✅ JSON/Text export |

---

## Use Cases Per Sector

### 1. Healthcare / Medical Diagnosis

**Wat het doet:**
- Laadt medische kennis (symptomen, ziektes, tests)
- Ontvangt patiënt observaties
- Redeneert automatisch naar mogelijke diagnoses
- Bevestigt/sluit uit op basis van testresultaten

**Voorbeeld output:**
```
🤔 Mogelijke Diagnoses (voor testen):
   • Possible diagnosis: influenza
   • Possible diagnosis: covid19

✅ Bevestigde Diagnose:
   • CONFIRMED: covid19
     └─ Gebaseerd op positieve covid_rapid_test

❌ Uitgesloten:
   • EXCLUDED: influenza
```

**Waarom dit waardevol is:**
- Systeem hallucineert niet - het redeneert op basis van kennis
- Volledige traceerbaarheid voor audits
- Artsen kunnen kennis toevoegen zonder code te wijzigen
- Transparant: je ziet precies waarom een diagnose is gesteld

**Toepassing:**
- Klinische beslissingsondersteuning
- Medische training (studenten zien de redenering)
- Triage systemen
- Second opinion tools

---

### 2. Legal / Criminal Investigation

**Wat het doet:**
- Laadt onderzoekskennis (bewijstypen, verdachte attributen)
- Ontvangt case observaties (getuigenissen, bewijs, alibi's)
- Redeneert naar verdachten met automatische herziening bij nieuw bewijs

**Voorbeeld output:**
```
🔍 Initiële Conclusies:
   • Alibi provided - lower suspicion

🚨 NIEUW BEWIJS: Alibi blijkt vals

   • CRITICAL: False alibi - consciousness of guilt
   • STRONG EVIDENCE: Suspect lied to investigators
   • COMPELLING: Physical evidence places suspect at scene

🎯 Primaire Verdachte: Sarah (business partner)
   Sterkte van zaak: ZEER STERK
```

**Waarom dit waardevol is:**
- Automatische herziening wanneer bewijs verandert (backward propagation)
- Geen tunnelvisie - systeem overweegt alle mogelijkheden
- Volledige audit trail voor juridische review
- Kan "waarom" en "waarom niet" vragen beantwoorden

**Toepassing:**
- Onderzoeksondersteuning voor politie/justitie
- Compliance onderzoeken
- Fraud detectie
- Due diligence

---

### 3. Software / Bug Analysis

**Wat het doet:**
- Laadt debugging kennis (symptomen, oorzaken, fix patterns)
- Ontvangt bug observaties (logs, errors, filesystem checks)
- Traceert automatisch van symptoom naar root cause
- Suggereert fixes gebaseerd op geïdentificeerde oorzaak

**Voorbeeld output:**
```
📖 Het Verhaal:
   1. Users rapporteerden broken images (http_404 errors)
   2. Database check: file metadata exists ✓
   3. Filesystem check: files NOT in expected location ✗
   4. Git history: recent code change modified upload path
   5. Root cause: Code changed maar nginx config niet
   6. Fix: Update nginx config naar nieuwe upload path

🔧 Suggested Fixes:
   • sync_code_and_config
   • update_file_paths
```

**Waarom dit waardevol is:**
- Systematische debugging in plaats van random guessing
- Identificeert welke aannames fout waren
- Vindt gerelateerde bugs voordat ze problemen veroorzaken
- Nieuwe developers kunnen complexe systemen debuggen

**Toepassing:**
- Developer tooling
- Incident response
- Post-mortem analyse
- Onboarding van nieuwe developers

---

## Technische Werking

### Knowledge Format

RSIR accepteert simpele text files:

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

### Algemene Reasoning Rules

RSIR gebruikt algemene regels die voor alle cases werken:

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

Deze regels zijn **niet scenario-specifiek** - ze werken voor elke ziekte, elke test.

---

## Waarom Dit Anders Is Dan LLMs

| Aspect | LLM (GPT, Claude) | RSIR |
|--------|-------------------|------|
| Bij onzekerheid | Hallucineert een antwoord | Toont wat het niet weet |
| Reasoning | Verborgen in weights | Volledig traceerbaar |
| Kennis updaten | Hertrainen nodig | Edit text file |
| Nieuwe cases | Kan onverwacht falen | Redeneert consistent |
| Audit trail | Beperkt | 100% - elke stap gedocumenteerd |
| Backward propagation | Niet mogelijk | Automatisch bij nieuw bewijs |

---

## De Kracht van Backward Propagation

Wanneer nieuw bewijs binnenkomt dat oude conclusies ontkracht:

1. **LLM:** Weet niet dat eerdere conclusie fout was
2. **RSIR:** Herziet automatisch alle afhankelijke conclusies

Voorbeeld Detective Case:
```
Initieel: Sarah heeft alibi → lage verdenking
Nieuw bewijs: Alibi is vals
RSIR: Herziet automatisch → hoge verdenking + "consciousness of guilt"
```

Dit is cruciaal voor domeinen waar informatie verandert (onderzoeken, diagnoses, debugging).

---

## Technische Specificaties

- **Taal:** Rust
- **Binaries:** `definition_demo`, `medical_knowledge_demo`, `detective_knowledge_demo`, `debugging_knowledge_demo`
- **Knowledge format:** Text files (custom format)
- **State format:** JSON
- **Semantic network:** 295.955 edges (bij 2707 definities)

---

## Volgende Stappen

1. **API endpoint** - REST API voor integratie
2. **Web UI** - Visuele interface voor kennisbeheer
3. **Custom knowledge generator** - Tool om eigen domeinkennis te maken
4. **ICS integratie** - Koppeling met andere cognitieve modules

---

## Contact

Oscurso Labs
https://oscurso.com
