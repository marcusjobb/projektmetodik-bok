---
title: Venndiagram
description: "Ett Venndiagram visar vad två eller tre saker har gemensamt och vad som är unikt för var och en — med överlappande cirklar. Bra för jämförelser och för att hitta det som ryms i en MVP."
parent: Diagram & analysverktyg
nav_order: 70
---

# Venndiagram

## Grundidén

Ett Venndiagram ritar varje grupp av saker som en **cirkel**. Där cirklarna överlappar finns det som hör till *båda*; där de inte överlappar finns det som är unikt för en grupp. Det är ett av de snabbaste sätten att svara på frågan **"vad har de här gemensamt — och vad skiljer dem åt?"**

Diagrammet kommer från mängdläran i matematiken, och därför heter delarna som i matten: mängd, snitt och union.

## Vad används det till?

- **Jämföra två metoder, verktyg eller lösningar** — vad är gemensamt för Scrum och Kanban?
- **Hitta det gemensamma i flera önskemål** — vad vill både kunden och användarna ha?
- **Avgränsa en MVP** — det som kunden vill ha, som går att bygga och som ryms i budget
- **Förklara överlapp mellan roller** — vilka uppgifter delar Product Owner och projektledare?

## Delarna och vad de heter

<svg class="dg" viewBox="0 0 720 340" role="img" aria-labelledby="vn1-t" xmlns="http://www.w3.org/2000/svg">
<title id="vn1-t">Venndiagram med namngivna delar: universum, mängd A, mängd B, det som är unikt för A, snittet och unionen</title>
<defs>
<clipPath id="vn1-c"><circle cx="310" cy="170" r="100"/></clipPath>
</defs>
<rect class="box" x="160" y="20" width="400" height="300" rx="6"/>
<text x="174" y="44" class="title">U</text>
<circle class="hl" cx="410" cy="170" r="100" clip-path="url(#vn1-c)"/>
<circle class="line strong" cx="310" cy="170" r="100"/>
<circle class="line strong" cx="410" cy="170" r="100"/>
<text x="255" y="175" text-anchor="middle" class="title">A</text>
<text x="465" y="175" text-anchor="middle" class="title">B</text>
<text x="360" y="175" text-anchor="middle">A ∩ B</text>
<text x="130" y="60" text-anchor="end" class="part">Universum (ramen)</text>
<line class="leader" x1="136" y1="56" x2="160" y2="56"/>
<text x="130" y="110" text-anchor="end" class="part">Mängd A (cirkel)</text>
<line class="leader" x1="136" y1="106" x2="239" y2="99"/>
<text x="130" y="220" text-anchor="end" class="part">Unikt för A</text>
<line class="leader" x1="136" y1="216" x2="250" y2="210"/>
<line class="leader" x1="481" y1="99" x2="584" y2="96"/><text x="590" y="100" class="part">Mängd B (cirkel)</text>
<line class="leader" x1="360" y1="215" x2="584" y2="186"/><text x="590" y="190" class="part">Snitt (A ∩ B)</text>
<line class="leader" x1="410" y1="270" x2="584" y2="286"/><text x="590" y="290" class="part">Union (A ∪ B)</text>
<text x="590" y="306" class="muted">allt i A eller B</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Mängd** (set) | En cirkel med ett namn | En grupp saker som hör ihop — "allt Scrum innehåller" |
| **Snitt** (intersection, A ∩ B) | Ytan där cirklarna överlappar | Det som finns i *båda* mängderna — det gemensamma |
| **Unikt för en mängd** | Den del av cirkeln som inte överlappar | Det som bara finns i den ena — det som skiljer |
| **Union** (A ∪ B) | Båda cirklarna tillsammans | Allt som finns i *minst en* av mängderna |
| **Universum** (U) | En ram runt alla cirklar | Allt vi pratar om just nu — även det som inte hamnar i någon cirkel |

> Med tre cirklar får du sju ytor: tre "bara en", tre "två av tre" och en mitt där **alla tre** överlappar. Det är mitten som oftast är intressantast.

## Exempel — Scrum och Kanban

Ett team ska välja arbetssätt och vill se vad de två vanligaste agila metoderna faktiskt har gemensamt. Ramen (universum) är "agila arbetssätt".

<svg class="dg" viewBox="0 0 720 360" role="img" aria-labelledby="vn2-t" xmlns="http://www.w3.org/2000/svg">
<title id="vn2-t">Venndiagram som jämför Scrum och Kanban: sprintar, roller och ceremonier är unikt för Scrum, löpande flöde och WIP-gränser unikt för Kanban, backlog, tavla och små steg är gemensamt</title>
<defs>
<clipPath id="vn2-c"><circle cx="260" cy="190" r="150"/></clipPath>
</defs>
<rect class="box" x="20" y="20" width="680" height="330" rx="6"/>
<text x="32" y="42" class="muted">Agila arbetssätt</text>
<circle class="hl" cx="460" cy="190" r="150" clip-path="url(#vn2-c)"/>
<circle class="line strong" cx="260" cy="190" r="150"/>
<circle class="line strong" cx="460" cy="190" r="150"/>
<text x="200" y="110" text-anchor="middle" class="title">Scrum</text>
<text x="520" y="110" text-anchor="middle" class="title">Kanban</text>
<text x="195" y="150" text-anchor="middle">Sprintar</text>
<text x="195" y="180" text-anchor="middle">Roller (PO, SM)</text>
<text x="195" y="210" text-anchor="middle">Fyra ceremonier</text>
<text x="195" y="240" text-anchor="middle">Sprint backlog</text>
<text x="525" y="150" text-anchor="middle">Löpande flöde</text>
<text x="525" y="180" text-anchor="middle">WIP-gränser</text>
<text x="525" y="210" text-anchor="middle">Inga fasta roller</text>
<text x="525" y="240" text-anchor="middle">Ledtid mäts</text>
<text x="360" y="165" text-anchor="middle">Backlog</text>
<text x="360" y="195" text-anchor="middle">Tavla</text>
<text x="360" y="225" text-anchor="middle">Små steg</text>
</svg>

Mitten visar vad teamet får "på köpet" oavsett val: en backlog, en synlig tavla och vanan att leverera i små steg. Det som skiljer är **rytmen** — fasta sprintar eller ett löpande flöde. Mer om båda finns i [Scrum](../agilt/scrum.md) och [Kanban](../agilt/kanban.md).

## Exempel — tre cirklar som hittar MVP:n

En elevgrupp ska bygga en bokningsapp åt skolans grupprum. Kunden har en lång önskelista, men tiden är åtta veckor. Gruppen ritar tre cirklar: **vad kunden vill**, **vad vi kan bygga** och **vad som ryms i budget (tid)**. Det som hamnar i mitten blir [MVP:n](../begrepp/user-story-och-mvp.md).

<svg class="dg" viewBox="0 0 720 420" role="img" aria-labelledby="vn3-t" xmlns="http://www.w3.org/2000/svg">
<title id="vn3-t">Venndiagram med tre cirklar: kunden vill, går att bygga och ryms i budget. I mitten där alla tre överlappar ligger MVP: boka tid</title>
<defs>
<clipPath id="vn3-c1"><circle cx="290" cy="160" r="120"/></clipPath>
<clipPath id="vn3-c3"><circle cx="360" cy="280" r="120"/></clipPath>
</defs>
<g clip-path="url(#vn3-c1)"><circle class="hl" cx="430" cy="160" r="120" clip-path="url(#vn3-c3)"/></g>
<circle class="line strong" cx="290" cy="160" r="120"/>
<circle class="line strong" cx="430" cy="160" r="120"/>
<circle class="line strong" cx="360" cy="280" r="120"/>
<text x="240" y="110" text-anchor="middle" class="title">Kunden vill</text>
<text x="240" y="135" text-anchor="middle" class="muted">Chattfunktion</text>
<text x="480" y="110" text-anchor="middle" class="title">Går att bygga</text>
<text x="480" y="135" text-anchor="middle" class="muted">Mörkt läge</text>
<text x="360" y="365" text-anchor="middle" class="title">Ryms i budget</text>
<text x="360" y="385" text-anchor="middle" class="muted">Färgteman</text>
<text x="360" y="120" text-anchor="middle" class="muted">Betalning</text>
<text x="300" y="250" text-anchor="middle" class="muted">Påminnelser</text>
<text x="420" y="250" text-anchor="middle" class="muted">Statistik</text>
<text x="360" y="195" text-anchor="middle" class="title">MVP</text>
<text x="360" y="215" text-anchor="middle" class="muted">Boka tid</text>
</svg>

Läs ytorna två och två: *betalning* vill kunden ha och den går att bygga — men den ryms inte i tiden. *Påminnelser* är billigt och önskat, men gruppen vet inte hur man skickar sms. Det är bara **boka tid** som klarar alla tre villkoren. Allt utanför mitten går till backloggen inför en senare version.

## När ska du välja ett Venndiagram?

| Välj Venndiagram när… | Välj något annat när… |
|-----------------------|-----------------------|
| Du jämför 2–3 saker och vill se gemensamt/unikt | Du jämför många alternativ på flera kriterier → en tabell eller [prioriteringsmatris](prioriteringsmatriser.md) |
| Du vill hitta det som uppfyller flera villkor samtidigt (MVP) | Du vill värdera *hur viktigt* något är, inte bara *om* det ingår → [prioriteringsmatriser](prioriteringsmatriser.md) |
| Du vill visa överlapp mellan roller eller ansvar | Du vill samla och sortera många idéer fritt → [tankekarta](tankekarta.md) |
| | Du vill väga interna och externa faktorer mot varandra → [SWOT](swot.md) |

## Vanliga misstag

- **För många cirklar.** Fyra eller fler cirklar ger så många ytor att ingen kan läsa dem. Håll dig till två eller tre.
- **Cirklar som inte överlappar.** Ett Venndiagram utan överlapp visar inget — då räcker två listor.
- **Samma sak i två ytor.** Varje sak ska stå på *exakt ett* ställe. Står "Backlog" både i Scrum-delen och i mitten blir diagrammet motsägelsefullt.
- **Storleken tolkas som mängd.** Cirklarnas storlek betyder inget i ett vanligt Venndiagram. Vill du visa hur *mycket* något är — använd ett diagram för data.

## Övning

Rita ett Venndiagram med tre cirklar för ditt eget nästa projekt: *vad användarna behöver*, *vad teamet kan* och *vad som hinns med*. Placera minst två saker i varje yta. Vad hamnar i mitten — och är det tillräckligt för en första version?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Venndiagram | Överlappande cirklar som visar gemensamt och unikt |
| Mängd | En cirkel — en grupp saker |
| Snitt (∩) | Överlappet — finns i båda |
| Union (∪) | Allt i någon av cirklarna |
| Universum | Ramen — allt vi pratar om |
