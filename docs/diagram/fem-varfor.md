---
title: 5 varför
description: "5 varför är en enkel rotorsaksanalys: fråga 'varför?' om och om igen tills ni hittar orsaken som går att åtgärda. Här finns också fiskbensdiagrammet för när orsakerna är flera."
parent: Diagram & analysverktyg
nav_order: 110
---

# 5 varför

## Grundidén

När något har gått fel är det lätt att laga symptomet och gå vidare. **5 varför** (*5 Whys*) tvingar teamet att gräva djupare: ni skriver ner problemet och frågar *varför hände det?* Svaret blir nästa fråga: *och varför hände det?* Efter ungefär fem varv brukar ni ha nått **rotorsaken** — det som faktiskt måste ändras för att problemet inte ska komma tillbaka.

Siffran fem är en tumregel, inte en lag. Ibland räcker tre varv, ibland behövs sju. Ni är framme när svaret är något ni kan **göra något åt**.

## Vad används det till?

- **Efter en incident** — en deploy som gick fel, en server som låg nere
- **I en retrospektiv** — när samma problem dyker upp sprint efter sprint
- **Vid buggar som kommer tillbaka** — laga orsaken, inte bara buggen
- **Att undvika skuldbeläggning** — frågan är *varför processen tillät felet*, inte *vem som gjorde det*

## Delarna och vad de heter

<svg class="dg" viewBox="0 0 720 450" role="img" aria-labelledby="fv1-t" xmlns="http://www.w3.org/2000/svg">
<title id="fv1-t">5 varför som en kedja med namngivna delar: problemformulering, följdfrågan varför, varför-kedjan med fem svar, rotorsak och åtgärder</title>
<defs>
<marker id="fv1-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<rect class="q1" x="60" y="20" width="400" height="36" rx="4"/><text x="260" y="43" text-anchor="middle" class="title">Problemformulering: vad hände?</text>
<rect class="box" x="60" y="74" width="400" height="36" rx="4"/><text x="260" y="97" text-anchor="middle">Varför 1: svar på första frågan</text>
<rect class="box" x="60" y="128" width="400" height="36" rx="4"/><text x="260" y="151" text-anchor="middle">Varför 2: varför hände svar 1?</text>
<rect class="box" x="60" y="182" width="400" height="36" rx="4"/><text x="260" y="205" text-anchor="middle">Varför 3: varför hände svar 2?</text>
<rect class="box" x="60" y="236" width="400" height="36" rx="4"/><text x="260" y="259" text-anchor="middle">Varför 4: varför hände svar 3?</text>
<rect class="box" x="60" y="290" width="400" height="36" rx="4"/><text x="260" y="313" text-anchor="middle">Varför 5: varför hände svar 4?</text>
<rect class="hl" x="60" y="344" width="400" height="36" rx="4"/><text x="260" y="367" text-anchor="middle" class="title">Rotorsak: det som måste ändras</text>
<rect class="q4" x="60" y="398" width="400" height="36" rx="4"/><text x="260" y="421" text-anchor="middle" class="title">Åtgärd: vem gör vad, när?</text>
<line class="line strong" x1="260" y1="56" x2="260" y2="73" marker-end="url(#fv1-f)"/>
<line class="line strong" x1="260" y1="110" x2="260" y2="127" marker-end="url(#fv1-f)"/>
<line class="line strong" x1="260" y1="164" x2="260" y2="181" marker-end="url(#fv1-f)"/>
<line class="line strong" x1="260" y1="218" x2="260" y2="235" marker-end="url(#fv1-f)"/>
<line class="line strong" x1="260" y1="272" x2="260" y2="289" marker-end="url(#fv1-f)"/>
<line class="line strong" x1="260" y1="326" x2="260" y2="343" marker-end="url(#fv1-f)"/>
<line class="line strong" x1="260" y1="380" x2="260" y2="397" marker-end="url(#fv1-f)"/>
<text x="272" y="69" class="muted">varför?</text>
<text x="272" y="123" class="muted">varför?</text>
<text x="272" y="177" class="muted">varför?</text>
<text x="272" y="231" class="muted">varför?</text>
<text x="272" y="285" class="muted">varför?</text>
<path class="line strong" d="M468 74H478V326H468"/>
<line class="leader" x1="464" y1="38" x2="494" y2="38"/><text x="500" y="42" class="part">Problemformulering</text>
<line class="leader" x1="324" y1="65" x2="494" y2="68"/><text x="500" y="72" class="part">Följdfråga</text>
<line class="leader" x1="482" y1="200" x2="494" y2="200"/><text x="500" y="204" class="part">Varför-kedjan</text>
<line class="leader" x1="464" y1="362" x2="494" y2="362"/><text x="500" y="366" class="part">Rotorsak</text>
<line class="leader" x1="464" y1="416" x2="494" y2="416"/><text x="500" y="420" class="part">Åtgärder</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Problemformulering** | Översta rutan | Vad som hände, konkret och mätbart: *vad*, *när*, *hur mycket* |
| **Följdfråga** | "Varför?" mellan rutorna | Samma fråga varje gång, ställd till det senaste svaret |
| **Varför-kedjan** | Rutorna Varför 1–5 | Varje svar är orsaken till svaret ovanför. Läs den baklänges med "därför" — då ska den hänga ihop |
| **Rotorsak** (*root cause*) | Markerad ruta efter kedjan | Den djupaste orsaken som teamet själva kan ändra på |
| **Åtgärder** (*corrective actions*) | Sista rutan | Vad som ska ändras, vem som gör det och när. Ofta en ändring i *processen*, inte bara i koden |

## Exempel — deployen som misslyckades

Ett litet IT-konsultbolag deployar en ny version av en kunds bokningssystem en fredag eftermiddag. Deployen kraschar och sidan ligger nere i en timme. På måndagens retro gör teamet en 5 varför.

<svg class="dg" viewBox="0 0 720 450" role="img" aria-labelledby="fv2-t" xmlns="http://www.w3.org/2000/svg">
<title id="fv2-t">Ifylld 5 varför för en misslyckad deploy till produktion, från problemet via fem svar till rotorsaken att pipelinen inte testar migreringar mot realistisk data, och en åtgärd</title>
<defs>
<marker id="fv2-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<text x="130" y="43" text-anchor="end" class="title">Problem</text>
<text x="130" y="97" text-anchor="end" class="title">Varför 1</text>
<text x="130" y="151" text-anchor="end" class="title">Varför 2</text>
<text x="130" y="205" text-anchor="end" class="title">Varför 3</text>
<text x="130" y="259" text-anchor="end" class="title">Varför 4</text>
<text x="130" y="313" text-anchor="end" class="title">Varför 5</text>
<text x="130" y="367" text-anchor="end" class="title">Rotorsak</text>
<text x="130" y="421" text-anchor="end" class="title">Åtgärd</text>
<rect class="q1" x="140" y="20" width="560" height="36" rx="4"/><text x="155" y="43">Deployen till produktion misslyckades i fredags</text>
<rect class="box" x="140" y="74" width="560" height="36" rx="4"/><text x="155" y="97">Databasmigreringen kraschade mitt i deployen</text>
<rect class="box" x="140" y="128" width="560" height="36" rx="4"/><text x="155" y="151">Ny kolumn var NOT NULL men saknade standardvärde</text>
<rect class="box" x="140" y="182" width="560" height="36" rx="4"/><text x="155" y="205">I testmiljön var tabellen tom — felet syntes aldrig</text>
<rect class="box" x="140" y="236" width="560" height="36" rx="4"/><text x="155" y="259">Ingen testar migreringar mot realistisk data</text>
<rect class="box" x="140" y="290" width="560" height="36" rx="4"/><text x="155" y="313">Pipelinen har inget steg som kräver det</text>
<rect class="hl" x="140" y="344" width="560" height="36" rx="4"/><text x="155" y="367" class="title">Pipelinen testar inte migreringar mot riktig datamängd</text>
<rect class="q4" x="140" y="398" width="560" height="36" rx="4"/><text x="155" y="421">Kör migreringen mot en anonymiserad prod-kopia före deploy</text>
<line class="line strong" x1="660" y1="56" x2="660" y2="73" marker-end="url(#fv2-f)"/>
<line class="line strong" x1="660" y1="110" x2="660" y2="127" marker-end="url(#fv2-f)"/>
<line class="line strong" x1="660" y1="164" x2="660" y2="181" marker-end="url(#fv2-f)"/>
<line class="line strong" x1="660" y1="218" x2="660" y2="235" marker-end="url(#fv2-f)"/>
<line class="line strong" x1="660" y1="272" x2="660" y2="289" marker-end="url(#fv2-f)"/>
<line class="line strong" x1="660" y1="326" x2="660" y2="343" marker-end="url(#fv2-f)"/>
<line class="line strong" x1="660" y1="380" x2="660" y2="397" marker-end="url(#fv2-f)"/>
</svg>

Kontrollera kedjan genom att läsa den baklänges: *pipelinen har inget sådant steg* → **därför** testar ingen mot realistisk data → **därför** syntes inte felet i den tomma testmiljön → **därför** kraschade migreringen → **därför** misslyckades deployen. Det håller.

Lägg märke till vad teamet *inte* skrev: "Ali glömde standardvärdet". Det är sant, men det går inte att åtgärda — alla glömmer ibland. Det som går att åtgärda är att processen inte fångade det.

| Åtgärd | Ansvarig | Klart |
|--------|----------|-------|
| Lägg till ett pipeline-steg som kör migreringen mot en anonymiserad kopia av produktionsdatabasen | Sara | Sprint 7 |
| Lägg till "nya kolumner har standardvärde eller tillåter NULL" i checklistan för kodgranskning | Ali | Nästa vecka |
| Ingen deploy till produktion efter kl 15 på fredagar | Hela teamet | Direkt |

> Använd **anonymiserad** data i testmiljön — riktiga kunduppgifter hör inte hemma där.

## Fiskbensdiagrammet — när orsakerna är flera

5 varför följer **en** kedja. Ibland har ett problem flera orsaker som samverkar, och då riskerar ni att bara hitta en av dem. Då passar ett **fiskbensdiagram** (även kallat **Ishikawadiagram**, efter Kaoru Ishikawa) bättre. Problemet sitter i huvudet, och varje ben är en kategori av möjliga orsaker.

<svg class="dg" viewBox="0 0 720 310" role="img" aria-labelledby="fv3-t" xmlns="http://www.w3.org/2000/svg">
<title id="fv3-t">Fiskbensdiagram med namngivna delar: huvud med problemet, ryggrad, ben för kategorierna människor, metod, verktyg och miljö, samt en orsak på varje ben</title>
<defs>
<marker id="fv3-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<line class="line strong" x1="40" y1="160" x2="563" y2="160" marker-end="url(#fv3-f)"/>
<rect class="q1" x="565" y="130" width="140" height="60" rx="4"/>
<text x="635" y="155" text-anchor="middle" class="title">Deployen</text>
<text x="635" y="175" text-anchor="middle" class="title">misslyckades</text>
<line class="line strong" x1="110" y1="50" x2="190" y2="160"/>
<line class="line strong" x1="300" y1="50" x2="380" y2="160"/>
<line class="line strong" x1="110" y1="270" x2="190" y2="160"/>
<line class="line strong" x1="300" y1="270" x2="380" y2="160"/>
<text x="110" y="40" text-anchor="middle" class="title">Människor</text>
<text x="300" y="40" text-anchor="middle" class="title">Metod</text>
<text x="110" y="292" text-anchor="middle" class="title">Verktyg</text>
<text x="300" y="292" text-anchor="middle" class="title">Miljö</text>
<line class="line" x1="20" y1="100" x2="146" y2="100"/><text x="130" y="95" text-anchor="end" class="muted">Stress före helg</text>
<line class="line" x1="210" y1="100" x2="336" y2="100"/><text x="320" y="95" text-anchor="end" class="muted">Ingen checklista</text>
<line class="line" x1="25" y1="220" x2="146" y2="220"/><text x="144" y="215" text-anchor="end" class="muted">Pipeline utan test</text>
<line class="line" x1="230" y1="220" x2="336" y2="220"/><text x="334" y="215" text-anchor="end" class="muted">Tom testdatabas</text>
<text x="635" y="110" text-anchor="middle" class="part">Huvud (problemet)</text>
<line class="leader" x1="635" y1="116" x2="635" y2="130"/>
<line class="leader" x1="317" y1="70" x2="414" y2="58"/><text x="420" y="62" class="part">Ben (kategori)</text>
<line class="leader" x1="470" y1="163" x2="470" y2="200"/><text x="470" y="212" class="part">Ryggrad</text>
<line class="leader" x1="290" y1="223" x2="414" y2="246"/><text x="420" y="250" class="part">Orsak</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Huvud** | Ruta längst till höger | Problemet — samma problemformulering som i 5 varför |
| **Ryggrad** | Vågrät pil mot huvudet | Binder ihop alla orsaker till problemet |
| **Ben** | Sneda linjer från ryggraden | En **kategori** av orsaker. Vanliga i IT: Människor, Metod, Verktyg, Miljö (ibland även Mätning och Material) |
| **Orsak** | Kort linje på ett ben | En möjlig orsak inom kategorin. Den viktigaste kan ni sedan gräva i med 5 varför |

De två verktygen fungerar bra ihop: fiskbenet ger **bredden** (alla tänkbara orsaker), 5 varför ger **djupet** (varför just den orsaken uppstod).

## Mall att kopiera

```markdown
## 5 varför: <kort rubrik>

**Problemformulering:** <Vad hände? När? Hur stor blev effekten?>

1. **Varför?** <svar>
2. **Varför?** <varför hände svar 1?>
3. **Varför?** <varför hände svar 2?>
4. **Varför?** <varför hände svar 3?>
5. **Varför?** <varför hände svar 4?>

**Sammanfattning av rotorsaken:** <den djupaste orsaken som vi själva kan ändra på>

### Åtgärder

| Åtgärd | Ansvarig | Klart senast |
|--------|----------|--------------|
|        |          |              |
```

## När ska du välja 5 varför?

| Välj 5 varför när… | Välj något annat när… |
|--------------------|-----------------------|
| Problemet är tydligt avgränsat och har hänt | Orsakerna verkar vara många och samverka → fiskbensdiagram (ovan) |
| Ni vill komma förbi symptomet till något ni kan ändra | Ni vill se läget framåt, inte förklara något som hänt → [SWOT](swot.md) |
| Ni har en retro där samma problem återkommer | Ni vill samla idéer brett utan att leta orsak → [tankekarta](tankekarta.md) |
| | Ni har hittat åtgärderna och vill göra dem till tydliga mål → [SMART-mål](smart-mal.md) |

## Vanliga misstag

- **Att stanna vid en person.** "För att Ali glömde" är aldrig en rotorsak. Fråga varför processen lät det hända.
- **Att hoppa i kedjan.** Varje svar måste vara orsaken till svaret precis ovanför. Läs baklänges med "därför" och kontrollera.
- **Att gissa.** Svaren ska bygga på det ni faktiskt vet — loggar, commits, tidslinjen. Skriv "vet inte, ta reda på" hellre än att hitta på.
- **Åtgärder utan ägare.** "Vi ska testa mer" blir aldrig av. Skriv vem och när.

## Övning

Tänk på ett problem från ett projekt ni gjort — en missad deadline, en bugg i en inlämning, ett möte som inte ledde någonstans. Skriv en problemformulering med *vad*, *när* och *hur mycket*, och gör fem varv. Läs kedjan baklänges med "därför". Håller den? Skriv sedan en åtgärd med ansvarig och datum.

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| 5 varför | Fråga "varför?" upprepade gånger tills ni når rotorsaken |
| Problemformulering | Konkret: vad, när, hur mycket |
| Rotorsak | Den djupaste orsaken som går att åtgärda |
| Åtgärder | Vem gör vad, när — oftast en ändring i processen |
| Fiskbensdiagram (Ishikawa) | Alternativ när orsakerna är flera: huvud = problem, ryggrad, ben = kategorier |
