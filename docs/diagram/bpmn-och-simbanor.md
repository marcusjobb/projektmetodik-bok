---
title: BPMN och simbanor
description: "Processkartor visar vem som gör vad, i vilken ordning, när ett arbete går mellan flera roller. Ett simbanediagram räcker långt — BPMN är standarden när processen ska vara exakt."
parent: Diagram & analysverktyg
nav_order: 10
---

# BPMN och simbanor

## Grundidén

En processkarta visar **hur ett arbete flyttar sig mellan människor**. Varje roll får en egen *simbana* — en rad i diagrammet, som en bana i en simhall — och stegen ritas i den bana där de görs. När en pil korsar en banlinje lämnas arbetet över till någon annan, och det är oftast där det går fel: ärenden blir liggande, information tappas bort, ingen vet vems tur det är.

Det finns två nivåer:

- **Simbanediagram** (swimlane) — rutor och pilar i banor. Inga särskilda symboler, alla förstår det direkt.
- **BPMN** (Business Process Model and Notation) — en standard med bestämda symboler för händelser, beslut och meddelanden. Mer exakt, och kan läsas av verktyg som kör processen automatiskt.

## Vad används det till?

- **Kartlägga hur det fungerar idag** — innan man förbättrar något måste teamet vara överens om nuläget
- **Hitta flaskhalsar och överlämningar** — varje pil mellan två banor är en risk för väntan
- **Förklara en process för en ny kollega** eller för kunden
- **Specificera ett system** — vilka steg ska appen sköta, och vilka gör en människa?

## Delarna och vad de heter

Bilden visar de viktigaste BPMN-symbolerna. Ett simbanediagram använder bara banorna, rutorna och pilarna — resten är BPMN:s tillägg.

<svg class="dg" viewBox="0 0 720 390" role="img" aria-labelledby="bp1-t" xmlns="http://www.w3.org/2000/svg">
<title id="bp1-t">BPMN-diagram med namngivna delar: pool, bana, starthändelse, aktivitet, exklusiv gateway, mellanhändelse, sluthändelse, sekvensflöde, meddelandeflöde och dataobjekt</title>
<defs>
<marker id="bp1-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
<marker id="bp1-o" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10" class="line strong"/></marker>
<marker id="bp1-c" viewBox="0 0 10 10" refX="5" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><circle cx="5" cy="5" r="4" class="box"/></marker>
</defs>
<rect class="line strong" x="20" y="20" width="550" height="260"/>
<line class="line strong" x1="50" y1="20" x2="50" y2="280"/>
<line class="line" x1="80" y1="20" x2="80" y2="280"/>
<line class="line" x1="50" y1="150" x2="570" y2="150"/>
<text x="41" y="150" text-anchor="middle" class="title" transform="rotate(-90 41 150)">IT-konsultbolaget</text>
<text x="70" y="85" text-anchor="middle" transform="rotate(-90 70 85)">Servicedesk</text>
<text x="70" y="215" text-anchor="middle" transform="rotate(-90 70 215)">Utvecklare</text>
<circle class="box" cx="130" cy="85" r="15"/>
<line class="line strong" x1="145" y1="85" x2="165" y2="85" marker-end="url(#bp1-f)"/>
<rect class="box" x="165" y="60" width="100" height="50" rx="10"/><text x="215" y="90" text-anchor="middle">Registrera</text>
<line class="line strong" x1="265" y1="85" x2="300" y2="85" marker-end="url(#bp1-f)"/>
<path class="box" d="M320 65L340 85L320 105L300 85Z"/>
<line class="line strong" x1="312" y1="77" x2="328" y2="93"/><line class="line strong" x1="328" y1="77" x2="312" y2="93"/>
<line class="line strong" x1="340" y1="85" x2="380" y2="85" marker-end="url(#bp1-f)"/><text x="360" y="78" text-anchor="middle" class="muted">enkelt</text>
<rect class="box" x="380" y="60" width="100" height="50" rx="10"/><text x="430" y="90" text-anchor="middle">Lös direkt</text>
<line class="line strong" x1="480" y1="85" x2="515" y2="85" marker-end="url(#bp1-f)"/>
<circle class="solid" cx="530" cy="85" r="15"/><circle class="box" cx="530" cy="85" r="11"/>
<path class="line strong" d="M320 105V190" marker-end="url(#bp1-f)"/><text x="314" y="140" text-anchor="end" class="muted">komplext</text>
<rect class="box" x="265" y="190" width="110" height="50" rx="10"/><text x="320" y="220" text-anchor="middle">Åtgärda fel</text>
<line class="line strong" x1="375" y1="215" x2="405" y2="215" marker-end="url(#bp1-f)"/>
<circle class="box" cx="420" cy="215" r="15"/><circle class="line strong" cx="420" cy="215" r="11"/>
<text x="420" y="255" text-anchor="middle" class="muted">review klar</text>
<path class="line strong" d="M435 215H530V100" marker-end="url(#bp1-f)"/>
<line class="line dash" x1="211" y1="110" x2="211" y2="190"/>
<path class="box" d="M197 190H217L225 198V226H197Z"/><path class="line" d="M217 190V198H225"/>
<line class="leader" x1="211" y1="229" x2="211" y2="236"/><text x="211" y="250" text-anchor="middle" class="part">Dataobjekt</text>
<rect class="line strong" x="20" y="330" width="550" height="45"/><text x="295" y="358" text-anchor="middle" class="title">Kund</text>
<line class="line dash" x1="130" y1="330" x2="130" y2="100" marker-start="url(#bp1-c)" marker-end="url(#bp1-o)"/>
<text x="138" y="318" class="muted">felanmälan</text>
<line class="leader" x1="130" y1="50" x2="130" y2="70"/><text x="130" y="46" text-anchor="middle" class="part">Starthändelse</text>
<line class="leader" x1="320" y1="50" x2="320" y2="65"/><text x="320" y="46" text-anchor="middle" class="part">Exklusiv gateway</text>
<line class="leader" x1="430" y1="50" x2="430" y2="60"/><text x="430" y="46" text-anchor="middle" class="part">Aktivitet</text>
<line class="leader" x1="570" y1="30" x2="592" y2="30"/><text x="598" y="34" class="part">Pool</text>
<line class="leader" x1="545" y1="85" x2="592" y2="85"/><text x="598" y="89" class="part">Sluthändelse</text>
<line class="leader" x1="570" y1="150" x2="592" y2="150"/><text x="598" y="154" class="part">Bana (lane)</text>
<line class="leader" x1="530" y1="180" x2="592" y2="180"/><text x="598" y="184" class="part">Sekvensflöde</text>
<line class="leader" x1="434" y1="222" x2="592" y2="260"/><text x="598" y="264" class="part">Mellanhändelse</text>
<line class="leader" x1="130" y1="295" x2="592" y2="300"/><text x="598" y="304" class="part">Meddelandeflöde</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Pool** | Stor ram med namnet i en lodrät list till vänster | En organisation eller ett system — en egen "spelare". Kunden är ofta en egen pool |
| **Bana** (lane) | Rad inuti poolen | En roll, ett team eller en avdelning inom poolen |
| **Starthändelse** | Tunn cirkel | Det som sätter igång processen |
| **Mellanhändelse** | Dubbel cirkel | Något som händer *under* processen — ofta en väntan ("review klar", "svar mottaget") |
| **Sluthändelse** | Tjock cirkel | Processen är klar |
| **Aktivitet / uppgift** | Rektangel med rundade hörn | Ett arbetssteg som någon utför. Namnge med verb: "Registrera", inte "Registrering" |
| **Exklusiv gateway** (X) | Romb med kryss | Ett beslut — flödet tar **en** av vägarna. Skriv villkoren på pilarna |
| **Parallell gateway** (+) | Romb med plus | Flödet delas i vägar som körs **samtidigt** — och sammanfogas med en likadan romb (se exemplet) |
| **Sekvensflöde** | Heldragen pil | Ordningen mellan steg *inom* en pool |
| **Meddelandeflöde** | Streckad pil med ring i början | Information som skickas *mellan* pooler — mejl, ärende, API-anrop |
| **Dataobjekt** | Papper med vikt hörn, kopplat med streckad linje | Information som skapas eller används i ett steg |

**Tumregel:** sekvensflöden stannar inom en pool, meddelandeflöden korsar poolgränsen. Det är den vanligaste BPMN-regeln att bryta.

## Exempel — supportärende hos ett IT-konsultbolag

En kund anmäler ett fel i systemet konsultbolaget har byggt. Servicedesk tar emot ärendet; är felet känt svarar de direkt, annars går det vidare till en utvecklare.

Först som ett **enkelt simbanediagram** — så här ritar teamet på whiteboarden första gången:

<svg class="dg" viewBox="0 0 720 280" role="img" aria-labelledby="bp2-t" xmlns="http://www.w3.org/2000/svg">
<title id="bp2-t">Simbanediagram för ett supportärende med banorna Kund, Servicedesk och Utvecklare</title>
<defs>
<marker id="bp2-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<rect class="line strong" x="20" y="20" width="680" height="240"/>
<line class="line" x1="20" y1="100" x2="700" y2="100"/>
<line class="line" x1="20" y1="180" x2="700" y2="180"/>
<line class="line" x1="130" y1="20" x2="130" y2="260"/>
<text x="75" y="65" text-anchor="middle" class="title">Kund</text>
<text x="75" y="145" text-anchor="middle" class="title">Servicedesk</text>
<text x="75" y="225" text-anchor="middle" class="title">Utvecklare</text>
<rect class="box" x="150" y="40" width="110" height="40" rx="8"/><text x="205" y="65" text-anchor="middle">Anmäler fel</text>
<rect class="box" x="570" y="40" width="120" height="40" rx="8"/><text x="630" y="65" text-anchor="middle">Får svar</text>
<rect class="box" x="150" y="120" width="110" height="40" rx="8"/><text x="205" y="145" text-anchor="middle">Registrerar</text>
<rect class="box" x="570" y="120" width="120" height="40" rx="8"/><text x="630" y="145" text-anchor="middle">Svarar kunden</text>
<rect class="box" x="290" y="200" width="110" height="40" rx="8"/><text x="345" y="225" text-anchor="middle">Rättar felet</text>
<rect class="box" x="430" y="200" width="110" height="40" rx="8"/><text x="485" y="225" text-anchor="middle">Testar</text>
<line class="line strong" x1="205" y1="80" x2="205" y2="120" marker-end="url(#bp2-f)"/>
<path class="line strong" d="M260 140H345V200" marker-end="url(#bp2-f)"/>
<line class="line strong" x1="400" y1="220" x2="430" y2="220" marker-end="url(#bp2-f)"/>
<path class="line strong" d="M485 200V140H570" marker-end="url(#bp2-f)"/>
<line class="line strong" x1="630" y1="120" x2="630" y2="80" marker-end="url(#bp2-f)"/>
</svg>

Diagrammet räcker för att se att ärendet byter bana fyra gånger. Men det säger inget om *när* det går till utvecklaren — alla ärenden? — eller att rättning och test kan ske samtidigt. Samma process i **BPMN**:

<svg class="dg" viewBox="0 0 720 430" role="img" aria-labelledby="bp3-t" xmlns="http://www.w3.org/2000/svg">
<title id="bp3-t">BPMN-diagram för ett supportärende: kunden som egen pool, IT-konsultbolaget med banorna Servicedesk och Utvecklare, en exklusiv gateway för känt fel och en parallell gateway för rättning och test</title>
<defs>
<marker id="bp3-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
<marker id="bp3-o" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10" class="line strong"/></marker>
<marker id="bp3-c" viewBox="0 0 10 10" refX="5" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><circle cx="5" cy="5" r="4" class="box"/></marker>
</defs>
<rect class="line strong" x="20" y="20" width="680" height="90"/>
<line class="line strong" x1="50" y1="20" x2="50" y2="110"/>
<text x="41" y="65" text-anchor="middle" class="title" transform="rotate(-90 41 65)">Kund</text>
<circle class="box" cx="85" cy="65" r="15"/>
<line class="line strong" x1="100" y1="65" x2="120" y2="65" marker-end="url(#bp3-f)"/>
<rect class="box" x="120" y="40" width="90" height="50" rx="10"/><text x="165" y="61" text-anchor="middle">Skicka</text><text x="165" y="79" text-anchor="middle">ärende</text>
<line class="line strong" x1="210" y1="65" x2="565" y2="65" marker-end="url(#bp3-f)"/>
<circle class="box" cx="580" cy="65" r="15"/><circle class="line strong" cx="580" cy="65" r="11"/>
<text x="580" y="38" text-anchor="middle" class="muted">svar mottaget</text>
<line class="line strong" x1="595" y1="65" x2="625" y2="65" marker-end="url(#bp3-f)"/>
<circle class="solid" cx="640" cy="65" r="15"/><circle class="box" cx="640" cy="65" r="11"/>
<rect class="line strong" x="20" y="150" width="680" height="260"/>
<line class="line strong" x1="50" y1="150" x2="50" y2="410"/>
<line class="line" x1="80" y1="150" x2="80" y2="410"/>
<line class="line" x1="50" y1="280" x2="700" y2="280"/>
<text x="41" y="280" text-anchor="middle" class="title" transform="rotate(-90 41 280)">IT-konsultbolaget</text>
<text x="70" y="215" text-anchor="middle" transform="rotate(-90 70 215)">Servicedesk</text>
<text x="70" y="345" text-anchor="middle" transform="rotate(-90 70 345)">Utvecklare</text>
<circle class="box" cx="100" cy="215" r="15"/>
<line class="line strong" x1="115" y1="215" x2="130" y2="215" marker-end="url(#bp3-f)"/>
<rect class="box" x="130" y="190" width="90" height="50" rx="10"/><text x="175" y="211" text-anchor="middle">Registrera</text><text x="175" y="229" text-anchor="middle">ärende</text>
<line class="line strong" x1="220" y1="215" x2="245" y2="215" marker-end="url(#bp3-f)"/>
<path class="box" d="M265 195L285 215L265 235L245 215Z"/>
<line class="line strong" x1="257" y1="207" x2="273" y2="223"/><line class="line strong" x1="273" y1="207" x2="257" y2="223"/>
<text x="265" y="186" text-anchor="middle" class="muted">Känt fel?</text>
<line class="line strong" x1="285" y1="215" x2="535" y2="215" marker-end="url(#bp3-f)"/><text x="300" y="208" class="muted">ja</text>
<rect class="box" x="535" y="190" width="90" height="50" rx="10"/><text x="580" y="220" text-anchor="middle">Svara kund</text>
<line class="line strong" x1="625" y1="215" x2="650" y2="215" marker-end="url(#bp3-f)"/>
<circle class="solid" cx="665" cy="215" r="15"/><circle class="box" cx="665" cy="215" r="11"/>
<line class="line strong" x1="265" y1="235" x2="265" y2="320" marker-end="url(#bp3-f)"/><text x="273" y="262" class="muted">nej</text>
<rect class="box" x="215" y="320" width="100" height="50" rx="10"/><text x="265" y="350" text-anchor="middle">Felsöka</text>
<line class="line strong" x1="315" y1="345" x2="335" y2="345" marker-end="url(#bp3-f)"/>
<path class="box" d="M355 325L375 345L355 365L335 345Z"/>
<line class="line strong" x1="355" y1="333" x2="355" y2="357"/><line class="line strong" x1="343" y1="345" x2="367" y2="345"/>
<path class="line strong" d="M355 325V306H395" marker-end="url(#bp3-f)"/>
<path class="line strong" d="M355 365V384H395" marker-end="url(#bp3-f)"/>
<rect class="box" x="395" y="288" width="100" height="36" rx="10"/><text x="445" y="311" text-anchor="middle">Rätta koden</text>
<rect class="box" x="395" y="366" width="100" height="36" rx="10"/><text x="445" y="389" text-anchor="middle">Skriv test</text>
<path class="line strong" d="M495 306H535V325" marker-end="url(#bp3-f)"/>
<path class="line strong" d="M495 384H535V365" marker-end="url(#bp3-f)"/>
<path class="box" d="M535 325L555 345L535 365L515 345Z"/>
<line class="line strong" x1="535" y1="333" x2="535" y2="357"/><line class="line strong" x1="523" y1="345" x2="547" y2="345"/>
<path class="line strong" d="M555 345H580V240" marker-end="url(#bp3-f)"/>
<path class="line dash" d="M165 90V130H100V200" marker-start="url(#bp3-c)" marker-end="url(#bp3-o)"/>
<text x="175" y="140" class="muted">felanmälan</text>
<line class="line dash" x1="580" y1="190" x2="580" y2="80" marker-start="url(#bp3-c)" marker-end="url(#bp3-o)"/>
<text x="588" y="140" class="muted">lösning</text>
</svg>

Det BPMN-versionen visar som simbanediagrammet missade:

- **Kunden är en egen pool.** Konsultbolaget styr inte vad kunden gör — de två pratar via *meddelanden* (streckade pilar).
- **Gatewayen "Känt fel?"** gör beslutet synligt. Om 80 % av ärendena går "ja"-vägen är det servicedesk som behöver mer stöd, inte utvecklarna.
- **Den parallella gatewayen** säger att rättning och test görs samtidigt, och att kunden inte får svar förrän *båda* är klara.

## När räcker ett simbanediagram — och när behövs BPMN?

| Välj simbanediagram när… | Välj BPMN när… |
|--------------------------|----------------|
| Teamet ska bli överens om nuläget, snabbt, på whiteboard | Processen ska dokumenteras så att den inte kan misstolkas |
| Publiken är kunder, chefer eller nya kollegor | Publiken är verksamhetsutvecklare eller systemutvecklare |
| Det viktiga är *vem* som gör vad | Beslut, väntan och parallella steg är det viktiga |
| Ni är i början av ett projekt | Processen ska automatiseras i ett verktyg (t.ex. en workflow-motor) |

| Vill du visa… | Välj hellre |
|---------------|-------------|
| Hur *kunden* upplever processen, inklusive känslor | [Kundresa](kundresa.md) |
| Varför något går fel, inte hur flödet ser ut | [Fem varför](fem-varfor.md) |
| Hur arbetet flödar genom teamets tavla | [Kanban](../agilt/kanban.md) |

## Vanliga misstag

- **Ett steg per bana, alltid.** Om varje ruta ligger i en ny bana är banorna för smala — kanske är det samma roll.
- **Rita idealet istället för verkligheten.** Kartlägg först hur det *faktiskt* går till, även det pinsamma. Annars hittar ni inga problem.
- **Gateway utan villkor.** En romb med två pilar ut men utan "ja"/"nej" på pilarna säger ingenting.
- **Sekvensflöde mellan pooler.** Mellan organisationer går information som meddelanden — ni styr inte varandras ordning.
- **För mycket på en gång.** Fler än 15–20 steg blir oläsligt. Dela upp i delprocesser.

## Mall att kopiera

Fyll i tabellen tillsammans innan ni ritar — då blir diagrammet nästan en avskrift.

| # | Steg (verb + objekt) | Bana (vem) | Kommer efter | Beslut? (villkor) | Väntan / meddelande? |
|---|----------------------|------------|--------------|-------------------|----------------------|
| 1 | | | — | | |
| 2 | | | 1 | | |
| 3 | | | 2 | | |

## Övning

Rita ett simbanediagram för hur er grupp lämnar in en projektuppgift: från att någon skriver klart till att läraren har satt betyg. Banor: *Student*, *Gruppen*, *Lärare*, *Lärplattformen*. Rita sedan om det i BPMN: var finns det beslut (godkänd/komplettering)? Vilka steg kan ske parallellt? Är lärplattformen en bana eller en egen pool?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Simbanediagram | Rutor och pilar i en bana per roll — enkelt, alla förstår |
| BPMN | Standard med bestämda symboler för händelser, beslut och meddelanden |
| Pool / bana | Organisation / roll inom organisationen |
| Cirklar | Händelser: start (tunn), mellan (dubbel), slut (tjock) |
| Romb | Gateway: X = en väg, + = alla vägar samtidigt |
| Heldragen / streckad pil | Inom poolen / mellan pooler |
