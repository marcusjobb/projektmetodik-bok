---
title: Roadmap och tidslinje
description: "Tidslinje, roadmap och Gantt-schema visar alla tre hur ett projekt ska röra sig framåt i tiden — men med olika mycket detalj och olika mycket säkerhet."
parent: Diagram & analysverktyg
nav_order: 40
---

# Roadmap och tidslinje

## Grundidén

Tre diagram svarar på frågan *"när händer vad?"* — med olika upplösning:

- **Tidslinje** — en linje med viktiga datum på. Bara *när*, inte *vad som görs däremellan*.
- **Gantt-schema** — en stapel per aktivitet längs en tidsaxel, med beroenden mellan staplarna. Mycket detalj: vem väntar på vem, och vad händer om något blir sent?
- **Roadmap** — en grov bild av vad som ska byggas i vilken ordning. Antingen med datum, eller i varianten **Nu / Nästa / Senare** utan datum alls.

Ju längre fram i tiden, desto mindre vet man. Det är den viktigaste skillnaden mellan diagrammen: hur mycket säkerhet de *låtsas* ha.

## Vad används det till?

- **Kommunicera med beställaren** — "när får vi se något?"
- **Hitta beroenden** — vad kan inte börja förrän något annat är klart?
- **Se konsekvensen av en försening** — flyttas slutdatumet, eller finns det marginal?
- **Prioritera** — vad gör vi nu, och vad får vänta?

## Delarna och vad de heter

Gantt-schemat har flest delar, så det är det som är annoterat här. En tidslinje är i princip bara tidsaxeln med milstolpar.

<svg class="dg" viewBox="0 0 720 280" role="img" aria-labelledby="rm1-t" xmlns="http://www.w3.org/2000/svg">
<title id="rm1-t">Gantt-schema för en tio veckors projektkurs med namngivna delar: aktivitet, tidsaxel, stapel, beroende, kritisk linje, milstolpe och idag-linje</title>
<defs>
<marker id="rm1-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<line class="line strong" x1="180" y1="50" x2="540" y2="50"/>
<path class="line" d="M180 50V55M216 50V55M252 50V55M288 50V55M324 50V55M360 50V55M396 50V55M432 50V55M468 50V55M504 50V55M540 50V55"/>
<text x="198" y="44" text-anchor="middle" class="muted">v1</text>
<text x="234" y="44" text-anchor="middle" class="muted">v2</text>
<text x="270" y="44" text-anchor="middle" class="muted">v3</text>
<text x="306" y="44" text-anchor="middle" class="muted">v4</text>
<text x="342" y="44" text-anchor="middle" class="muted">v5</text>
<text x="378" y="44" text-anchor="middle" class="muted">v6</text>
<text x="414" y="44" text-anchor="middle" class="muted">v7</text>
<text x="450" y="44" text-anchor="middle" class="muted">v8</text>
<text x="486" y="44" text-anchor="middle" class="muted">v9</text>
<text x="522" y="44" text-anchor="middle" class="muted">v10</text>
<text x="20" y="83">Förstudie</text>
<text x="20" y="119">Design</text>
<text x="20" y="155">Utveckling</text>
<text x="20" y="191">Rapport</text>
<text x="20" y="227">Presentation</text>
<rect class="q1" x="180" y="68" width="72" height="20" rx="3"/>
<rect class="q1" x="252" y="104" width="72" height="20" rx="3"/>
<rect class="q1" x="324" y="140" width="144" height="20" rx="3"/>
<rect class="hl" x="324" y="176" width="108" height="20" rx="3"/>
<path class="solid" d="M522 210L534 222L522 234L510 222Z"/>
<path class="line strong" d="M252 78H264V104" marker-end="url(#rm1-f)"/>
<path class="line strong" d="M324 114H336V140" marker-end="url(#rm1-f)"/>
<path class="line strong" d="M468 150H522V210" marker-end="url(#rm1-f)"/>
<line class="line strong dash" x1="378" y1="50" x2="378" y2="245"/>
<line class="leader" x1="40" y1="48" x2="40" y2="68"/><text x="20" y="44" class="part">Aktivitet</text>
<line class="leader" x1="540" y1="40" x2="555" y2="40"/><text x="560" y="44" class="part">Tidsaxel</text>
<line class="leader" x1="338" y1="128" x2="555" y2="118"/><text x="560" y="122" class="part">Beroende</text>
<line class="leader" x1="440" y1="160" x2="555" y2="160"/><text x="560" y="164" class="part">Kritisk linje</text>
<line class="leader" x1="432" y1="190" x2="555" y2="194"/><text x="560" y="198" class="part">Stapel</text>
<line class="leader" x1="534" y1="222" x2="555" y2="226"/><text x="560" y="230" class="part">Milstolpe</text>
<line class="leader" x1="378" y1="245" x2="555" y2="258"/><text x="560" y="262" class="part">Idag-linje</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Aktivitet** | En rad med namn till vänster | Ett arbetspaket — tillräckligt stort för att planera, tillräckligt litet för att följa upp |
| **Tidsaxel** | Skala överst: dagar, veckor eller månader | Tiden går åt höger |
| **Stapel** | Liggande rektangel | När aktiviteten pågår — början och slut |
| **Beroende** | Pil från slutet av en stapel till början av en annan | "B kan inte börja förrän A är klar" |
| **Milstolpe** | Romb (diamant) | En tidpunkt, inte en aktivitet: en leverans, ett beslut, en deadline. Har ingen längd |
| **Idag-linje** | Lodrät streckad linje | Var ni är nu. Staplar till vänster om linjen borde vara klara |
| **Kritisk linje** | Markerade staplar (här röda) | Kedjan av beroenden där *varje* försening flyttar slutdatumet. Rapporten ligger inte på den — den kan bli en vecka sen utan att presentationen påverkas |

## Exempel — en 10-veckors projektkurs

En elevgrupp har en projektkurs på tio veckor där de bygger bokningsappen för grupprum. Skolan har bestämt **datumen**: kick-off, inlämning av projektplan, demo varannan vecka och slutredovisning. Teamet bestämmer själva **innehållet** i varje sprint.

Därför använder de två diagram. Först en **tidslinje** för det som är fast:

<svg class="dg" viewBox="0 0 720 150" role="img" aria-labelledby="rm2-t" xmlns="http://www.w3.org/2000/svg">
<title id="rm2-t">Tidslinje för en tio veckors projektkurs med kick-off vecka 1, projektplan vecka 2, sprintdemo vecka 4, 6 och 8, kodfrys vecka 9 och slutredovisning vecka 10</title>
<defs>
<marker id="rm2-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<line class="line strong" x1="40" y1="60" x2="690" y2="60" marker-end="url(#rm2-f)"/>
<text x="72" y="82" text-anchor="middle" class="muted">v1</text>
<text x="136" y="82" text-anchor="middle" class="muted">v2</text>
<text x="200" y="82" text-anchor="middle" class="muted">v3</text>
<text x="264" y="82" text-anchor="middle" class="muted">v4</text>
<text x="328" y="82" text-anchor="middle" class="muted">v5</text>
<text x="392" y="82" text-anchor="middle" class="muted">v6</text>
<text x="456" y="82" text-anchor="middle" class="muted">v7</text>
<text x="520" y="82" text-anchor="middle" class="muted">v8</text>
<text x="584" y="82" text-anchor="middle" class="muted">v9</text>
<text x="648" y="82" text-anchor="middle" class="muted">v10</text>
<path class="solid" d="M72 53L79 60L72 67L65 60Z"/><line class="line" x1="72" y1="52" x2="72" y2="40"/><text x="72" y="34" text-anchor="middle">Kick-off</text>
<path class="solid" d="M136 53L143 60L136 67L129 60Z"/><line class="line" x1="136" y1="88" x2="136" y2="106"/><text x="136" y="122" text-anchor="middle">Projektplan</text><text x="136" y="138" text-anchor="middle" class="muted">inlämnad</text>
<path class="solid" d="M264 53L271 60L264 67L257 60Z"/><line class="line" x1="264" y1="52" x2="264" y2="40"/><text x="264" y="34" text-anchor="middle">Sprint 1-demo</text>
<path class="solid" d="M392 53L399 60L392 67L385 60Z"/><line class="line" x1="392" y1="88" x2="392" y2="106"/><text x="392" y="122" text-anchor="middle">Sprint 2-demo</text>
<path class="solid" d="M520 53L527 60L520 67L513 60Z"/><line class="line" x1="520" y1="52" x2="520" y2="40"/><text x="520" y="34" text-anchor="middle">Sprint 3-demo</text>
<path class="solid" d="M584 53L591 60L584 67L577 60Z"/><line class="line" x1="584" y1="88" x2="584" y2="106"/><text x="584" y="122" text-anchor="middle">Kodfrys</text>
<path class="solid" d="M648 53L655 60L648 67L641 60Z"/><line class="line" x1="648" y1="52" x2="648" y2="40"/><text x="648" y="34" text-anchor="middle">Slutredovisning</text>
</svg>

Sedan en **roadmap i Nu / Nästa / Senare-form** för innehållet. Den har inga datum — bara ordning:

<svg class="dg" viewBox="0 0 720 290" role="img" aria-labelledby="rm3-t" xmlns="http://www.w3.org/2000/svg">
<title id="rm3-t">Roadmap i tre kolumner, Nu, Nästa och Senare, för en bokningsapp — detaljerad och säker till vänster, grov och osäker till höger</title>
<defs>
<marker id="rm3-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<rect class="hl" x="20" y="20" width="210" height="50" rx="4"/><text x="125" y="42" text-anchor="middle" class="title">Nu</text><text x="125" y="60" text-anchor="middle" class="muted">sprint 3</text>
<rect class="box" x="255" y="20" width="210" height="50" rx="4"/><text x="360" y="42" text-anchor="middle" class="title">Nästa</text><text x="360" y="60" text-anchor="middle" class="muted">sprint 4–5</text>
<rect class="box" x="490" y="20" width="210" height="50" rx="4"/><text x="595" y="42" text-anchor="middle" class="title">Senare</text><text x="595" y="60" text-anchor="middle" class="muted">om tid finns</text>
<rect class="box" x="20" y="82" width="210" height="40" rx="4"/><text x="125" y="107" text-anchor="middle">Boka rum</text>
<rect class="box" x="20" y="132" width="210" height="40" rx="4"/><text x="125" y="157" text-anchor="middle">Avboka</text>
<rect class="box" x="20" y="182" width="210" height="40" rx="4"/><text x="125" y="207" text-anchor="middle">Logga in med skolkonto</text>
<rect class="box" x="255" y="82" width="210" height="40" rx="4"/><text x="360" y="107" text-anchor="middle">Filtrera på rumsstorlek</text>
<rect class="box" x="255" y="132" width="210" height="40" rx="4"/><text x="360" y="157" text-anchor="middle">Påminnelse 15 min innan</text>
<rect class="box" x="255" y="182" width="210" height="40" rx="4"/><text x="360" y="207" text-anchor="middle">Visa lediga rum i grönt</text>
<rect class="box" x="490" y="82" width="210" height="40" rx="4"/><text x="595" y="107" text-anchor="middle">Återkommande bokning</text>
<rect class="box" x="490" y="132" width="210" height="40" rx="4"/><text x="595" y="157" text-anchor="middle">Betyg på rum</text>
<rect class="box" x="490" y="182" width="210" height="40" rx="4"/><text x="595" y="207" text-anchor="middle">Koppling till schemat</text>
<line class="line strong" x1="40" y1="245" x2="680" y2="245" marker-end="url(#rm3-f)"/>
<text x="20" y="272" class="muted">detaljerat och säkert</text>
<text x="700" y="272" text-anchor="end" class="muted">grovt och osäkert</text>
</svg>

Tillsammans svarar de på båda frågorna beställaren och läraren har: *när* får vi se något (tidslinjen), och *vad* kommer först (roadmapen). Ett detaljerat Gantt-schema över alla tio veckor hade blivit fel redan i vecka 3 — teamet vet inte i vecka 1 vad sprint 3 kommer att innehålla.

## Nu / Nästa / Senare eller datumbaserad roadmap?

| | Nu / Nästa / Senare | Datumbaserad |
|---|---------------------|--------------|
| **Säger** | I vilken ordning | Vilket datum |
| **Passar** | Agila team, produkter som utvecklas löpande | När något utanför teamet hänger på datumet: en lansering, en mässa, en lag som börjar gälla |
| **Risk** | Beställaren vill ändå ha datum — och gissar själv | Datumen uppfattas som löften, även när de var gissningar |
| **Tips** | Ju längre till höger, desto grövre punkter | Visa osäkerhet: "kvartal 3" istället för "14 september" |

## När ska du välja vilken?

| Välj… | När… |
|-------|------|
| **Tidslinje** | Det viktiga är några fasta datum — deadlines, demos, avstämningar |
| **Gantt-schema** | Det finns många beroenden, flera team eller leverantörer, och fasta datum. Vanligt i [vattenfallsprojekt](../vattenfall/vattenfallsmodellen.md), byggprojekt och upphandlingar |
| **Roadmap Nu/Nästa/Senare** | Ni jobbar agilt och innehållet ändras efter varje sprint |
| **Datumbaserad roadmap** | Ledningen eller kunden behöver planera runt era leveranser |
| Något annat | Vill ni prioritera *vad* som ska in i "Nu"? → [Prioriteringsmatriser](prioriteringsmatriser.md) |

### Gantt och agilt — går det ihop?

Inte riktigt, och det är poängen. Ett Gantt-schema förutsätter att man vet vilka aktiviteter som finns och hur lång tid de tar — innan man börjar. [Scrum](../agilt/scrum.md) bygger på motsatt antagande: att man lär sig vad som behövs medan man bygger, och planerar en sprint i taget.

Men det finns lägen där de möts:

- **Ramen kan vara fast även när innehållet är agilt.** Kursens tio veckor, med demo varannan vecka, är en tidslinje. Inuti varje sprint jobbar teamet agilt.
- **Beroenden utanför teamet.** Om ni väntar på att skolans IT ska öppna inloggningen med skolkonto är det ett beroende — det kan vara värt att rita, även i ett agilt projekt.
- **Sprintarna själva kan bli staplar** i ett Gantt-schema på hög nivå, så länge ingen försöker planera *innehållet* i sprint 4 i detalj redan nu.

## Vanliga misstag

- **Falsk precision.** Ett Gantt-schema med dagsprecision tio veckor framåt ser professionellt ut och är nästan garanterat fel. Planera detaljerat nära, grovt långt bort.
- **Glömma beroendena.** Utan pilar är ett Gantt-schema bara en färgglad lista. Det är beroendena som visar vad en försening kostar.
- **Milstolpe med längd.** "Testning" är en aktivitet (stapel). "Testning klar" är en milstolpe (romb).
- **Roadmap som löfte.** Skriv tydligt på roadmapen att den visar *nuvarande plan*. Uppdatera den efter varje sprint review.
- **Rita och aldrig uppdatera.** En plan som inte följs upp är värdelös. Flytta idag-linjen varje vecka och se vad som ligger efter.

## Mall att kopiera

**Roadmap — Nu / Nästa / Senare**

| Nu (denna sprint) | Nästa (1–2 sprintar) | Senare (kanske) |
|-------------------|----------------------|-----------------|
| | | |
| | | |
| | | |

**Aktivitetslista för Gantt-schema** — fyll i innan ni ritar:

| Aktivitet | Start (vecka) | Slut (vecka) | Beror på | Ansvarig | Kritisk? |
|-----------|---------------|--------------|----------|----------|----------|
| | | | — | | |
| | | | | | |
| **Milstolpe:** | | — | | | |

## Övning

Ta er egen kurs eller LIA-period. Rita först en tidslinje med de datum som är fasta (inlämningar, redovisningar, start och slut). Gör sedan en Nu/Nästa/Senare-roadmap för det ni ska bygga. Diskutera i gruppen: vilka punkter i "Senare" skulle ni stryka först om tiden tar slut?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Tidslinje | Viktiga datum på en linje |
| Gantt-schema | Staplar per aktivitet + beroenden + milstolpar |
| Milstolpe | En tidpunkt — romb, ingen längd |
| Kritisk linje | Kedjan där varje försening flyttar slutdatumet |
| Roadmap Nu/Nästa/Senare | Ordning utan datum — passar agilt |
| Datumbaserad roadmap | Ordning med datum — när andra planerar runt er |
