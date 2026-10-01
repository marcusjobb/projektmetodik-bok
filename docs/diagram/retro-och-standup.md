---
title: Retro- och standup-tavlor
description: "Tavlor som ger retrospektiven och daily standup en fast form: Gick bra / Gick mindre bra / Lärdomar / Åtgärder, Start-Stop-Continue, och Igår / Idag / Hinder."
parent: Diagram & analysverktyg
nav_order: 130
---

# Retro- och standup-tavlor

## Grundidén

Retrospektiven och daily standup är två av de möten som ingår i Scrum — vad de är och varför de finns står i [Scrum](../agilt/scrum.md). Den här sidan handlar om **tavlan**: kolumnerna ni ritar upp på whiteboarden eller i ett digitalt verktyg, och lapparna som hamnar i dem.

En bra tavla gör två saker. Den ger alla en **likadan ingång** — samma frågor, i samma ordning — och den lämnar ett **spår** efter mötet som ni kan gå tillbaka till.

## Vad används det till?

- **Retrotavlan** — samla erfarenheter från sprinten och göra dem till åtgärder
- **Start-Stop-Continue** — en snabbare retrovariant med fokus på beteenden
- **Standup-tavlan** — se på några sekunder vad alla gör och var något har fastnat
- **Uppföljning** — åtgärderna från förra retron är det första ni tittar på nästa gång

## Delarna och vad de heter — retrotavlan

<svg class="dg" viewBox="0 0 720 315" role="img" aria-labelledby="rs1-t" xmlns="http://www.w3.org/2000/svg">
<title id="rs1-t">Retrotavla med namngivna delar: rubrik, kolumnrubrik, kolumn, lapp och åtgärd med ägare. Kolumnerna är gick bra, gick mindre bra, lärdomar och åtgärder</title>
<text x="40" y="28" class="part">Rubrik (sprint/period)</text>
<line class="leader" x1="80" y1="33" x2="80" y2="50"/>
<text x="575" y="28" class="part">Kolumnrubrik</text>
<line class="leader" x1="617" y1="33" x2="617" y2="95"/>
<rect class="box" x="20" y="50" width="678" height="32" rx="4"/>
<text x="359" y="71" text-anchor="middle" class="title">Retro — Sprint 3, bokningsappen</text>
<rect class="box" x="20" y="127" width="162" height="143"/>
<rect class="box" x="192" y="127" width="162" height="143"/>
<rect class="box" x="364" y="127" width="162" height="143"/>
<rect class="box" x="536" y="127" width="162" height="143"/>
<rect class="q4" x="20" y="95" width="162" height="32" rx="4"/><text x="101" y="116" text-anchor="middle" class="title">Gick bra</text>
<rect class="q1" x="192" y="95" width="162" height="32" rx="4"/><text x="273" y="116" text-anchor="middle" class="title">Gick mindre bra</text>
<rect class="q2" x="364" y="95" width="162" height="32" rx="4"/><text x="445" y="116" text-anchor="middle" class="title">Lärdomar</text>
<rect class="q3" x="536" y="95" width="162" height="32" rx="4"/><text x="617" y="116" text-anchor="middle" class="title">Åtgärder</text>
<rect class="q4" x="30" y="140" width="142" height="44" rx="3"/><text x="101" y="158" text-anchor="middle" class="muted">Demon fungerade</text><text x="101" y="175" text-anchor="middle" class="muted">på första försöket</text>
<rect class="q4" x="30" y="194" width="142" height="44" rx="3"/><text x="101" y="212" text-anchor="middle" class="muted">Bra parprogrammering</text><text x="101" y="229" text-anchor="middle" class="muted">på inloggningen</text>
<rect class="q1" x="202" y="140" width="142" height="44" rx="3"/><text x="273" y="158" text-anchor="middle" class="muted">Merge-konflikter</text><text x="273" y="175" text-anchor="middle" class="muted">sista dagen</text>
<rect class="q1" x="202" y="194" width="142" height="44" rx="3"/><text x="273" y="212" text-anchor="middle" class="muted">Ingen testade</text><text x="273" y="229" text-anchor="middle" class="muted">på mobil</text>
<rect class="q2" x="374" y="140" width="142" height="44" rx="3"/><text x="445" y="158" text-anchor="middle" class="muted">Små PR:er är lättare</text><text x="445" y="175" text-anchor="middle" class="muted">att granska</text>
<rect class="q2" x="374" y="194" width="142" height="44" rx="3"/><text x="445" y="212" text-anchor="middle" class="muted">Fråga kunden</text><text x="445" y="229" text-anchor="middle" class="muted">tidigt</text>
<rect class="q3" x="546" y="140" width="142" height="44" rx="3"/><text x="617" y="158" text-anchor="middle" class="muted">Max 1 dag per PR</text><text x="617" y="175" text-anchor="middle" class="muted">Ansvar: Sara</text>
<rect class="q3" x="546" y="194" width="142" height="44" rx="3"/><text x="617" y="212" text-anchor="middle" class="muted">Mobiltest i DoD</text><text x="617" y="229" text-anchor="middle" class="muted">Ansvar: Ali</text>
<line class="leader" x1="101" y1="272" x2="101" y2="288"/><text x="101" y="300" text-anchor="middle" class="part">Kolumn</text>
<line class="leader" x1="273" y1="240" x2="273" y2="288"/><text x="273" y="300" text-anchor="middle" class="part">Lapp</text>
<line class="leader" x1="617" y1="240" x2="617" y2="288"/><text x="617" y="300" text-anchor="middle" class="part">Åtgärd med ägare</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Rubrik** | Överst på tavlan | Vilken sprint, period eller vilket projekt retron gäller |
| **Kolumn** | En lodrät yta per fråga | En av retrons frågor. Varje lapp hör hemma i exakt en kolumn |
| **Kolumnrubrik** | Färgad ruta överst i kolumnen | Frågan: *Gick bra*, *Gick mindre bra*, *Lärdomar*, *Åtgärder* |
| **Lapp** | En liten ruta (post-it) | En iakttagelse — en sak per lapp, kort formulerad |
| **Åtgärd med ägare** | Lapp i sista kolumnen | Något teamet ska *göra* nästa sprint, med ett namn på. Det är den här kolumnen som gör retron värd tiden |

**Så används kolumnerna:**

- **Gick bra** — vad vill vi fortsätta med?
- **Gick mindre bra** — vad skavde? Beskriv situationen, inte personen.
- **Lärdomar** — vad vet vi nu som vi inte visste för två veckor sedan?
- **Åtgärder** — max två eller tre, med ägare. Gör dem gärna [SMART](smart-mal.md). Återkommer samma problem varje retro, gräv i orsaken med [5 varför](fem-varfor.md).

### Variant: Start-Stop-Continue

En snabbare retro med tre kolumner som handlar om **vad teamet gör**:

| Start | Stop | Continue |
|-------|------|----------|
| Vad borde vi börja göra? | Vad borde vi sluta göra? | Vad funkar och ska fortsätta? |
| *Granska PR:er samma dag* | *Mergea sent på fredagar* | *Parprogrammera på svåra delar* |

Start-Stop-Continue passar när teamet är inne i en rytm och vill justera. Fyrkolumnstavlan ovan passar bättre efter en tuff sprint, när ni behöver förstå vad som hände innan ni bestämmer vad ni ska ändra.

## Exempel — standup-tavlan

Standup-tavlan har en rad per person och tre kolumner. Den sitter uppe hela sprinten (eller ligger i ett digitalt verktyg), och varje morgon flyttar alla sina lappar.

<svg class="dg" viewBox="0 0 720 285" role="img" aria-labelledby="rs2-t" xmlns="http://www.w3.org/2000/svg">
<title id="rs2-t">Standup-tavla med kolumnerna igår, idag och hinder och en rad per person: Sara, Ali och Jonas. Jonas har ett hinder: väntar på API-nyckel</title>
<rect class="box" x="20" y="20" width="100" height="32" rx="4"/><text x="70" y="41" text-anchor="middle" class="title">Vem</text>
<rect class="box" x="130" y="20" width="186" height="32" rx="4"/><text x="223" y="41" text-anchor="middle" class="title">Igår</text>
<rect class="box" x="326" y="20" width="186" height="32" rx="4"/><text x="419" y="41" text-anchor="middle" class="title">Idag</text>
<rect class="box" x="522" y="20" width="186" height="32" rx="4"/><text x="615" y="41" text-anchor="middle" class="title">Hinder</text>
<rect class="box" x="20" y="62" width="100" height="50" rx="4"/><text x="70" y="92" text-anchor="middle" class="title">Sara</text>
<rect class="box" x="20" y="122" width="100" height="50" rx="4"/><text x="70" y="152" text-anchor="middle" class="title">Ali</text>
<rect class="box" x="20" y="182" width="100" height="50" rx="4"/><text x="70" y="212" text-anchor="middle" class="title">Jonas</text>
<rect class="q2" x="138" y="68" width="170" height="38" rx="3"/><text x="223" y="92" text-anchor="middle" class="muted">Klar med inloggningen</text>
<rect class="q4" x="334" y="68" width="170" height="38" rx="3"/><text x="419" y="92" text-anchor="middle" class="muted">Börjar på avbokning</text>
<text x="615" y="92" text-anchor="middle" class="muted">—</text>
<rect class="q2" x="138" y="128" width="170" height="38" rx="3"/><text x="223" y="152" text-anchor="middle" class="muted">Fixade mobilvyn</text>
<rect class="q4" x="334" y="128" width="170" height="38" rx="3"/><text x="419" y="152" text-anchor="middle" class="muted">Granskar Saras PR</text>
<text x="615" y="152" text-anchor="middle" class="muted">—</text>
<rect class="q2" x="138" y="188" width="170" height="38" rx="3"/><text x="223" y="212" text-anchor="middle" class="muted">Skrev tester för bokning</text>
<rect class="q4" x="334" y="188" width="170" height="38" rx="3"/><text x="419" y="212" text-anchor="middle" class="muted">Kopplar mot betal-API</text>
<rect class="q1" x="530" y="188" width="170" height="38" rx="3"/><text x="615" y="212" text-anchor="middle" class="muted">Väntar på API-nyckel</text>
<line class="leader" x1="70" y1="234" x2="70" y2="258"/><text x="70" y="272" text-anchor="middle" class="part">En rad per person</text>
<line class="leader" x1="419" y1="228" x2="419" y2="258"/><text x="419" y="272" text-anchor="middle" class="part">Lapp</text>
<line class="leader" x1="615" y1="228" x2="615" y2="258"/><text x="615" y="272" text-anchor="middle" class="part">Hinder → hjälp efter mötet</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Igår** | Första kolumnen | Det jag blev klar med eller jobbade på sedan förra standup |
| **Idag** | Andra kolumnen | Det jag ska göra fram till nästa standup |
| **Hinder** (*blockers*) | Tredje kolumnen, gärna i varningsfärg | Det som stoppar mig och som jag behöver hjälp med |
| **Rad per person** | En vågrät rad | Alla svarar på samma tre frågor — ingen hoppas över |

Det viktiga på tavlan är den röda lappen. Jonas kan inte koppla mot betal-API:t förrän någon skaffat en nyckel. Hindret **löses inte på standupen** — det noteras, och den som kan hjälpa (oftast Scrum Master eller Product Owner) tar det med Jonas direkt efteråt.

## Mall att kopiera

**Retrospektiv**

```markdown
## Retro: <Sprint / period / projekt>
**Datum:** <åååå-mm-dd>  **Deltagare:**

### Uppföljning från förra retron
- [ ] <åtgärd> — <ansvarig> — klar? ja/nej

### Gick bra
-

### Gick mindre bra
-

### Lärdomar
-

### Åtgärder
| Åtgärd | Ansvarig | Klart senast |
|--------|----------|--------------|
|        |          |              |
```

**Start-Stop-Continue**

```markdown
## Retro: <Sprint / period>

| Start | Stop | Continue |
|-------|------|----------|
| -     | -    | -        |
```

**Daily standup**

```markdown
## Standup <åååå-mm-dd>

| Vem | Igår gjorde jag… | Idag ska jag… | Hinder |
|-----|------------------|---------------|--------|
|     |                  |               |        |

### Anteckningar
- <hinder som ska lösas efter mötet, och vem som tar det>
```

## När ska du välja vilken tavla?

| Välj… | När… |
|-------|------|
| **Gick bra / Gick mindre bra / Lärdomar / Åtgärder** | Efter en sprint där mycket hänt och ni behöver förstå varför |
| **Start-Stop-Continue** | Teamet har en rytm och vill göra små justeringar snabbt |
| **Igår / Idag / Hinder** | Varje dag, för att synka och hitta hinder tidigt |
| Något annat: [5 varför](fem-varfor.md) | Samma problem dyker upp i "Gick mindre bra" retro efter retro |
| Något annat: [prioriteringsmatriser](prioriteringsmatriser.md) | Retron gav för många åtgärder och ni måste välja |

## Vanliga misstag

- **Retro utan åtgärder.** Om sista kolumnen är tom har ni haft ett trevligt samtal, inte en retro.
- **Åtgärder utan ägare.** "Vi ska testa mer" blir aldrig av. Skriv ett namn på lappen.
- **Ingen uppföljning.** Börja varje retro med att titta på förra gångens åtgärder.
- **Standupen blir ett problemlösningsmöte.** Hinder ska *synas* på standupen och *lösas* efteråt, av dem som berörs.
- **"Igår: jobbade. Idag: jobbar vidare."** Skriv vad — så att andra kan se om de kan hjälpa eller om ni gör samma sak.

## Övning

Håll en retro i er projektgrupp med fyrkolumnstavlan. Varje person skriver tre lappar per kolumn under fem minuter i tystnad, sedan läser ni upp och grupperar. Bestäm max två åtgärder, gör dem SMART och skriv ett namn på varje. Nästa retro börjar med att ni följer upp dem.

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Retrotavla | Gick bra / Gick mindre bra / Lärdomar / Åtgärder |
| Start-Stop-Continue | Snabb retro om vad teamet gör |
| Standup-tavla | Igår / Idag / Hinder, en rad per person |
| Åtgärd med ägare | Det som gör retron värd tiden |
| Hinder | Syns på standupen, löses efter den |
