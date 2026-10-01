---
title: Diagram för data
description: "Linjediagram, stapeldiagram och cirkeldiagram — vilket ska du välja, vad heter delarna, och hur ser burndown och velocity ut när de ritas ärligt?"
parent: Diagram & analysverktyg
nav_order: 60
---

# Diagram för data

## Grundidén

Ett datadiagram (en *graf*) gör siffror till en bild, så att mönster syns utan att man läser varje värde. Valet av diagramtyp avgör vilket mönster som syns:

| Frågan du vill besvara | Diagram |
|------------------------|---------|
| Hur förändras något **över tid**? | **Linjediagram** |
| Hur stora är några **kategorier** jämfört med varandra? | **Stapeldiagram** — stående (kolumndiagram) eller liggande |
| Hur stor **andel av en helhet** är varje del? | **Cirkeldiagram** — men bara om delarna är få och tydligt olika |

I projekt möter ni dem hela tiden: burndown-diagram i sprinten, velocity över flera sprintar, tidrapporter och ärendestatistik på retrospektivet.

## Vad används det till?

- **Följa upp en sprint** — hinner vi? (burndown)
- **Planera nästa sprint** — hur mycket brukar vi klara? (velocity)
- **Hitta var tiden går** — vilka ärenden tar längst tid?
- **Underlag för beslut** — på en [retrospektiv](retro-och-standup.md), inför kunden eller ledningen

## Delarna och vad de heter

<svg class="dg" viewBox="0 0 720 380" role="img" aria-labelledby="dd1-t" xmlns="http://www.w3.org/2000/svg">
<title id="dd1-t">Linjediagram över supportärenden per vecka med namngivna delar: titel, y-axel, x-axel, axeletikett, skalsteg, dataserie, datapunkt, förklaring och källa</title>
<text x="200" y="40" class="title">Supportärenden per vecka</text>
<line class="line strong" x1="200" y1="70" x2="200" y2="290"/>
<line class="line strong" x1="200" y1="290" x2="500" y2="290"/>
<path class="line" d="M194 290H200M194 235H200M194 180H200M194 125H200M194 70H200"/>
<text x="190" y="294" text-anchor="end" class="muted">0</text>
<text x="190" y="239" text-anchor="end" class="muted">10</text>
<text x="190" y="184" text-anchor="end" class="muted">20</text>
<text x="190" y="129" text-anchor="end" class="muted">30</text>
<text x="190" y="74" text-anchor="end" class="muted">40</text>
<path class="line" d="M220 290V296M274 290V296M328 290V296M382 290V296M436 290V296M490 290V296"/>
<text x="220" y="310" text-anchor="middle" class="muted">v36</text>
<text x="274" y="310" text-anchor="middle" class="muted">v37</text>
<text x="328" y="310" text-anchor="middle" class="muted">v38</text>
<text x="382" y="310" text-anchor="middle" class="muted">v39</text>
<text x="436" y="310" text-anchor="middle" class="muted">v40</text>
<text x="490" y="310" text-anchor="middle" class="muted">v41</text>
<text x="160" y="180" text-anchor="middle" class="muted" transform="rotate(-90 160 180)">Antal ärenden</text>
<text x="350" y="334" text-anchor="middle" class="muted">Vecka</text>
<path class="line strong" d="M220 224L274 191L328 207.5L382 169L436 125L490 147"/>
<path class="line dash" d="M220 180L274 196.5L328 185.5L382 213L436 224L490 235"/>
<circle class="solid" cx="220" cy="224" r="4"/><circle class="solid" cx="274" cy="191" r="4"/><circle class="solid" cx="328" cy="207.5" r="4"/><circle class="solid" cx="382" cy="169" r="4"/><circle class="solid" cx="436" cy="125" r="4"/><circle class="solid" cx="490" cy="147" r="4"/>
<circle class="box" cx="220" cy="180" r="4"/><circle class="box" cx="274" cy="196.5" r="4"/><circle class="box" cx="328" cy="185.5" r="4"/><circle class="box" cx="382" cy="213" r="4"/><circle class="box" cx="436" cy="224" r="4"/><circle class="box" cx="490" cy="235" r="4"/>
<rect class="box" x="340" y="78" width="150" height="28" rx="3"/>
<line class="line strong" x1="350" y1="92" x2="372" y2="92"/><text x="378" y="97">Bugg</text>
<line class="line dash" x1="418" y1="92" x2="440" y2="92"/><text x="446" y="97">Fråga</text>
<text x="200" y="362" class="muted">Källa: ärendesystemet, vecka 36–41 2026</text>
<line class="leader" x1="66" y1="100" x2="198" y2="100"/><text x="20" y="104" class="part">Y-axel</text>
<line class="leader" x1="100" y1="180" x2="146" y2="180"/><text x="20" y="184" class="part">Axeletikett</text>
<line class="leader" x1="82" y1="235" x2="172" y2="235"/><text x="20" y="239" class="part">Skalsteg</text>
<line class="leader" x1="395" y1="40" x2="555" y2="40"/><text x="560" y="44" class="part">Titel</text>
<line class="leader" x1="490" y1="92" x2="555" y2="92"/><text x="560" y="96" class="part">Förklaring (legend)</text>
<line class="leader" x1="463" y1="136" x2="555" y2="150"/><text x="560" y="154" class="part">Dataserie</text>
<line class="leader" x1="494" y1="150" x2="555" y2="180"/><text x="560" y="184" class="part">Datapunkt</text>
<line class="leader" x1="500" y1="290" x2="555" y2="284"/><text x="560" y="288" class="part">X-axel</text>
<line class="leader" x1="455" y1="358" x2="555" y2="358"/><text x="560" y="362" class="part">Källa</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Titel** | Fet text överst | Vad diagrammet visar — gärna som ett påstående: "Buggarna ökar sedan v38" |
| **X-axel** | Vågrät linje längst ner | Oftast tiden eller kategorierna |
| **Y-axel** | Lodrät linje till vänster | Oftast det som mäts — antal, timmar, poäng |
| **Axeletikett** | Text längs axeln | Vad axeln mäter, och i vilken **enhet** |
| **Skalsteg** | Siffror med jämna mellanrum | Axelns indelning. Jämna steg (0, 10, 20…) och — för staplar — alltid från noll |
| **Dataserie** | En linje eller en grupp staplar | Alla värden som hör ihop, t.ex. "Bugg" |
| **Datapunkt** | En prick (eller en stapel) | Ett enskilt värde: vecka 40 kom det 30 buggar |
| **Förklaring** (legend) | Liten ruta med symboler | Vilken linje/färg som är vilken serie. Behövs inte om det bara finns en serie |
| **Källa** | Liten text under diagrammet | Var siffrorna kommer ifrån och vilken period. Utan källa går diagrammet inte att granska |

## Exempel — fyra diagram ur ett projekt

### Burndown — linjediagram

Ett **burndown-diagram** visar hur mycket arbete som är kvar i sprinten, dag för dag. Den streckade linjen är den **ideala** takten — om teamet blev klart med lika mycket varje dag. Den heldragna är den **faktiska**.

<svg class="dg" viewBox="0 0 720 370" role="img" aria-labelledby="dd2-t" xmlns="http://www.w3.org/2000/svg">
<title id="dd2-t">Burndown-diagram för sprint 3: ideal linje från 40 till 0 story points över tio dagar, och faktisk linje som ligger kvar på 40 de första dagarna och slutar på 4</title>
<text x="80" y="30" class="title">Burndown — sprint 3</text>
<line class="line strong" x1="80" y1="50" x2="80" y2="290"/>
<line class="line strong" x1="80" y1="290" x2="640" y2="290"/>
<path class="line" d="M74 290H80M74 230H80M74 170H80M74 110H80M74 50H80"/>
<text x="70" y="294" text-anchor="end" class="muted">0</text>
<text x="70" y="234" text-anchor="end" class="muted">10</text>
<text x="70" y="174" text-anchor="end" class="muted">20</text>
<text x="70" y="114" text-anchor="end" class="muted">30</text>
<text x="70" y="54" text-anchor="end" class="muted">40</text>
<path class="line" d="M80 290V296M136 290V296M192 290V296M248 290V296M304 290V296M360 290V296M416 290V296M472 290V296M528 290V296M584 290V296M640 290V296"/>
<text x="80" y="310" text-anchor="middle" class="muted">0</text>
<text x="136" y="310" text-anchor="middle" class="muted">1</text>
<text x="192" y="310" text-anchor="middle" class="muted">2</text>
<text x="248" y="310" text-anchor="middle" class="muted">3</text>
<text x="304" y="310" text-anchor="middle" class="muted">4</text>
<text x="360" y="310" text-anchor="middle" class="muted">5</text>
<text x="416" y="310" text-anchor="middle" class="muted">6</text>
<text x="472" y="310" text-anchor="middle" class="muted">7</text>
<text x="528" y="310" text-anchor="middle" class="muted">8</text>
<text x="584" y="310" text-anchor="middle" class="muted">9</text>
<text x="640" y="310" text-anchor="middle" class="muted">10</text>
<text x="30" y="170" text-anchor="middle" class="muted" transform="rotate(-90 30 170)">Kvarvarande story points</text>
<text x="360" y="334" text-anchor="middle" class="muted">Dag i sprinten</text>
<line class="line dash" x1="80" y1="50" x2="640" y2="290"/>
<path class="line strong" d="M80 50L136 50L192 68L248 80L304 80L360 110L416 134L472 170L528 200L584 236L640 266"/>
<circle class="solid" cx="80" cy="50" r="4"/><circle class="solid" cx="136" cy="50" r="4"/><circle class="solid" cx="192" cy="68" r="4"/><circle class="solid" cx="248" cy="80" r="4"/><circle class="solid" cx="304" cy="80" r="4"/><circle class="solid" cx="360" cy="110" r="4"/><circle class="solid" cx="416" cy="134" r="4"/><circle class="solid" cx="472" cy="170" r="4"/><circle class="solid" cx="528" cy="200" r="4"/><circle class="solid" cx="584" cy="236" r="4"/><circle class="solid" cx="640" cy="266" r="4"/>
<rect class="box" x="455" y="40" width="180" height="28" rx="3"/>
<line class="line dash" x1="465" y1="54" x2="487" y2="54"/><text x="493" y="59">Ideal</text>
<line class="line strong" x1="540" y1="54" x2="562" y2="54"/><text x="568" y="59">Faktisk</text>
<text x="80" y="356" class="muted">Källa: teamets sprinttavla, sprint 3</text>
</svg>

Så läser teamet det: den faktiska linjen ligger **över** den ideala hela sprinten — de ligger efter. Dag 1 hände ingenting (40 → 40) och dag 3–4 stod det still igen (35 → 35). På retron visade det sig att båda gångerna väntade de på svar från kunden. Sprinten slutade med 4 poäng kvar — en user story som inte blev klar.

### Velocity per sprint — stående staplar

**Velocity** är hur många story points teamet blev klara med per sprint. Sprintarna är *kategorier* (inte en jämn tidslinje med mätvärden däremellan), därför stående staplar, ett så kallat kolumndiagram.

<svg class="dg" viewBox="0 0 720 315" role="img" aria-labelledby="dd3-t" xmlns="http://www.w3.org/2000/svg">
<title id="dd3-t">Kolumndiagram över velocity per sprint: sprint 1 18 poäng, sprint 2 24, sprint 3 21, sprint 4 27, sprint 5 26 och sprint 6 29</title>
<text x="80" y="30" class="title">Velocity per sprint</text>
<line class="line strong" x1="80" y1="50" x2="80" y2="250"/>
<line class="line strong" x1="80" y1="250" x2="640" y2="250"/>
<path class="line" d="M74 250H80M74 200H80M74 150H80M74 100H80M74 50H80"/>
<text x="70" y="254" text-anchor="end" class="muted">0</text>
<text x="70" y="204" text-anchor="end" class="muted">10</text>
<text x="70" y="154" text-anchor="end" class="muted">20</text>
<text x="70" y="104" text-anchor="end" class="muted">30</text>
<text x="70" y="54" text-anchor="end" class="muted">40</text>
<text x="30" y="150" text-anchor="middle" class="muted" transform="rotate(-90 30 150)">Story points</text>
<rect class="hl" x="102" y="160" width="50" height="90"/><text x="127" y="154" text-anchor="middle">18</text>
<rect class="hl" x="195" y="130" width="50" height="120"/><text x="220" y="124" text-anchor="middle">24</text>
<rect class="hl" x="288" y="145" width="50" height="105"/><text x="313" y="139" text-anchor="middle">21</text>
<rect class="hl" x="382" y="115" width="50" height="135"/><text x="407" y="109" text-anchor="middle">27</text>
<rect class="hl" x="475" y="120" width="50" height="130"/><text x="500" y="114" text-anchor="middle">26</text>
<rect class="hl" x="568" y="105" width="50" height="145"/><text x="593" y="99" text-anchor="middle">29</text>
<text x="127" y="268" text-anchor="middle" class="muted">Sprint 1</text>
<text x="220" y="268" text-anchor="middle" class="muted">Sprint 2</text>
<text x="313" y="268" text-anchor="middle" class="muted">Sprint 3</text>
<text x="407" y="268" text-anchor="middle" class="muted">Sprint 4</text>
<text x="500" y="268" text-anchor="middle" class="muted">Sprint 5</text>
<text x="593" y="268" text-anchor="middle" class="muted">Sprint 6</text>
<text x="80" y="300" class="muted">Källa: sprintrapporter, sprint 1–6</text>
</svg>

Snittet är 24 poäng per sprint (145 / 6). Det är ett bättre underlag för nästa sprintplanering än den bästa sprinten (29) — och det är *teamets eget* mått. Velocity ska inte jämföras mellan team: ett annat team räknar story points på ett annat sätt. Se [Backlog och sprint](../begrepp/backlog-och-sprint.md).

### Tid per ärendetyp — liggande staplar

När kategorierna har långa namn, eller när det är många av dem, blir **liggande staplar** lättare att läsa — texten får plats och ögat jämför längder snabbt. Sortera från störst till minst.

<svg class="dg" viewBox="0 0 720 360" role="img" aria-labelledby="dd4-t" xmlns="http://www.w3.org/2000/svg">
<title id="dd4-t">Liggande stapeldiagram över median timmar per ärendetyp: ny funktion 16, integration 11, bugg 6, behörighet 3 och fråga 1</title>
<text x="150" y="30" class="title">Tid per ärendetyp</text>
<line class="line strong" x1="150" y1="50" x2="150" y2="276"/>
<line class="line strong" x1="150" y1="276" x2="630" y2="276"/>
<path class="line" d="M150 276V282M270 276V282M390 276V282M510 276V282M630 276V282"/>
<text x="150" y="296" text-anchor="middle" class="muted">0</text>
<text x="270" y="296" text-anchor="middle" class="muted">5</text>
<text x="390" y="296" text-anchor="middle" class="muted">10</text>
<text x="510" y="296" text-anchor="middle" class="muted">15</text>
<text x="630" y="296" text-anchor="middle" class="muted">20</text>
<text x="390" y="320" text-anchor="middle" class="muted">Timmar per ärende (median)</text>
<text x="140" y="75" text-anchor="end">Ny funktion</text><rect class="q2" x="150" y="56" width="384" height="28"/><text x="542" y="75">16 h</text>
<text x="140" y="119" text-anchor="end">Integration</text><rect class="q2" x="150" y="100" width="264" height="28"/><text x="422" y="119">11 h</text>
<text x="140" y="163" text-anchor="end">Bugg</text><rect class="q2" x="150" y="144" width="144" height="28"/><text x="302" y="163">6 h</text>
<text x="140" y="207" text-anchor="end">Behörighet</text><rect class="q2" x="150" y="188" width="72" height="28"/><text x="230" y="207">3 h</text>
<text x="140" y="251" text-anchor="end">Fråga</text><rect class="q2" x="150" y="232" width="24" height="28"/><text x="182" y="251">1 h</text>
<text x="150" y="346" class="muted">Källa: tidrapporter, 120 ärenden, vecka 30–39</text>
</svg>

Medianen används istället för medelvärdet, eftersom ett enda jätteärende annars drar upp hela stapeln. Skriv det i axeletiketten — annars vet läsaren inte vad hen tittar på.

### Fördelning av ärenden — cirkeldiagram (och varför det sällan är rätt val)

Ett cirkeldiagram visar delar av en helhet, där hela cirkeln är 100 %. Det fungerar bara när delarna är **få** (2–4) och **tydligt olika** stora. Ögat är dåligt på att jämföra vinklar och ytor, mycket bättre på att jämföra längder.

<svg class="dg" viewBox="0 0 720 315" role="img" aria-labelledby="dd5-t" xmlns="http://www.w3.org/2000/svg">
<title id="dd5-t">Två cirkeldiagram: till vänster tre tydligt olika delar, bugg 60 procent, fråga 30 och ny funktion 10, som är lätta att läsa; till höger sex nästan lika delar mellan 15 och 19 procent som är omöjliga att jämföra</title>
<text x="180" y="24" text-anchor="middle" class="title">Få delar av en helhet</text>
<path class="q2" d="M180 170L180 70A100 100 0 1 1 121.2 250.9Z"/>
<path class="q4" d="M180 170L121.2 250.9A100 100 0 0 1 121.2 89.1Z"/>
<path class="q3" d="M180 170L121.2 89.1A100 100 0 0 1 180 70Z"/>
<text x="232" y="182" text-anchor="middle">Bugg</text><text x="232" y="200" text-anchor="middle">60 %</text>
<text x="128" y="165" text-anchor="middle">Fråga</text><text x="128" y="183" text-anchor="middle">30 %</text>
<line class="line" x1="152" y1="78" x2="160" y2="62"/><text x="172" y="56" text-anchor="end" class="muted">Ny funktion 10 %</text>
<text x="180" y="298" text-anchor="middle" class="muted">Bugg är störst — syns direkt</text>
<text x="530" y="24" text-anchor="middle" class="title">Många nästan lika delar</text>
<path class="q1" d="M530 170L530 70A100 100 0 0 1 623 133.2Z"/>
<path class="q2" d="M530 170L623 133.2A100 100 0 0 1 602.9 238.5Z"/>
<path class="q3" d="M530 170L602.9 238.5A100 100 0 0 1 505.1 266.9Z"/>
<path class="q4" d="M530 170L505.1 266.9A100 100 0 0 1 434.9 200.9Z"/>
<path class="hl" d="M530 170L434.9 200.9A100 100 0 0 1 449.1 111.2Z"/>
<path class="box" d="M530 170L449.1 111.2A100 100 0 0 1 530 70Z"/>
<text x="567" y="121" text-anchor="middle">A</text>
<text x="594" y="187" text-anchor="middle">B</text>
<text x="548" y="237" text-anchor="middle">C</text>
<text x="486" y="222" text-anchor="middle">D</text>
<text x="466" y="165" text-anchor="middle">E</text>
<text x="500" y="117" text-anchor="middle">F</text>
<text x="530" y="298" text-anchor="middle" class="muted">Vilken är störst? Går inte att se</text>
</svg>

Till höger är A 19 %, B 18 %, C 17 %, D 16 %, E och F 15 % var. Det går inte att se — och därför ska de här siffrorna visas som liggande staplar, eller helt enkelt som en tabell.

**Ärlig varning:** använd *inte* cirkeldiagram när

- det finns fler än 4–5 delar
- delarna är ungefär lika stora
- du vill jämföra två perioder (två cirklar bredvid varandra är nästan omöjliga att jämföra)
- delarna inte blir 100 % tillsammans — t.ex. när ett ärende kan ha flera typer
- någon föreslår 3D-effekt. En lutad cirkel gör de främre bitarna större än de är.

Är du osäker: välj ett stapeldiagram. Det är nästan aldrig fel.

## När ska du välja vilket?

| Välj… | När… | Exempel i projekt |
|-------|------|-------------------|
| **Linjediagram** | Värdena följer på varandra i tid och du vill se trenden | Burndown, öppna buggar per vecka, svarstid över tid |
| **Stående staplar** (kolumner) | Få kategorier eller tidsperioder som du jämför | Velocity per sprint, ärenden per månad |
| **Liggande staplar** | Många kategorier, långa namn, eller en topplista | Tid per ärendetyp, fel per modul |
| **Cirkeldiagram** | 2–4 delar av en helhet, tydligt olika stora | Andel buggar av alla ärenden |
| **Tabell** | Läsaren behöver de exakta värdena | Tidrapport, budget |
| Något annat | Du vill visa hur grupper överlappar → [Venndiagram](venndiagram.md) — eller prioritera idéer → [Prioriteringsmatriser](prioriteringsmatriser.md) | — |

## Vanliga misstag

- **Y-axeln börjar inte på noll** i ett stapeldiagram. En stapel på 21 ser dubbelt så hög ut som en på 18 om axeln börjar på 15. (I linjediagram kan det vara okej att zooma — men skriv ut skalan tydligt.)
- **Ojämna skalsteg.** 0, 10, 20, 50, 100 på samma axel förvränger allt. Välj jämna steg.
- **Ingen enhet.** "Tid" — timmar, dagar, minuter? Skriv enheten i axeletiketten.
- **Linjediagram för kategorier.** En linje mellan "Bugg" och "Fråga" påstår att det finns något däremellan. Kategorier ska ha staplar.
- **För många serier.** Fler än 3–4 linjer i samma diagram blir spagetti. Dela upp.
- **Ingen källa.** Om ingen kan se var siffrorna kommer ifrån går det inte att lita på dem.
- **Färg som enda skillnad.** Alla ser inte färg på samma sätt — skilj också med streckad/heldragen linje eller direkta etiketter, som i exemplen ovan.

## Mall att kopiera

Fyll i innan du ritar — det tvingar fram rätt diagramtyp:

| Fråga | Ditt svar |
|-------|-----------|
| Vad vill jag att läsaren ska förstå? (blir titeln) | |
| Tid, kategorier eller andelar? (blir diagramtypen) | |
| Vad är x-axeln, och vilken enhet? | |
| Vad är y-axeln, och vilken enhet? Börjar den på 0? | |
| Hur många serier? Behövs en förklaring? | |
| Var kommer siffrorna ifrån, och vilken period? (blir källan) | |

## Övning

Ta fram siffrorna från ert senaste projekt eller er senaste sprint — antal klara uppgifter per person, per dag eller per typ. Rita samma siffror två gånger: en gång som cirkeldiagram och en gång som stapeldiagram. Visa båda för någon utanför gruppen och fråga *"vilken del är störst?"*. Vilket diagram svarade de snabbast på?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Linjediagram | Förändring över tid — burndown |
| Stapeldiagram, stående | Jämför få kategorier — velocity |
| Stapeldiagram, liggande | Många kategorier eller långa namn — sortera |
| Cirkeldiagram | Andelar av en helhet — bara 2–4 tydligt olika delar |
| Axeletikett | Vad axeln mäter + enhet |
| Skalsteg | Jämna steg, staplar från noll |
| Källa | Var siffrorna kommer ifrån |
