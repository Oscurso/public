# WIM - Working Intent Memory

## Toepassing: Juridisch Zaakbeheer

### Wat is WIM?

WIM is een cognitieve module die **intent tracking en context behoud** beheert in high-stakes omgevingen. Het beantwoordt de vraag: "Wat ben ik aan het doen en waarom?"

**Kernprincipe:** In de juridische praktijk waar context verlies gemiste deadlines en aansprakelijkheid betekent, zorgt WIM ervoor dat complex zaakonderzoek onderbrekingen overleeft en dat rechtbank deadlines nooit gemist worden.

---

## Hoe Werkt Het?

1. **Intent Creatie** - Zaakdoelen geregistreerd met deadlines en prioriteit
2. **Taak Decompositie** - Complexe zaken opgebroken in trackbare taken
3. **Focus Management** - Trackt onderzoeksdiepte en declarabele tijd
4. **Onderbreking Afhandeling** - Evalueert rechtbank deadlines: nu afhandelen of uitstellen?
5. **Context Behoud** - Legt volledige onderzoeksstaat vast voor naadloze hervatting
6. **Voortgang Tracking** - Monitort voltooiing over meerdere gelijktijdige zaken

---

## Juridisch Zaakbeheer Scenario

### De Uitdaging

Een senior procesadvocaat met 12 gelijktijdige zaken. Diep in procesvoorbereiding voor een €7.8M productaansprakelijkheidszaak wanneer een spoed kort geding deadline arriveert - indienen binnen 2 uur. Hoe:

- Reageer je op de noodsituatie zonder je procesvoorbereiding onderzoek te verliezen?
- Behoud je je exacte positie in documenten, verhoren en jurisprudentie?
- Beheer je meerdere rechtbank deadlines tegelijk?
- Hervat je complex juridisch onderzoek naadloos na de noodsituatie?

### WIM in Actie

| Tijd | Gebeurtenis | WIM Reactie |
|------|-------------|-------------|
| 14:20 | Procesvoorbereiding begint | Creëert intent, trackt getuige-deskundige voorbereiding |
| 14:47 | Diep onderzoek | Pagina 14/23 van expert outline, verhoor bookmarks opgeslagen |
| 14:47 | KORT GEDING SPOED | Deadline over 2u 13m, evalueert urgentie: 0.94 vs drempel 0.80 |
| 14:47 | Beslissing | HANDLE_NOW - rechtbank deadline is absoluut |
| 14:53 | Context bewaard | Onderzoeksstaat opgeslagen, schakelt naar kort geding |
| 16:47 | Kort geding ingediend | 13 minuten voor deadline |
| 20:35 | Terug naar procesvoorbereiding | Herstelt context in 2 minuten |

---

## Demo Resultaten

### Rechtbank Deadline Analyse

```
Huidige intent urgentie:    0.72 (Procesvoorbereiding - belangrijk maar niet direct)
Onderbreking urgentie:      0.94 (Rechtbank deadline - mag niet gemist worden)
Onderbreking drempel:       0.80

→ Rechtbank deadline OVERSCHRIJDT drempel met 0.14
→ Beslissing: ONMIDDELLIJK AFHANDELEN
→ Rationale: Rechtbankregels zijn absoluut - missen betekent zaak afgewezen
```

WIM begrijpt de juridische realiteit - rechtbank deadlines zijn niet-onderhandelbaar. De beslissing om procesvoorbereiding te onderbreken is automatisch en gedocumenteerd.

### Onderzoek Context Behoud

Bij het schakelen naar de kort geding noodsituatie legde WIM vast:

- **Document positie:** expert_testimony_outline_stevens_v3.docx (pagina 14/23)
- **Verhoor bookmarks:** Stevens transcript (pp. 47-52 gemarkeerd)
- **Jurisprudentie onderzoek:** 3 Hoge Raad zaken open
  - Barker v. Lull (1978) - productdefect standaard
  - Soule v. GM (1994) - ontwerpdefect jury instructies
- **Mentale context:** "Dr. Stevens moet FEA modellering vereenvoudigen voor jury - gebruik paperclip buig-analogie"
- **Declarabele tijd:** 1u 32m bewaard (hervat op dezelfde klok)

**Context herstel tijd: 2 minuten** (vs 2-3 uur zonder WIM)

### Multi-Zaak Beheer

Tijdens de noodsituatie beheerde WIM drie gelijktijdige zaak-intents:

| Zaak | Prioriteit | Status | Deadline |
|------|------------|--------|----------|
| Martinez kort geding | Kritiek | Actief | Vandaag 17:00 |
| Johnson procesvoorbereiding | Hoog | Gepauzeerd | 13 dagen |
| Thompson discovery | Medium | Gedelegeerd | Vandaag EOD |

WIM delegeerde automatisch de Thompson discovery aan een medewerker met instructies: "Review voor indienen om 16:30"

### Deadline Prestaties

| Indiening | Deadline | Werkelijk | Marge |
|-----------|----------|-----------|-------|
| Martinez kort geding | 17:00 | 16:47 | 13 minuten |
| Thompson Discovery | 17:00 | 16:51 | 9 minuten |

**Rechtbank deadlines gehaald: 2/2 (100%)**

---

## Prestatie Metrics

### Einde-Dag Samenvatting

| Metric | Waarde |
|--------|--------|
| Actieve Zaken | 3 |
| Rechtbank Deadlines Gehaald | 2/2 (100%) |
| Context Switches | 4 |
| Gem. Switch Tijd | 2.8 minuten |
| Johnson Procesvoorbereiding | 6.2 declarabele uren |
| Martinez Kort Geding | 5.5 declarabele uren |
| Thompson Discovery | 0.4 declarabele uren |
| Totaal Declarabel | 12.1 uren |
| Realisatiegraad | 96% |
| Onderzoek Integriteit | 100% bewaard |
| Jurisprudentie Kruisbesmetting | 0 |

---

## Waarom WIM Belangrijk Is in de Juridische Praktijk

### Zonder WIM

- ✗ 45 minuten gemiddeld om juridische onderzoekscontext te herbouwen
- ✗ €385 declarabele waarde verloren per context switch
- ✗ Jurisprudentie verwarring over meerdere zaken
- ✗ 2-3 uur om te vinden "waar was ik" in onderzoek
- ✗ 78% declaratie realisatie (tijd verloren aan reconstructie)
- ✗ Risico op gemiste deadlines tijdens complexe zaken
- ✗ "Voor welke zaak was dat precedent ook alweer?"

### Met WIM

- ✓ 2 minuten context herstel (96% sneller)
- ✓ 96% declaratie realisatie (18% verbetering)
- ✓ Nul zaakverwarring - complete isolatie tussen zaken
- ✓ Rechtbank deadlines automatisch geprioriteerd
- ✓ Onderzoeksstaat bewaard tot exacte pagina/paragraaf
- ✓ Complete declarabele tijd tracking over onderbrekingen
- ✓ Delegatie met volledige context overdracht

---

## ROI Berekening

**Per Advocaat: €630.000/jaar**

Gebaseerd op:
- 45 minuten bespaard per context switch × 4 switches/dag = 3 uur/dag
- 3 uur × €385/uur = €1.155/dag herwonnen declarabele tijd
- 250 werkdagen × €1.155 = €289.000 in herwonnen declaraties
- 18% realisatie verbetering op €1.8M jaarlijkse declaraties = €324.000
- Verminderde aansprakelijkheid door gemiste deadlines = onbetaalbaar

---

## Waarom Dit Anders Is Dan Practice Management Software

| Aspect | Traditionele PM Software | WIM |
|--------|--------------------------|-----|
| Focus | Agenda en deadlines | Intent en context management |
| Onderzoeksstaat | Niet getrackt | Bewaard tot paginanummer |
| Onderbrekingen | Handmatige prioritering | Automatische urgentie evaluatie |
| Context switching | Je staat er alleen voor | 2 minuten complete herstel |
| Declaratie tracking | Start/stop timers | Continu over onderbrekingen |
| Multi-zaak | Aparte silo's | Geünificeerd intent management |
| Mentale context | Verloren | "Paperclip analogie" bewaard |

---

## Technische Specificaties

- **Taal:** Rust
- **Binary:** `wim` (standalone executable, cross-platform)
- **State format:** JSON
- **Input:** Knowledge-driven scenarios
- **Output:** CLI + JSON + Reports
- **Integratie:** ICS-ready voor volledige cognitieve stack

---

## Doelgroep

- **Advocatenkantoren** - Procesrecht, ondernemingsrecht, IE
- **In-House Legal** - Juridische afdelingen
- **Legal Tech** - Practice management verbetering
- **Zelfstandige Advocaten** - Multi-zaak beheer
- **Legal Operations** - Efficiëntie optimalisatie
- **Compliance Teams** - Regelgevende deadline beheer

---

## Orde van Advocaten Afstemming

WIM ondersteunt compliance met:

- **Gedragsregels** - Competentie en zorgvuldigheid vereisten
- **Declaratie Ethiek** - Accurate tijdregistratie
- **Cliënt Communicatie** - Status tracking en updates
- **Belangenconflicten** - Zaak isolatie en tracking
- **Deadline Beheer** - Rechtbank regel compliance

---

## Volgende Stappen

1. **ICS Integratie** - Koppeling met ECE, RSIR, CDE voor complete cognitieve loop
2. **Document Management Integratie** - iManage, NetDocuments connectiviteit
3. **Rechtbank Agenda Sync** - Automatische deadline import
4. **Onderzoeksplatform Integratie** - Legal Intelligence, Kluwer Navigator bookmarks
5. **Declaratiesysteem Brug** - Directe tijdregistratie naar administratie

---

## Contact

Oscurso Labs
https://oscurso.com
