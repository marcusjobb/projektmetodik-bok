---
title: Organisationsschema
description: "Ett organisationsschema visar vem som rapporterar till vem — roller, nivåer och stabsfunktioner. Bra för att förstå en organisation, men det beskriver inte hur ett agilt team faktiskt jobbar."
parent: Diagram & analysverktyg
nav_order: 50
---

# Organisationsschema

## Grundidén

Ett **organisationsschema** visar hur en organisation är uppbyggd: vilka roller som finns, och **vem som rapporterar till vem**. Det klassiska schemat är ett träd med den högsta chefen överst. Varje linje nedåt betyder "är chef över" — och därmed vem som sätter lön, godkänner semester och har personalansvar.

När ni börjar på en LIA-plats eller i ett kundprojekt är schemat ofta det första ni behöver: *vem frågar jag om vad?*

## Vad används det till?

- **Förstå en ny arbetsplats** — vem är min chef, och vem är min chefs chef?
- **Hitta rätt person** — vem beslutar om budget, vem äger systemet ni ska integrera mot?
- **Planera ett projekt** — vilka avdelningar berörs, och vem behöver godkänna?
- **Se otydligheter** — personer med två chefer, eller roller som ingen äger

## Delarna och vad de heter

<svg class="dg" viewBox="0 0 720 345" role="img" aria-labelledby="os1-t" xmlns="http://www.w3.org/2000/svg">
<title id="os1-t">Organisationsschema med namngivna delar: ruta för roll, rapportlinje, nivåer, stabsfunktion vid sidan av linjen och matrislinje till ett projekt</title>
<rect class="hl" x="225" y="20" width="140" height="40" rx="4"/><text x="295" y="45" text-anchor="middle" class="title">VD</text>
<line class="line dash" x1="295" y1="80" x2="400" y2="80"/>
<rect class="box" x="400" y="64" width="130" height="32" rx="4"/><text x="465" y="85" text-anchor="middle">HR &amp; ekonomi</text>
<line class="line strong" x1="295" y1="60" x2="295" y2="120"/>
<line class="line strong" x1="155" y1="120" x2="435" y2="120"/>
<line class="line strong" x1="155" y1="120" x2="155" y2="140"/>
<line class="line strong" x1="295" y1="120" x2="295" y2="140"/>
<line class="line strong" x1="435" y1="120" x2="435" y2="140"/>
<rect class="box" x="95" y="140" width="120" height="40" rx="4"/><text x="155" y="165" text-anchor="middle">Sälj</text>
<rect class="box" x="235" y="140" width="120" height="40" rx="4"/><text x="295" y="165" text-anchor="middle">Utveckling</text>
<rect class="box" x="375" y="140" width="120" height="40" rx="4"/><text x="435" y="165" text-anchor="middle">Drift</text>
<line class="line strong" x1="295" y1="180" x2="295" y2="205"/>
<line class="line strong" x1="225" y1="205" x2="365" y2="205"/>
<line class="line strong" x1="225" y1="205" x2="225" y2="230"/>
<line class="line strong" x1="365" y1="205" x2="365" y2="230"/>
<rect class="box" x="170" y="230" width="110" height="40" rx="4"/><text x="225" y="255" text-anchor="middle">Team A</text>
<rect class="box" x="310" y="230" width="110" height="40" rx="4"/><text x="365" y="255" text-anchor="middle">Team B</text>
<path class="line dash" d="M365 270V308H400"/>
<line class="line dash" x1="435" y1="180" x2="435" y2="290"/>
<rect class="q3" x="400" y="290" width="140" height="36" rx="4"/><text x="470" y="313" text-anchor="middle">Kundprojekt X</text>
<text x="20" y="45" class="part">Nivå 1</text>
<text x="20" y="165" class="part">Nivå 2</text>
<text x="20" y="255" class="part">Nivå 3</text>
<line class="leader" x1="365" y1="40" x2="555" y2="40"/><text x="560" y="44" class="part">Ruta / roll</text>
<line class="leader" x1="530" y1="80" x2="555" y2="80"/><text x="560" y="84" class="part">Stabsfunktion</text>
<line class="leader" x1="435" y1="130" x2="555" y2="120"/><text x="560" y="124" class="part">Rapportlinje</text>
<line class="leader" x1="437" y1="240" x2="555" y2="236"/><text x="560" y="240" class="part">Matrislinje</text>
<line class="leader" x1="540" y1="308" x2="555" y2="308"/><text x="560" y="312" class="part">Projekt (matris)</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Ruta / roll** | Rektangel med rolltitel (ibland namn) | En befattning, en avdelning eller ett team. Skriv rollen — personer byts ut |
| **Rapportlinje** | Heldragen linje uppåt | "Rapporterar till" — linjechefen, med personalansvar |
| **Nivå** | Rutor på samma höjd | Samma steg i hierarkin. Antalet nivåer säger hur "platt" organisationen är |
| **Stabsfunktion** | Ruta vid sidan av en linje, ofta med streckad koppling | Stöd till chefen — HR, ekonomi, juridik — som inte är chef över linjen under |
| **Matrislinje** | Prickad eller streckad linje | Ett andra sammanhang personen jobbar i, oftast ett projekt. Projektledaren styr *arbetet*, linjechefen styr *anställningen* |
| **Projekt (matris)** | Ruta som "korsar" linjeorganisationen | Ett tillfälligt uppdrag där personer från flera avdelningar jobbar ihop |

En organisation där folk har både en linjechef och en projektchef kallas **matrisorganisation**. Den är vanlig i konsultbolag — och den är källan till frågan "vem bestämmer egentligen?" när två chefer vill olika saker.

## Exempel — ett IT-konsultbolag och ett Scrum-team

Ett IT-konsultbolag har konsulterna organiserade efter kompetens — en konsultchef för .NET, en för Cloud. Men konsulterna arbetar ute hos kunder. Konsult B och Konsult D sitter just nu i samma kunduppdrag:

<svg class="dg" viewBox="0 0 720 360" role="img" aria-labelledby="os2-t" xmlns="http://www.w3.org/2000/svg">
<title id="os2-t">Organisationsschema för ett IT-konsultbolag: VD med stabsfunktion, fyra avdelningar, konsulter under två konsultchefer, och två konsulter kopplade med streckade linjer till ett kunduppdrag</title>
<rect class="hl" x="290" y="20" width="140" height="38" rx="4"/><text x="360" y="44" text-anchor="middle" class="title">VD</text>
<line class="line dash" x1="360" y1="80" x2="470" y2="80"/>
<rect class="box" x="470" y="64" width="140" height="32" rx="4"/><text x="540" y="85" text-anchor="middle">Ekonomi &amp; HR</text>
<line class="line strong" x1="360" y1="58" x2="360" y2="120"/>
<line class="line strong" x1="95" y1="120" x2="620" y2="120"/>
<line class="line strong" x1="95" y1="120" x2="95" y2="140"/>
<line class="line strong" x1="270" y1="120" x2="270" y2="140"/>
<line class="line strong" x1="445" y1="120" x2="445" y2="140"/>
<line class="line strong" x1="620" y1="120" x2="620" y2="140"/>
<rect class="box" x="20" y="140" width="150" height="40" rx="4"/><text x="95" y="165" text-anchor="middle">Sälj</text>
<rect class="box" x="195" y="140" width="150" height="40" rx="4"/><text x="270" y="165" text-anchor="middle">Konsultchef .NET</text>
<rect class="box" x="370" y="140" width="150" height="40" rx="4"/><text x="445" y="165" text-anchor="middle">Konsultchef Cloud</text>
<rect class="box" x="545" y="140" width="150" height="40" rx="4"/><text x="620" y="165" text-anchor="middle">Intern IT</text>
<path class="line strong" d="M215 180V266M215 221H230M215 266H230"/>
<rect class="box" x="230" y="205" width="115" height="32" rx="4"/><text x="287" y="226" text-anchor="middle">Konsult A</text>
<rect class="box" x="230" y="250" width="115" height="32" rx="4"/><text x="287" y="271" text-anchor="middle">Konsult B</text>
<path class="line strong" d="M390 180V266M390 221H405M390 266H405"/>
<rect class="box" x="405" y="205" width="115" height="32" rx="4"/><text x="462" y="226" text-anchor="middle">Konsult C</text>
<rect class="box" x="405" y="250" width="115" height="32" rx="4"/><text x="462" y="271" text-anchor="middle">Konsult D</text>
<line class="line dash" x1="287" y1="282" x2="287" y2="310"/>
<line class="line dash" x1="462" y1="282" x2="462" y2="310"/>
<rect class="q3" x="230" y="310" width="290" height="36" rx="4"/><text x="375" y="333" text-anchor="middle">Uppdrag hos kund: bokningssystem</text>
</svg>

Konsult B:s **linjechef** är konsultchefen för .NET — det är hen som har utvecklingssamtal och sätter lön. Men det dagliga arbetet styrs i kunduppdraget. Det är en matris, och det är därför konsulter ofta har *två* frågor att hålla isär: "vad ska jag göra idag?" (uppdraget) och "hur går det för mig?" (linjechefen).

Inne i kunduppdraget jobbar B och D i ett **Scrum-team**. Och här slutar organisationsschemat att fungera — för Scrum-rollerna är inte en hierarki:

<svg class="dg" viewBox="0 0 720 280" role="img" aria-labelledby="os3-t" xmlns="http://www.w3.org/2000/svg">
<title id="os3-t">Ett Scrum-team ritat som tre roller på samma nivå — Product Owner, Scrum Master och Utvecklare — som delar samma produktmål, med konsultchefen utanför teamet</title>
<rect class="box" x="20" y="20" width="140" height="36" rx="4"/><text x="90" y="43" text-anchor="middle">Konsultchef</text>
<path class="line dash" d="M90 56V140H190"/>
<text x="20" y="170" class="muted">personalansvar —</text>
<text x="20" y="188" class="muted">inte teamchef</text>
<rect class="line dash" x="190" y="20" width="510" height="240" rx="16"/>
<text x="445" y="48" text-anchor="middle" class="title">Scrum-team</text>
<rect class="box" x="215" y="80" width="140" height="40" rx="4"/><text x="285" y="105" text-anchor="middle">Product Owner</text>
<rect class="box" x="375" y="80" width="140" height="40" rx="4"/><text x="445" y="105" text-anchor="middle">Scrum Master</text>
<rect class="box" x="535" y="80" width="140" height="40" rx="4"/><text x="605" y="105" text-anchor="middle">Utvecklare</text>
<line class="line strong" x1="355" y1="100" x2="375" y2="100"/>
<line class="line strong" x1="515" y1="100" x2="535" y2="100"/>
<text x="285" y="142" text-anchor="middle" class="muted">vad och varför</text>
<text x="285" y="160" text-anchor="middle" class="muted">(prioriterar)</text>
<text x="445" y="142" text-anchor="middle" class="muted">hur vi jobbar</text>
<text x="445" y="160" text-anchor="middle" class="muted">(tar bort hinder)</text>
<text x="605" y="142" text-anchor="middle" class="muted">bygger produkten</text>
<text x="605" y="160" text-anchor="middle" class="muted">(självorganiserade)</text>
<rect class="hl" x="215" y="180" width="460" height="36" rx="4"/><text x="445" y="203" text-anchor="middle">Produktmålet — samma mål för alla tre rollerna</text>
<text x="445" y="245" text-anchor="middle" class="muted">Ingen av rollerna är chef över de andra</text>
</svg>

Tre saker att lägga märke till:

- **Rollerna står bredvid varandra, inte över.** Product Owner bestämmer *vad* som är viktigast, men inte *hur* utvecklarna ska jobba. Scrum Master är inte en chef — se [Roller](../agilt/roller.md).
- **Linjechefen står utanför teamet.** Konsultchefen har personalansvar men lägger sig inte i sprinten.
- **Det som håller ihop teamet är målet**, inte en rapportlinje. Därför ritas det som en gemensam grund snarare än en topp.

Försöker man rita in ett Scrum-team i ett vanligt träd — med Scrum Master överst — har man missförstått [Scrum](../agilt/scrum.md).

## När ska du välja ett organisationsschema?

| Välj organisationsschema när… | Välj något annat när… |
|-------------------------------|-----------------------|
| Frågan är vem som är chef över vem | Frågan är vem som *gör* vad i en process → [BPMN och simbanor](bpmn-och-simbanor.md) |
| Ni ska förstå en kunds eller LIA-plats organisation | Ni vill visa hur ett agilt team samarbetar — rita rollerna på samma nivå, som ovan |
| Ni ska ta reda på vem som behöver godkänna något | Ni vill reda ut vem som har ansvar för vilka beslut — en ansvarsmatris (RACI-tabell) passar bättre |

## Vanliga misstag

- **Blanda roller och personer.** Skriv rollen ("Konsultchef .NET") och lägg till namn om det behövs. Annars är schemat inaktuellt efter första personalbytet.
- **Rita Scrum som ett träd.** Product Owner överst, Scrum Master under, utvecklare längst ner — fel på alla tre punkterna.
- **Glömma matrisen.** I många organisationer är det streckade linjerna som styr vardagen. Utan dem ser schemat enklare ut än verkligheten.
- **Stabsfunktion som chef.** HR ritas vid sidan av, inte ovanför avdelningarna — HR är inte chef över utvecklarna.
- **För många nivåer i ett schema.** Rita ett översiktsschema och ett detaljerat per avdelning hellre än allt på en gång.

## Mall att kopiera

| Roll | Rapporterar till (linje) | Streckad linje till (projekt/uppdrag) | Stab? | Person (valfritt) |
|------|--------------------------|----------------------------------------|-------|-------------------|
| | — | | | |
| | | | | |
| | | | | |

Varje rad blir en ruta; kolumnen *Rapporterar till* blir de heldragna linjerna, nästa kolumn de streckade.

## Övning

Rita organisationsschemat för er utbildning: utbildningsledare, lärare/utbildare, studerande, ledningsgrupp, eventuell LIA-handledare. Var sitter LIA-handledaren — i trädet, eller på en streckad linje? Rita sedan er projektgrupp som ett Scrum-team. Vem i gruppen har vilken roll, och är någon av dem *chef*?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Organisationsschema | Vem rapporterar till vem — ett träd |
| Rapportlinje | Heldragen linje: linjechef, personalansvar |
| Stabsfunktion | Stöd vid sidan av linjen, t.ex. HR |
| Matrisorganisation | Linjechef + projekt — streckade linjer |
| Scrum-team | Tre roller på samma nivå, inte en hierarki |
