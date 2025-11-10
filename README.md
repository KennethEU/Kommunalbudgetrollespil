# 🎭 Budgetrollespil: Kommunalpolitik i praksis

Et interaktivt undervisningsværktøj til at simulere budgetforhandlinger i et kommunalt byråd. Systemet hjælper lærere med at organisere elever i interessegrupper og byråd, hvor de skal forhandle om fordeling af 100 millioner kroner.

## 📋 Formål

Dette rollespil giver eleverne hands-on erfaring med:

- **Demokratiske processer** - hvordan interessegrupper forhandler i et byråd
- **Magtfordeling** - forskellige grupper har forskellig politisk magt (stemmevægt)
- **Kompromiser** - nødvendigheden af at forhandle og give efter
- **Budgetprioritering** - hvordan man fordeler begrænsede ressourcer
- **Politisk realisme** - forståelse for at ikke alle får lige meget

## 🚀 Kom i gang

### Installation
Ingen installation nødvendig! Åbn blot `index.html` i en moderne webbrowser.

### Hurtig start
1. Åbn `index.html` i din browser
2. Vælg input-metode:
   - **Elevnavne** - indtast navne manuelt (kopiér fra Lectio)
   - **Antal elever** - vælg et tal (systemet navngiver automatisk)
3. Klik "Lav interessegrupper"
4. Klik "Lav byråd"
5. Lad eleverne forhandle!

## 📖 Sådan fungerer rollespillet

### FASE 1: Interessegrupper (ca. 20 minutter)

Eleverne inddeles tilfældigt i 5 interessegrupper:

| Gruppe | Interesseområde | Rolle |
|--------|-----------------|-------|
| 👨‍👩‍👧‍👦 | **Børnefamilier i Tilst** | Vil have bedre skoler, legepladser, børnehaver |
| 👴👵 | **Ældre og pårørende** | Vil have bedre plejecentre, hjemmehjælp |
| 🎓🎵 | **Unge og studerende** | Vil have bedre fritidstilbud, kulturhuse, uddannelse |
| 💼🏢 | **Erhvervsliv** | Vil have infrastruktur, erhvervsudvikling |
| 🚴🌳 | **Klima og transport** | Vil have grønne områder, cykelstier, bæredygtighed |

**Opgave for eleverne:**
- Formuler 3 konkrete krav med beløb
- Forbered argumenter for jeres sag
- Vælg eventuelt en talsperson

### FASE 2: Byrådene (ca. 20-30 minutter)

Systemet danner automatisk byråd (matrixgrupper) med én repræsentant fra hver interessegruppe.

**Særlige regler:**
- Hver interessegruppe har **forskellig stemmevægt** (2, 4 eller 6 stemmer)
- Hvis 2 personer fra samme gruppe sidder i et byråd, **deles stemmerne**
- Byrådet skal fordele **præcis 100 millioner kroner**
- Beslutningen skal have **flertal** (mere end halvdelen af stemmerne)

**Opgave for eleverne:**
- Forhandl om budgetfordelingen
- Lyt til de andre gruppers argumenter
- Find kompromiser
- Stem for eller imod det endelige forslag

**Eksempel på stemmevægt:**
```
Byråd 1:
- Maria (Børnefamilier) → 6 stemmer
- Jonas (Ældre) → 4 stemmer
- Emma (Unge) → 2 stemmer
- Lars (Erhverv) → 4 stemmer
- Sarah (Klima) → 2 stemmer

Total: 18 stemmer
Flertal kræver: 10 stemmer
```

### FASE 3: Resultatindtastning og analyse

Efter forhandlingerne indtaster læreren/eleverne:

1. **Budgetfordeling** - hvor mange millioner hver interessegruppe fik
2. **Stemmeadfærd** - hvem stemte for/imod forslaget

Systemet genererer automatisk:

- ✅ **Validering** - tjekker at totalen er præcis 100 mio.
- 📊 **Statistik** - sammenligner de forskellige byråds beslutninger
- 🗳️ **Stemmeanalyse** - viser om bestemte grupper oftere stemte for/imod

## ✨ Funktioner

### Grundlæggende
- ✅ **Automatisk gruppeinddeling** - fordeler elever tilfældigt og jævnt
- ✅ **Matrix-gruppering** - laver byråd med én fra hver interessegruppe
- ✅ **Stemmevægt-system** - simulerer reel magtfordeling
- ✅ **Fleksibel input** - navne fra Lectio eller bare et antal

### Avancerede funktioner
- 💾 **Auto-gem** - arbejdet gemmes automatisk i browseren
- ➕ **Tilføj forsinkede elever** - selv efter grupper er dannet
- 📊 **Live statistik** - sammenlign byrådenes beslutninger
- 🗳️ **Stemmeanalyse** - se hvilke grupper der stemte for/imod
- ✅ **Validering** - tjek at budgettet går op

### Lærerværktøjer
- 🎲 **Tilfældig fordeling** - sikrer fair opdeling
- 🔄 **Start forfra** - nulstil til ny klasse
- 💡 **Indbyggede guides** - hjælpetekster og forklaringer
- 📱 **Responsivt design** - virker på tablets og mobil

## 🎓 Pædagogiske læringspunkter

### Efter rollespillet kan I diskutere:

**Demokrati og magt:**
- Hvorfor havde nogle grupper flere stemmer?
- Er det retfærdigt at nogle har mere magt?
- Hvordan er det i det virkelige byråd?

**Forhandling og kompromis:**
- Fik alle grupper noget af det de ville have?
- Hvilke grupper måtte give mest efter?
- Hvordan opnåede I enighed?

**Prioritering:**
- Hvilke områder blev prioriteret højest?
- Var der forskel mellem byrådene?
- Hvorfor blev der prioriteret forskelligt?

**Minoriteter vs. flertal:**
- Hvad skete der hvis du var i en gruppe med få stemmer?
- Skulle beslutninger kræve enstemmighed eller bare flertal?
- Hvordan kan minoriteter få indflydelse?

### Sammenligning med virkeligheden

Efter rollespillet kan I se på:
- [Aarhus Kommunes budget](https://www.aarhus.dk/da/politik/budget-og-oekonomi/)
- Hvordan ser magtfordelingen ud i jeres eget byråd?
- Hvilke interessegrupper har mest indflydelse i virkeligheden?

## 🔧 Tekniske detaljer

### Teknologi
- **Frontend:** React 18 (standalone, ingen build nødvendig)
- **Styling:** Vanilla CSS (intet framework)
- **Persistens:** localStorage (auto-gem)
- **Browser:** Moderne browsers (ES6+)

### Datafiler
- **index.html** - Hele applikationen (standalone fil)
- **localStorage** - Automatisk gemt data (slettes ved "Start forfra")

### Dataformat for gemt session
```javascript
{
  inputMode: 'names' | 'count',
  studentCount: number,
  studentNames: string,
  interestGroups: array,
  byraad: array,
  budgetResults: array,
  groupVotes: object
}
```

## 🎨 Tilpasning

### Justér stemmevægt
Inden du laver interessegrupper kan du justere hvor mange stemmer hver gruppe har:
- Minimum: 2 stemmer
- Maksimum: 6 stemmer
- Spring: Kun lige tal (2, 4, 6)

### Standardindstilling
Stemmerne fordeles tilfældigt ved start for at simulere at forskellige grupper har forskellig politisk magt.

## 📱 Browser-kompatibilitet

| Browser | Understøttet | Note |
|---------|-------------|------|
| Chrome 90+ | ✅ | Anbefalet |
| Edge 90+ | ✅ | Anbefalet |
| Firefox 88+ | ✅ | Virker godt |
| Safari 14+ | ✅ | Virker godt |
| IE 11 | ❌ | Ikke understøttet |

## ⚠️ Bemærk

- **Data gemmes kun lokalt** - hvis du sletter browserdata, mistes dit arbejde
- **Inkognito-mode** - data gemmes ikke mellem sessions
- **Flere faner** - åbn ikke samme session i flere faner samtidig
- **Print-funktion** - er fjernet (brug browserens screenshot i stedet)

## 🐛 Fejlfinding

### "Data gemt automatisk" vises ikke?
→ Tjek om du har blokeret localStorage i din browser

### Kan ikke indtaste navne?
→ Tjek at du har valgt "📝 Brug elevnavne" øverst

### Byråd laver ikke lige grupper?
→ Dette er normalt - hvis der er 21 elever og 4 byråd, vil nogle byråd have ekstra medlemmer

### Total bliver ikke præcis 100 mio.?
→ Brug decimaler (fx 33.3) for at få det til at gå op

## 📄 Licens

Dette projekt er udviklet til undervisningsbrug og er frit tilgængeligt.

## 🤝 Feedback og forbedringer

Har du forslag til forbedringer eller har fundet en fejl?
- Skriv til din IT-support
- Eller lav en kopi og tilpas efter behov

## 📚 Ressourcer

### Relevante læremidler
- Samspillet mellem stat, regioner og kommuner
- Demokrati på mange niveauer
- Interessegrupper og lobbyisme

### Yderligere læsning
- [Kommunernes Landsforening (KL)](https://www.kl.dk/)
- [Undervisningsministeriet - Demokrati og medborgerskap](https://www.uvm.dk/)

---

**God fornøjelse med rollespillet!** 🎭🏛️
