---
title: Kundresa
description: "En kundresa (user journey map) visar hur en användare upplever hela vägen från att hon hör talas om er tjänst till att hon har använt den — steg, kontaktpunkter och känslor."
parent: Diagram & analysverktyg
nav_order: 20
---

# Kundresa

## Grundidén

En **kundresa** — på engelska *user journey map* eller *customer journey map* — beskriver en användares väg genom er tjänst **ur användarens perspektiv**. Inte hur systemet fungerar, utan vad hon gör, var hon möter er, och hur hon *känner sig* på vägen.

Kärnan är **känslokurvan**: en linje som går upp när något känns bra och ner när det skaver. De djupaste dalarna är teamets bästa ledtrådar till vad som ska byggas eller förbättras härnäst.

## Vad används det till?

- **Hitta smärtpunkter** — var tappar ni användaren, var blir hon förvirrad eller irriterad?
- **Prioritera backlogen** — en dal i kurvan blir ofta en eller flera [user stories](../begrepp/user-story-och-mvp.md)
- **Skapa en gemensam bild** i teamet av vem ni bygger för
- **Se helheten** — användaren upplever inte "appen" och "mejlet" och "dörrskylten" som separata saker, men teamet bygger dem ofta var för sig

## Delarna och vad de heter

En kundresa ritas som ett rutnät: faserna går från vänster till höger, och varje rad svarar på en fråga om just den fasen.

<svg class="dg" viewBox="0 0 720 390" role="img" aria-labelledby="ku1-t" xmlns="http://www.w3.org/2000/svg">
<title id="ku1-t">Kundresa med namngivna delar: persona, faser, aktiviteter, kontaktpunkter, känslokurva, smärtpunkt och möjlighet</title>
<rect class="hl" x="40" y="20" width="470" height="40" rx="4"/><text x="56" y="45">Sara, 22, student — vill hitta ett grupprum snabbt</text>
<rect class="box" x="40" y="72" width="150" height="30" rx="4"/><text x="115" y="92" text-anchor="middle" class="title">Upptäcka</text>
<rect class="box" x="200" y="72" width="150" height="30" rx="4"/><text x="275" y="92" text-anchor="middle" class="title">Boka</text>
<rect class="box" x="360" y="72" width="150" height="30" rx="4"/><text x="435" y="92" text-anchor="middle" class="title">Använda</text>
<rect class="box" x="40" y="110" width="150" height="40" rx="4"/><text x="115" y="135" text-anchor="middle" class="muted">Hör om appen</text>
<rect class="box" x="200" y="110" width="150" height="40" rx="4"/><text x="275" y="135" text-anchor="middle" class="muted">Väljer rum och tid</text>
<rect class="box" x="360" y="110" width="150" height="40" rx="4"/><text x="435" y="135" text-anchor="middle" class="muted">Checkar in</text>
<rect class="q2" x="40" y="158" width="150" height="40" rx="4"/><text x="115" y="183" text-anchor="middle" class="muted">Kurskamrat</text>
<rect class="q2" x="200" y="158" width="150" height="40" rx="4"/><text x="275" y="183" text-anchor="middle" class="muted">Bokningsvyn i appen</text>
<rect class="q2" x="360" y="158" width="150" height="40" rx="4"/><text x="435" y="183" text-anchor="middle" class="muted">QR-kod vid dörren</text>
<rect class="line" x="40" y="206" width="470" height="80"/>
<line class="line dash" x1="40" y1="246" x2="510" y2="246"/>
<text x="48" y="224" class="muted">+</text><text x="48" y="280" class="muted">−</text>
<path class="line strong" d="M115 226C195 226 195 272 275 272C355 272 355 232 435 232"/>
<circle class="solid" cx="115" cy="226" r="4"/><circle class="q1" cx="275" cy="272" r="6"/><circle class="solid" cx="435" cy="232" r="4"/>
<line class="line dash" x1="275" y1="278" x2="275" y2="294"/>
<rect class="q1" x="200" y="294" width="150" height="36" rx="4"/><text x="275" y="317" text-anchor="middle" class="muted">Krånglig tidsväljare</text>
<rect class="q4" x="200" y="338" width="150" height="36" rx="4"/><text x="275" y="361" text-anchor="middle" class="muted">Visa lediga rum först</text>
<line class="leader" x1="510" y1="40" x2="525" y2="40"/><text x="530" y="44" class="part">Persona</text>
<line class="leader" x1="510" y1="87" x2="525" y2="87"/><text x="530" y="91" class="part">Fas</text>
<line class="leader" x1="510" y1="130" x2="525" y2="130"/><text x="530" y="134" class="part">Aktivitet</text>
<line class="leader" x1="510" y1="178" x2="525" y2="178"/><text x="530" y="182" class="part">Kontaktpunkt (touchpoint)</text>
<line class="leader" x1="439" y1="233" x2="525" y2="246"/><text x="530" y="250" class="part">Känslokurva</text>
<line class="leader" x1="350" y1="312" x2="525" y2="312"/><text x="530" y="316" class="part">Smärtpunkt</text>
<line class="leader" x1="350" y1="356" x2="525" y2="356"/><text x="530" y="360" class="part">Möjlighet</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Persona** | Ruta överst med namn, ålder, mål | En påhittad men realistisk användare. Resan gäller *henne*, inte "alla användare" |
| **Fas** | Kolumnrubrik | Ett större skede i resan, t.ex. Upptäcka → Jämföra → Boka → Använda → Följa upp |
| **Aktivitet** | Rad med vad personen *gör* | Konkreta handlingar i fasen, skrivna från användarens håll |
| **Kontaktpunkt** (touchpoint) | Rad med var hon möter er | Kanalen: appen, ett mejl, en skylt, en kompis, kundtjänst |
| **Känslokurva** | Linje som går upp och ner | Hur det känns i varje fas — över mittlinjen bra, under dålig |
| **Smärtpunkt** | Röd markering, ofta vid en dal i kurvan | Något som skaver: förvirring, väntan, irritation |
| **Möjlighet** | Grön ruta under smärtpunkten | Teamets idé om hur smärtpunkten kan lösas |

## Exempel — en student bokar grupprum

Teamet bygger en bokningsapp för skolans grupprum. Efter fem korta intervjuer med studenter ritar de Saras resa. Kurvan går ner i *Boka* — alla fem tyckte att det var svårt att se vilka rum som var lediga.

<svg class="dg" viewBox="0 0 720 460" role="img" aria-labelledby="ku2-t" xmlns="http://www.w3.org/2000/svg">
<title id="ku2-t">Kundresa för en student som bokar grupprum, med fem faser och en känslokurva som går ner i fasen Boka</title>
<text x="20" y="48" class="muted">Persona</text>
<rect class="hl" x="120" y="20" width="580" height="46" rx="4"/>
<text x="136" y="40" class="title">Sara, 22, studerar systemutveckling</text>
<text x="136" y="58" class="muted">Mål: boka ett grupprum till gruppen inför tentan — snabbt, från mobilen</text>
<text x="20" y="95" class="muted">Fas</text>
<rect class="box" x="120" y="76" width="112" height="28" rx="4"/><text x="176" y="95" text-anchor="middle" class="title">Upptäcka</text>
<rect class="box" x="236" y="76" width="112" height="28" rx="4"/><text x="292" y="95" text-anchor="middle" class="title">Jämföra</text>
<rect class="box" x="352" y="76" width="112" height="28" rx="4"/><text x="408" y="95" text-anchor="middle" class="title">Boka</text>
<rect class="box" x="468" y="76" width="112" height="28" rx="4"/><text x="524" y="95" text-anchor="middle" class="title">Använda</text>
<rect class="box" x="584" y="76" width="112" height="28" rx="4"/><text x="640" y="95" text-anchor="middle" class="title">Följa upp</text>
<text x="20" y="140" class="muted">Aktiviteter</text>
<rect class="box" x="120" y="110" width="112" height="50" rx="4"/><text x="176" y="130" text-anchor="middle" class="muted">Hör om appen</text><text x="176" y="148" text-anchor="middle" class="muted">av en kurskamrat</text>
<rect class="box" x="236" y="110" width="112" height="50" rx="4"/><text x="292" y="130" text-anchor="middle" class="muted">Jämför med</text><text x="292" y="148" text-anchor="middle" class="muted">att maila skolan</text>
<rect class="box" x="352" y="110" width="112" height="50" rx="4"/><text x="408" y="130" text-anchor="middle" class="muted">Väljer rum</text><text x="408" y="148" text-anchor="middle" class="muted">och tid</text>
<rect class="box" x="468" y="110" width="112" height="50" rx="4"/><text x="524" y="130" text-anchor="middle" class="muted">Checkar in</text><text x="524" y="148" text-anchor="middle" class="muted">med QR-kod</text>
<rect class="box" x="584" y="110" width="112" height="50" rx="4"/><text x="640" y="130" text-anchor="middle" class="muted">Får en fråga om</text><text x="640" y="148" text-anchor="middle" class="muted">betyg på rummet</text>
<text x="20" y="196" class="muted">Kontaktpunkter</text>
<rect class="q2" x="120" y="166" width="112" height="50" rx="4"/><text x="176" y="186" text-anchor="middle" class="muted">Kurskamrat,</text><text x="176" y="204" text-anchor="middle" class="muted">Instagram</text>
<rect class="q2" x="236" y="166" width="112" height="50" rx="4"/><text x="292" y="186" text-anchor="middle" class="muted">Appbutiken,</text><text x="292" y="204" text-anchor="middle" class="muted">skolans webb</text>
<rect class="q2" x="352" y="166" width="112" height="50" rx="4"/><text x="408" y="186" text-anchor="middle" class="muted">Bokningsvyn</text><text x="408" y="204" text-anchor="middle" class="muted">i appen</text>
<rect class="q2" x="468" y="166" width="112" height="50" rx="4"/><text x="524" y="186" text-anchor="middle" class="muted">QR-kod på</text><text x="524" y="204" text-anchor="middle" class="muted">dörren</text>
<rect class="q2" x="584" y="166" width="112" height="50" rx="4"/><text x="640" y="186" text-anchor="middle" class="muted">Push-notis</text><text x="640" y="204" text-anchor="middle" class="muted">och mejl</text>
<text x="20" y="283" class="muted">Känslokurva</text>
<rect class="line" x="120" y="222" width="576" height="114"/>
<line class="line dash" x1="120" y1="275" x2="696" y2="275"/>
<text x="128" y="240" class="muted">+</text><text x="128" y="330" class="muted">−</text>
<path class="line strong" d="M176 252C234 252 234 284 292 284C350 284 350 310 408 310C466 310 466 242 524 242C582 242 582 256 640 256"/>
<circle class="solid" cx="176" cy="252" r="4"/><circle class="solid" cx="292" cy="284" r="4"/><circle class="q1" cx="408" cy="310" r="6"/><circle class="solid" cx="524" cy="242" r="4"/><circle class="solid" cx="640" cy="256" r="4"/>
<text x="176" y="243" text-anchor="middle" class="muted">nyfiken</text>
<text x="292" y="304" text-anchor="middle" class="muted">osäker</text>
<text x="408" y="331" text-anchor="middle" class="muted">frustrerad</text>
<text x="524" y="233" text-anchor="middle" class="muted">lättad</text>
<text x="640" y="247" text-anchor="middle" class="muted">nöjd</text>
<text x="20" y="372" class="muted">Smärtpunkter</text>
<rect class="q1" x="236" y="342" width="112" height="50" rx="4"/><text x="292" y="362" text-anchor="middle" class="muted">Oklart om appen</text><text x="292" y="380" text-anchor="middle" class="muted">kostar något</text>
<rect class="q1" x="352" y="342" width="112" height="50" rx="4"/><text x="408" y="362" text-anchor="middle" class="muted">Lediga tider</text><text x="408" y="380" text-anchor="middle" class="muted">syns inte direkt</text>
<text x="20" y="428" class="muted">Möjligheter</text>
<rect class="q4" x="236" y="398" width="112" height="50" rx="4"/><text x="292" y="418" text-anchor="middle" class="muted">Visa direkt att</text><text x="292" y="436" text-anchor="middle" class="muted">den är gratis</text>
<rect class="q4" x="352" y="398" width="112" height="50" rx="4"/><text x="408" y="418" text-anchor="middle" class="muted">Visa lediga rum</text><text x="408" y="436" text-anchor="middle" class="muted">först, i grönt</text>
</svg>

Så här läser teamet kartan:

1. **Djupaste dalen är *Boka*** — och det är just den fas där appen gör allt jobb. Det är teamets eget ansvar, så det hamnar högst i backlogen: "Som student vill jag se lediga rum direkt, så att jag slipper klicka mig igenom varje rum."
2. **Kurvan börjar sjunka redan i *Jämföra*** — i appbutiken och på skolans webb, alltså utanför appen. Smärtpunkten där är billig att åtgärda (en mening i beskrivningen), men syns bara om man ritar hela resan.
3. **Toppen i *Använda* ska skyddas.** QR-incheckningen fungerar — rör den inte i onödan.

## När ska du välja en kundresa?

| Välj kundresa när… | Välj något annat när… |
|--------------------|-----------------------|
| Ni vill förstå *upplevelsen*, inte bara flödet | Ni vill se vem *i teamet/organisationen* som gör vad → [BPMN och simbanor](bpmn-och-simbanor.md) |
| Användaren möter er i flera kanaler | Ni vill planera vilka sidor appen ska ha → [Sitemap](sitemap.md) |
| Ni ska prioritera vad som ska byggas först | Ni behöver rangordna en färdig lista idéer → [Prioriteringsmatriser](prioriteringsmatriser.md) |
| Ni har pratat med riktiga användare | Ni vill brainstorma fritt kring ett ämne → [Tankekarta](tankekarta.md) |

## Vanliga misstag

- **Hitta på känslorna.** En kundresa utan intervjuer eller observationer är teamets gissning i snygg förpackning. Prata med minst 3–5 riktiga användare.
- **Rita systemets flöde.** "Backend validerar bokningen" är ingen aktivitet för Sara. Skriv det hon gör och ser.
- **En persona för alla.** "Användaren, 18–65 år" hjälper ingen. Gör hellre två kartor för två olika personor.
- **Bara glada toppar.** Om kurvan aldrig går under mittlinjen har ni inte letat tillräckligt.
- **Kartan blir en tavla på väggen.** Varje smärtpunkt ska leda till en möjlighet — och de viktigaste ska in i backlogen.

## Mall att kopiera

**Persona:** *namn, ålder, situation* — **Mål:** *vad vill hen uppnå?*

| | Upptäcka | Jämföra | Boka | Använda | Följa upp |
|---|---|---|---|---|---|
| **Aktiviteter** — vad gör hen? | | | | | |
| **Kontaktpunkter** — var möter hen oss? | | | | | |
| **Tankar** — vad säger hen? | | | | | |
| **Känsla** (−2 till +2) | | | | | |
| **Smärtpunkter** | | | | | |
| **Möjligheter** | | | | | |

Fyll i känsla som en siffra först — det är lättare att bli överens om "−2" än om en kurva. Rita sedan kurvan genom siffrorna.

## Övning

Välj en tjänst ni alla har använt nyligen — t.ex. att köpa en tågbiljett eller anmäla sig till en tenta. Gör en kundresa var, utan att prata med varandra. Jämför sedan era känslokurvor: var är ni överens om dalarna, och var skiljer det sig? Vilken smärtpunkt skulle ni åtgärda först om ni var teamet bakom tjänsten?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Kundresa | Användarens väg genom tjänsten, ur hennes perspektiv |
| Persona | Den användare resan gäller |
| Fas | Ett skede i resan — kolumnerna |
| Kontaktpunkt | Var användaren möter er |
| Känslokurva | Hur det känns — dalarna visar var ni ska jobba |
| Smärtpunkt → möjlighet | Problemet → teamets idé om lösning |
