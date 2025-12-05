# Oscurso Labs - Cognitieve Architectuur

<p align="center">
  <img src="https://img.shields.io/badge/Status-Actieve%20Ontwikkeling-green" alt="Status">
  <img src="https://img.shields.io/badge/Taal-Rust-orange" alt="Rust">
  <img src="https://img.shields.io/badge/Licentie-Proprietary-blue" alt="Licentie">
  <img src="https://img.shields.io/badge/AVG-Compliant-success" alt="AVG">
</p>

## 🧠 Wat Is Dit?

**Oscurso** bouwt een **deterministische cognitieve architectuur** - een alternatieve benadering van AI die transparantie, verklaarbaarheid en Europese datasoevereiniteit voorop stelt.

In tegenstelling tot black-box neurale netwerken waar je niet kunt zien *waarom* een beslissing is genomen, zijn Oscurso's cognitieve modules **volledig traceerbaar**. Elke redeneerstap, elke beslissing, elk inzicht kan worden geaudit en uitgelegd.

> **"Niet alleen een antwoord, maar de redenering die ernaartoe leidde."**

---

## 🏗️ Architectuur Overzicht

De Oscurso cognitieve stack bestaat uit **5 verbonden modules**, elk beantwoordt een fundamentele cognitieve vraag:

```
┌─────────────────────────────────────────────────────────────────┐
│                    OSCURSO COGNITIEVE LOOP                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│   ┌─────────┐     ┌─────────┐     ┌─────────┐                   │
│   │   ECE   │ ──▶ │  RSIR   │ ──▶ │   CDE   │                   │
│   │Curiosity│     │Redeneren│     │ Kritiek │                   │
│   └─────────┘     └─────────┘     └─────────┘                   │
│        │                               │                         │
│        │         ┌─────────┐           │                         │
│        └───────▶ │   WIM   │ ◀─────────┘                         │
│                  │ Intentie│                                     │
│                  └─────────┘                                     │
│                       │                                          │
│                       ▼                                          │
│                  ┌─────────┐                                     │
│                  │   ODI   │                                     │
│                  │ Dromen  │                                     │
│                  └─────────┘                                     │
│                       │                                          │
│                       └──────────────▶ [voert terug naar ECE]    │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

---

## 📦 De Modules

| Module | Volledige Naam | Vraag | Doel |
|--------|----------------|-------|------|
| **[ECE](./ECE)** | Emergent Curiosity Engine | *"Wat wil ik weten?"* | Genereert vragen, identificeert kennishiaten, drijft exploratie |
| **[RSIR](./RSIR)** | Recursive Self-Interrogating Reasoning | *"Wat kan ik concluderen?"* | Multi-laag redeneren met zelfkritiek en betrouwbaarheidsregistratie |
| **[CDE](./CDE)** | Critical Decision Engine | *"Klopt dit wel?"* | Valideert conclusies, identificeert logische fouten, stresstests redenering |
| **[WIM](./WIM)** | Working Intent Memory | *"Wat ben ik aan het doen?"* | Beheert actieve taken, handelt onderbrekingen af, bewaart context |
| **[ODI](./ODI)** | Overnight Dream Integration | *"Wat heb ik geleerd?"* | Consolideert kennis, vindt patronen, genereert inzichten |

---

## 🎯 Kernfuncties

### Deterministisch & Traceerbaar
Elke beslissing heeft een duidelijke audit trail. Geen verborgen lagen, geen onverklaarbare outputs.

### Europese Datasoevereiniteit
Gebouwd voor AVG-compliance. Jouw data blijft transparant en onder jouw controle.

### Echte Werkende Systemen
Geen vaporware. Elke module heeft werkende demo's met echte outputs die je kunt draaien.

### Industrie-Bewezen
Demo's voor Healthcare, Finance, Legal, Research en Cybersecurity sectoren.

---

## 📊 Echte Systeem Output

### ECE - Emergent Curiosity Engine
```
[CURIOSITY] Gegenereerd 12 vragen over patiënt behandelpatronen
[DEPTH 1] "Wat veroorzaakt heropname binnen 30 dagen?"
[DEPTH 2] "Zijn er medicijninteractie patronen die we missen?"
[DEPTH 3] "Kunnen leefstijlfactoren behandelresistentie voorspellen?"
```

### RSIR - Recursive Self-Interrogating Reasoning
```
[LAAG 1] Initiële analyse: 3 hypotheses gevormd
[LAAG 2] Zelfkritiek: Hypothese B geëlimineerd (onvoldoende bewijs)
[LAAG 3] Betrouwbaarheid: 0.87 voor resterende conclusies
[OUTPUT] Aanbeveling met volledige redeneerketen
```

### CDE - Critical Decision Engine
```
[ANALYSE] Beslissing: Keur €2.4M infrastructuurinvestering goed
[DEVIL'S ADVOCATE] Gevonden 3 potentiële faalmodi
[STRESS TEST] Scenario analyse: 2/5 randgevallen vereisen mitigatie
[VERDICT] VOORWAARDELIJK GOEDGEKEURD met risicomitigaties
```

### WIM - Working Intent Memory
```
[INTENT] Primair: Voltooi kwartaalrapport (60% voortgang)
[INTERRUPT] Urgent: Productie-incident (urgentie: 0.92)
[PRESERVE] Opgeslagen: cursorpositie, open bestanden, mentaal model
[RESTORE] Context hersteld in 47 seconden (vs 15min handmatig)
```

### ODI - Overnight Dream Integration
```
[COLLECTING] Verzameld 30 herinneringen
[PATTERN FINDING] Gevonden 30 patronen
[ASSOCIATING] Gecreëerd 38 associaties
[INSIGHT] Cross-domein verbinding ontdekt (nieuwheid: 0.90)
```

> **Geïnteresseerd in een live demo?** [Neem contact op](mailto:contact@oscurso.com) om een demonstratie met jouw eigen data in te plannen.

---

## 🏭 Industrie Toepassingen

| Industrie | Use Case | Module Focus |
|-----------|----------|--------------|
| **Healthcare** | Behandelpatroon ontdekking, medicijninteracties | ECE, ODI |
| **Finance** | Risico-analyse, marktcorrelatie ontdekking | CDE, ODI |
| **Legal** | Jurisprudentie analyse, strategie optimalisatie | RSIR, CDE |
| **Research** | Hypothese generatie, methodologie patronen | ECE, RSIR |
| **Cybersecurity** | Threat intelligence consolidatie | ODI, CDE |

---

## 📚 Documentatie

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

## 🔧 Technische Stack

- **Taal:** Rust (performance, veiligheid, voorspelbaarheid)
- **State Management:** JSON-gebaseerde knowledge graphs
- **Integratie:** ICS (Integrated Cognitive System) orchestratie
- **Deployment:** Standalone binaries, cross-platform
- **API:** REST endpoints (gepland)

---

## 🌍 Waarom Oscurso?

### Het Probleem met Huidige AI

| Neurale Netwerken | Oscurso Aanpak |
|-------------------|----------------|
| Black box beslissingen | Volledig traceerbare redenering |
| Kan "waarom" niet uitleggen | Complete audit trail |
| Datasoevereiniteit zorgen | AVG-compliant by design |
| Vereist enorme rekenkracht | Efficiënte, gerichte verwerking |
| Hallucinaties gebruikelijk | Deterministisch, verifieerbaar |

### Europese AI Soevereiniteit

Wij geloven dat Europa zijn eigen benadering van AI nodig heeft - een die aansluit bij Europese waarden van privacy, transparantie en individuele rechten. Oscurso is vanaf de grond opgebouwd met deze principes.

---

## 📈 Roadmap

- [x] ECE - Emergent Curiosity Engine
- [x] RSIR - Recursive Self-Interrogating Reasoning  
- [x] CDE - Critical Decision Engine
- [x] WIM - Working Intent Memory
- [x] ODI - Overnight Dream Integration
- [ ] ICS - Volledige cognitieve loop integratie
- [ ] API endpoints voor enterprise integratie
- [ ] Multi-agent samenwerking
- [ ] Continu leren zonder vergeten

---

## 🤝 Contact

**Oscurso Labs**

- 🌐 Website: [oscurso.com](https://oscurso.com)
- 📧 Email: [info@oscurso.com](mailto:info@oscurso.com)
- 🔗 LinkedIn: [Oscurso](https://linkedin.com/company/oscurso)

---

## 📜 Licentie

Proprietary - Alle Rechten Voorbehouden

Deze repository bevat publieke demonstraties en documentatie. De onderliggende systemen en algoritmes zijn eigendom van Oscurso Labs.

---

<p align="center">
  <strong>Transparante AI Bouwen voor Europa</strong><br>
  <em>Niet alleen intelligentie. Begrijpelijke intelligentie.</em>
</p>
