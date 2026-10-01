---
title: Sitemap
description: "En sitemap (webbplatskarta) visar vilka sidor en webbplats eller app har och hur de hänger ihop — ett träd som teamet ritar innan någon börjar designa eller koda."
parent: Diagram & analysverktyg
nav_order: 30
---

# Sitemap

## Grundidén

En **sitemap** — webbplatskarta — är ett träd över alla sidor i en webbplats eller app. Startsidan överst, sektionerna under, och sidorna i varje sektion under dem. Den svarar på två frågor: *vilka sidor behövs?* och *hur hittar man dit?*

**Inte samma sak som `sitemap.xml`.** Ordet används också om en XML-fil som ligger på en färdig webbplats och listar alla adresser åt Google och andra sökmotorer. Den genereras oftast automatiskt. Den här sidan handlar om planeringsverktyget — bilden teamet ritar innan sidorna finns.

## Vad används det till?

- **Planera omfånget** — hur många sidor handlar det om? Det påverkar hela tidsplanen
- **Bestämma navigeringen** — det som ligger på nivå 1 blir oftast huvudmenyn
- **Dela upp arbetet** i teamet — en sektion per person eller par
- **Skilja på MVP och senare** — vilka sidor måste finnas i första leveransen? (se [User story och MVP](../begrepp/user-story-och-mvp.md))
- **Se var inloggning behövs** — det styr både design och säkerhet

## Delarna och vad de heter

<svg class="dg" viewBox="0 0 720 350" role="img" aria-labelledby="sm1-t" xmlns="http://www.w3.org/2000/svg">
<title id="sm1-t">Sitemap med namngivna delar: startsida, hierarkilinje, sektion på nivå 1, sida på nivå 2, sida bakom inloggning och delade sidor i sidfoten</title>
<rect class="hl" x="200" y="20" width="140" height="40" rx="4"/><text x="270" y="45" text-anchor="middle" class="title">Startsida</text>
<line class="line strong" x1="270" y1="60" x2="270" y2="85"/>
<line class="line strong" x1="85" y1="85" x2="455" y2="85"/>
<line class="line strong" x1="85" y1="85" x2="85" y2="110"/>
<line class="line strong" x1="270" y1="85" x2="270" y2="110"/>
<line class="line strong" x1="455" y1="85" x2="455" y2="110"/>
<rect class="box" x="20" y="110" width="130" height="40" rx="4"/><text x="85" y="135" text-anchor="middle">Rum</text>
<rect class="box" x="205" y="110" width="130" height="40" rx="4"/><text x="270" y="135" text-anchor="middle">Hjälp</text>
<rect class="box" x="390" y="110" width="130" height="40" rx="4"/><text x="455" y="135" text-anchor="middle">Mina bokningar</text>
<rect class="solid" x="528" y="124" width="12" height="9" rx="1"/><path class="line strong" d="M530.5 124V120a3.5 3.5 0 0 1 7 0V124"/>
<path class="line" d="M40 150V233M40 191H55M40 233H55"/>
<rect class="box" x="55" y="175" width="110" height="32" rx="4"/><text x="110" y="196" text-anchor="middle">Rumslista</text>
<rect class="box" x="55" y="217" width="110" height="32" rx="4"/><text x="110" y="238" text-anchor="middle">Rumsdetalj</text>
<path class="line" d="M225 150V233M225 191H240M225 233H240"/>
<rect class="box" x="240" y="175" width="120" height="32" rx="4"/><text x="300" y="196" text-anchor="middle">Vanliga frågor</text>
<rect class="box" x="240" y="217" width="120" height="32" rx="4"/><text x="300" y="238" text-anchor="middle">Kontakt</text>
<path class="line" d="M410 150V233M410 191H425M410 233H425"/>
<rect class="box" x="425" y="175" width="110" height="32" rx="4"/><text x="480" y="196" text-anchor="middle">Kommande</text>
<rect class="box" x="425" y="217" width="110" height="32" rx="4"/><text x="480" y="238" text-anchor="middle">Historik</text>
<rect class="line dash" x="20" y="280" width="520" height="54" rx="4"/>
<text x="32" y="312" class="muted">Sidfot:</text>
<rect class="box" x="90" y="292" width="110" height="30" rx="4"/><text x="145" y="312" text-anchor="middle">Integritet</text>
<rect class="box" x="210" y="292" width="130" height="30" rx="4"/><text x="275" y="312" text-anchor="middle">Tillgänglighet</text>
<rect class="box" x="350" y="292" width="100" height="30" rx="4"/><text x="400" y="312" text-anchor="middle">Cookies</text>
<line class="leader" x1="340" y1="40" x2="555" y2="40"/><text x="560" y="44" class="part">Startsida</text>
<line class="leader" x1="460" y1="97" x2="555" y2="90"/><text x="560" y="94" class="part">Hierarkilinje</text>
<line class="leader" x1="543" y1="128" x2="555" y2="124"/><text x="560" y="128" class="part">Bakom inloggning</text>
<line class="leader" x1="520" y1="145" x2="555" y2="154"/><text x="560" y="158" class="part">Sektion (nivå 1)</text>
<line class="leader" x1="535" y1="191" x2="555" y2="191"/><text x="560" y="195" class="part">Sida (nivå 2)</text>
<line class="leader" x1="540" y1="307" x2="555" y2="307"/><text x="560" y="311" class="part">Delad/global sida</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Startsida** | Överst, ofta markerad | Ingången. Alla sidor ska gå att nå härifrån |
| **Sektion / nivå** | En rad i trädet | Nivå 1 blir oftast huvudmenyn; nivå 2 är sidorna inuti en sektion |
| **Sida** | Ruta | En vy användaren kan hamna på — en egen adress (URL) |
| **Hierarkilinje** | Linje från förälder till barn | "Den här sidan ligger under den där" — oftast också vägen i menyn |
| **Delad / global sida** | Utanför trädet, ofta i en streckad ram | Sidor som länkas från *alla* sidor, t.ex. i sidfoten |
| **Bakom inloggning** | Hänglås (eller streckad ruta) | Kräver att användaren är inloggad. Allt under en låst sektion är också låst |

En sitemap visar **struktur**, inte flöde. Pilar som visar "först gör man det här, sen det här" hör hemma i en [kundresa](kundresa.md) eller en [processkarta](bpmn-och-simbanor.md).

## Exempel — bokningsappens webbplats

Teamet som bygger bokningsappen för grupprum ritar sin sitemap i sprint 0. De markerar direkt vilka sidor som ingår i MVP:n, så att det syns att resten kan vänta.

<svg class="dg" viewBox="0 0 720 400" role="img" aria-labelledby="sm2-t" xmlns="http://www.w3.org/2000/svg">
<title id="sm2-t">Sitemap för en bokningsapp för grupprum med fyra sektioner, sidor bakom inloggning, sidfot och markering av vilka sidor som ingår i MVP</title>
<rect class="hl" x="290" y="20" width="140" height="40" rx="4"/><text x="360" y="45" text-anchor="middle" class="title">Startsida</text>
<line class="line strong" x1="430" y1="40" x2="500" y2="40"/>
<rect class="hl" x="500" y="20" width="120" height="40" rx="4"/><text x="560" y="45" text-anchor="middle">Logga in</text>
<line class="line strong" x1="360" y1="60" x2="360" y2="85"/>
<line class="line strong" x1="95" y1="85" x2="620" y2="85"/>
<line class="line strong" x1="95" y1="85" x2="95" y2="110"/>
<line class="line strong" x1="270" y1="85" x2="270" y2="110"/>
<line class="line strong" x1="445" y1="85" x2="445" y2="110"/>
<line class="line strong" x1="620" y1="85" x2="620" y2="110"/>
<rect class="hl" x="20" y="110" width="150" height="40" rx="4"/><text x="95" y="135" text-anchor="middle">Hitta rum</text>
<rect class="hl" x="195" y="110" width="150" height="40" rx="4"/><text x="262" y="135" text-anchor="middle">Mina bokningar</text>
<rect class="box" x="370" y="110" width="150" height="40" rx="4"/><text x="445" y="135" text-anchor="middle">Konto</text>
<rect class="box" x="545" y="110" width="150" height="40" rx="4"/><text x="620" y="135" text-anchor="middle">Hjälp</text>
<rect class="solid" x="326" y="127" width="12" height="9" rx="1"/><path class="line strong" d="M328.5 127V123a3.5 3.5 0 0 1 7 0V127"/>
<rect class="solid" x="501" y="127" width="12" height="9" rx="1"/><path class="line strong" d="M503.5 127V123a3.5 3.5 0 0 1 7 0V127"/>
<path class="line" d="M40 150V270M40 186H55M40 228H55M40 270H55"/>
<rect class="hl" x="55" y="170" width="115" height="32" rx="4"/><text x="112" y="191" text-anchor="middle">Rumslista</text>
<rect class="box" x="55" y="212" width="115" height="32" rx="4"/><text x="112" y="233" text-anchor="middle">Rumsdetalj</text>
<rect class="hl" x="55" y="254" width="115" height="32" rx="4"/><text x="112" y="275" text-anchor="middle">Boka rum</text>
<path class="line" d="M215 150V270M215 186H230M215 228H230M215 270H230"/>
<rect class="hl" x="230" y="170" width="115" height="32" rx="4"/><text x="287" y="191" text-anchor="middle">Kommande</text>
<rect class="box" x="230" y="212" width="115" height="32" rx="4"/><text x="287" y="233" text-anchor="middle">Historik</text>
<rect class="hl" x="230" y="254" width="115" height="32" rx="4"/><text x="287" y="275" text-anchor="middle">Avboka</text>
<path class="line" d="M390 150V228M390 186H405M390 228H405"/>
<rect class="box" x="405" y="170" width="115" height="32" rx="4"/><text x="462" y="191" text-anchor="middle">Profil</text>
<rect class="box" x="405" y="212" width="115" height="32" rx="4"/><text x="462" y="233" text-anchor="middle">Notiser</text>
<path class="line" d="M565 150V228M565 186H580M565 228H580"/>
<rect class="box" x="580" y="170" width="115" height="32" rx="4"/><text x="637" y="191" text-anchor="middle">Vanliga frågor</text>
<rect class="box" x="580" y="212" width="115" height="32" rx="4"/><text x="637" y="233" text-anchor="middle">Kontakta oss</text>
<rect class="line dash" x="20" y="305" width="676" height="46" rx="4"/>
<text x="32" y="333" class="muted">Sidfot:</text>
<rect class="hl" x="90" y="313" width="150" height="30" rx="4"/><text x="165" y="333" text-anchor="middle">Integritetspolicy</text>
<rect class="box" x="252" y="313" width="130" height="30" rx="4"/><text x="317" y="333" text-anchor="middle">Tillgänglighet</text>
<rect class="box" x="394" y="313" width="100" height="30" rx="4"/><text x="444" y="333" text-anchor="middle">Om appen</text>
<rect class="hl" x="20" y="372" width="22" height="16" rx="2"/><text x="50" y="385">MVP (sprint 1–2)</text>
<rect class="box" x="200" y="372" width="22" height="16" rx="2"/><text x="230" y="385">Senare</text>
<rect class="solid" x="320" y="379" width="12" height="9" rx="1"/><path class="line strong" d="M322.5 379V375a3.5 3.5 0 0 1 7 0V379"/><text x="340" y="385">Kräver inloggning</text>
</svg>

Vad teamet lärde sig av att rita den:

- **MVP:n är nio sidor av nitton.** Det går att leverera på två sprintar — resten blir egna [backlog-poster](../begrepp/backlog-och-sprint.md).
- **Varje MVP-sida motsvarar en user story.** *Rumslista* ↔ "Som student vill jag se vilka rum som finns", *Avboka* ↔ "Som student vill jag kunna avboka så att rummet blir ledigt för andra". Saknas en story för en sida — behövs sidan verkligen? Saknas en sida för en story — då har ni glömt något.
- **Integritetspolicyn är med i MVP:n.** Appen sparar namn och bokningar, alltså personuppgifter. Då måste användarna kunna läsa hur uppgifterna hanteras redan från första dagen.
- **"Logga in" ligger utanför trädet** men länkas från startsidan, eftersom alla låsta sidor skickar dit.

## När ska du välja en sitemap?

| Välj sitemap när… | Välj något annat när… |
|-------------------|-----------------------|
| Ni ska bestämma vilka sidor/vyer som behövs | Ni vill förstå hur användaren *rör sig* och känner sig → [Kundresa](kundresa.md) |
| Ni ska planera menyer och navigering | Ni vill visa i vilken ordning sidorna ska byggas → [Roadmap och tidslinje](roadmap-och-tidslinje.md) |
| Ni ska skilja MVP från "senare" | Ni brainstormar fritt om vad appen *kan* innehålla → [Tankekarta](tankekarta.md) |
| Ni gör om en befintlig webbplats | Ni behöver beskriva hur data hänger ihop i databasen (det är ett ER-diagram, inte en sitemap) |

## Vanliga misstag

- **För djupt träd.** Mer än tre nivåer betyder att användaren måste klicka sig djupt för att hitta saker. Platta ut.
- **Sitemap som flödesschema.** Pilar mellan syskon ("sen går man till…") hör inte hemma här.
- **Glömma de tråkiga sidorna.** Felsidor, integritetspolicy, "glömt lösenord", tom-lägen ("du har inga bokningar"). De tar också tid att bygga.
- **Rita teamets organisation istället för användarens behov.** "Säljavdelningen" är ingen bra sektion; "Priser" är det.
- **Rita en gång och glömma.** Uppdatera kartan när en sida läggs till eller stryks — annars ljuger den om omfånget.

## Mall att kopiera

En indenterad lista är en sitemap i textform — snabbt att skriva och lätt att ändra i ett PR.

```text
Startsida
├── Sektion 1                     [MVP]
│   ├── Sida 1.1                  [MVP]  story: #
│   └── Sida 1.2                  [senare]
├── Sektion 2                     [MVP] [inloggning]
│   ├── Sida 2.1                  [MVP]  story: #
│   └── Sida 2.2                  [senare]
└── Sektion 3                     [senare]
Globalt (sidfot): Integritetspolicy [MVP], Tillgänglighet, Kontakt
Utanför trädet: Logga in, Felsida (404)
```

## Övning

Rita en sitemap för er skolas webbplats som den ser ut idag. Hur många nivåer har den? Finns det sidor ni aldrig hittar? Rita sedan om den som ni tycker att den *borde* se ut för en ny student — och markera vilka fem sidor som skulle vara MVP:n.

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Sitemap (planering) | Ett träd över alla sidor — vilka och hur de hänger ihop |
| `sitemap.xml` | En fil åt sökmotorer på en färdig webbplats — något annat |
| Nivå 1 | Sektionerna, oftast huvudmenyn |
| Delad sida | Länkas från alla sidor, t.ex. sidfoten |
| Hänglås | Kräver inloggning |
| MVP-markering | Vilka sidor måste finnas i första leveransen |
