---
title: Prioriteringsmatriser
description: "Eisenhowermatrisen och värde/insats-matrisen sorterar uppgifter i fyra rutor så att teamet ser vad som ska göras nu, vad som kan vänta och vad som kan strykas."
parent: Diagram & analysverktyg
nav_order: 100
---

# Prioriteringsmatriser

## Grundidén

När listan med saker att göra är längre än tiden räcker till måste någon välja. En **prioriteringsmatris** gör valet synligt: varje uppgift placeras i ett av fyra fält utifrån två frågor. Här finns de två vanligaste:

- **Eisenhowermatrisen** — frågorna är *är det brådskande?* och *är det viktigt?* Bra för ens egen eller teamets vecka.
- **Värde/insats-matrisen** (*impact/effort*) — frågorna är *hur mycket värde ger det?* och *hur mycket jobb kostar det?* Bra för att prioritera en backlog.

Båda är grova verktyg med flit. De ersätter inte diskussionen — de ger den något att peka på.

## Vad används det till?

- **Prioritera backloggen** inför sprintplaneringen — se [Backlog och sprint](../begrepp/backlog-och-sprint.md)
- **Planera sin egen vecka** — vad gör jag i dag, vad lägger jag in i kalendern?
- **Hitta snabba vinster** — saker som ger mycket för lite jobb
- **Säga nej med gott samvete** — det som hamnar i "Eliminera" eller "Slöseri" stryks

## Delarna och vad de heter — Eisenhowermatrisen

<svg class="dg" viewBox="0 0 720 400" role="img" aria-labelledby="pm1-t" xmlns="http://www.w3.org/2000/svg">
<title id="pm1-t">Eisenhowermatrisen med namngivna delar: fokusområde, brådska-axel, vikt-axel och fyra kvadranter: gör nu, planera, delegera och eliminera</title>
<rect class="box" x="130" y="15" width="410" height="34" rx="4"/>
<text x="335" y="37" text-anchor="middle">Fokusområde: t.ex. sprint 4</text>
<text x="230" y="72" text-anchor="middle" class="title">Brådskande</text>
<text x="440" y="72" text-anchor="middle" class="title">Inte brådskande</text>
<rect class="q1" x="130" y="85" width="200" height="125" rx="4"/>
<rect class="q2" x="340" y="85" width="200" height="125" rx="4"/>
<rect class="q3" x="130" y="220" width="200" height="125" rx="4"/>
<rect class="box" x="340" y="220" width="200" height="125" rx="4"/>
<text x="230" y="140" text-anchor="middle" class="title">1. Gör nu</text>
<text x="230" y="162" text-anchor="middle" class="muted">Gör det i dag</text>
<text x="440" y="140" text-anchor="middle" class="title">2. Planera</text>
<text x="440" y="162" text-anchor="middle" class="muted">Boka in tid för det</text>
<text x="230" y="275" text-anchor="middle" class="title">3. Delegera</text>
<text x="230" y="297" text-anchor="middle" class="muted">Låt någon annan göra det</text>
<text x="440" y="275" text-anchor="middle" class="title">4. Eliminera</text>
<text x="440" y="297" text-anchor="middle" class="muted">Stryk det</text>
<text x="120" y="145" text-anchor="end" class="title">Viktigt</text>
<text x="120" y="280" text-anchor="end" class="title">Inte viktigt</text>
<line class="leader" x1="544" y1="32" x2="560" y2="32"/><text x="566" y="36" class="part">Fokusområde</text>
<line class="leader" x1="510" y1="68" x2="560" y2="68"/><text x="566" y="72" class="part">Brådska-axel</text>
<line class="leader" x1="525" y1="105" x2="560" y2="126"/><text x="566" y="130" class="part">Kvadrant</text>
<line class="leader" x1="60" y1="290" x2="50" y2="370"/><text x="20" y="385" class="part">Vikt-axel</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Fokusområde** | Rubrik överst | Vad listan gäller — en sprint, en vecka, ett projekt |
| **Brådska-axel** | Kolumnerna | *Brådskande* = har en deadline nu eller någon väntar. Säger inget om värdet |
| **Vikt-axel** | Raderna | *Viktigt* = bidrar till målet. Säger inget om när |
| **1. Gör nu** (*Do*) | Viktigt + brådskande | Kriser och deadlines — gör det själv, i dag |
| **2. Planera** (*Schedule*) | Viktigt + inte brådskande | Det som bygger framtiden: tester, dokumentation, lärande. Boka in tid, annars blir det aldrig av |
| **3. Delegera** (*Delegate*) | Inte viktigt + brådskande | Måste göras snart, men inte nödvändigtvis av dig |
| **4. Eliminera** (*Eliminate*) | Inte viktigt + inte brådskande | Stryk det — eller skjut det långt ner i backloggen |

> **Ruta 2 är den viktigaste.** Team som bara jobbar i ruta 1 släcker bränder hela tiden. Det som ligger i ruta 2 — tester, refaktorering, en ordentlig README — är det som gör att det brinner mindre nästa sprint.

## Delarna och vad de heter — värde/insats-matrisen

<svg class="dg" viewBox="0 0 720 395" role="img" aria-labelledby="pm2-t" xmlns="http://www.w3.org/2000/svg">
<title id="pm2-t">Värde/insats-matris med namngivna delar: värdeaxel, insatsaxel, kvadrant och uppgift. Kvadranterna är snabba vinster, stora satsningar, utfyllnad och slöseri</title>
<defs>
<marker id="pm2-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<rect class="q4" x="130" y="60" width="210" height="140" rx="4"/>
<rect class="q2" x="350" y="60" width="210" height="140" rx="4"/>
<rect class="q3" x="130" y="210" width="210" height="140" rx="4"/>
<rect class="q1" x="350" y="210" width="210" height="140" rx="4"/>
<line class="line strong" x1="120" y1="355" x2="120" y2="48" marker-end="url(#pm2-f)"/>
<line class="line strong" x1="120" y1="355" x2="568" y2="355" marker-end="url(#pm2-f)"/>
<text x="235" y="95" text-anchor="middle" class="title">Snabba vinster</text>
<text x="235" y="117" text-anchor="middle" class="muted">Högt värde, liten insats</text>
<text x="455" y="95" text-anchor="middle" class="title">Stora satsningar</text>
<text x="455" y="117" text-anchor="middle" class="muted">Högt värde, stor insats</text>
<text x="235" y="245" text-anchor="middle" class="title">Utfyllnad</text>
<text x="235" y="267" text-anchor="middle" class="muted">Lågt värde, liten insats</text>
<text x="455" y="245" text-anchor="middle" class="title">Slöseri</text>
<text x="455" y="267" text-anchor="middle" class="muted">Lågt värde, stor insats</text>
<circle class="dot" cx="200" cy="160" r="5"/>
<circle class="dot" cx="260" cy="175" r="5"/>
<circle class="dot" cx="500" cy="160" r="5"/>
<circle class="dot" cx="190" cy="305" r="5"/>
<circle class="dot" cx="480" cy="305" r="5"/>
<text x="112" y="72" text-anchor="end" class="muted">Högt</text>
<text x="112" y="210" text-anchor="end" class="title">Värde</text>
<text x="112" y="350" text-anchor="end" class="muted">Lågt</text>
<text x="130" y="375" class="muted">Liten</text>
<text x="345" y="375" text-anchor="middle" class="title">Insats</text>
<text x="560" y="375" text-anchor="end" class="muted">Stor</text>
<text x="20" y="30" class="part">Värdeaxel</text><line class="leader" x1="92" y1="28" x2="116" y2="48"/>
<line class="leader" x1="555" y1="75" x2="574" y2="86"/><text x="580" y="90" class="part">Kvadrant</text>
<line class="leader" x1="506" y1="160" x2="574" y2="161"/><text x="580" y="165" class="part">Uppgift</text>
<line class="leader" x1="568" y1="360" x2="584" y2="374"/><text x="590" y="380" class="part">Insatsaxel</text>
</svg>

| Del | Hur den ritas | Vad den betyder |
|-----|---------------|-----------------|
| **Värdeaxel** (*impact*) | Lodrät axel | Hur mycket nytta uppgiften ger användaren eller kunden |
| **Insatsaxel** (*effort*) | Vågrät axel | Hur mycket jobb den kostar — gärna i story points |
| **Uppgift** | En prick eller lapp | En post i backloggen, placerad där teamet tror att den hör hemma |
| **Snabba vinster** (*quick wins*) | Högt värde, liten insats | Gör först |
| **Stora satsningar** (*major projects*) | Högt värde, stor insats | Planera noga, dela upp i mindre delar |
| **Utfyllnad** (*fill-ins*) | Lågt värde, liten insats | Gör när det blir tid över |
| **Slöseri** (*time wasters*) | Lågt värde, stor insats | Stryk eller tänk om |

## Exempel — bokningsappens backlog

Gruppen som bygger en bokningsapp för gymmet har tolv poster i backloggen och fyra veckor kvar. På sprintplaneringen sätter de upp lapparna på en värde/insats-matris på whiteboarden.

<svg class="dg" viewBox="0 0 720 390" role="img" aria-labelledby="pm3-t" xmlns="http://www.w3.org/2000/svg">
<title id="pm3-t">Värde/insats-matris med åtta backloguppgifter för en bokningsapp, två i varje kvadrant</title>
<defs>
<marker id="pm3-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<rect class="q4" x="130" y="40" width="280" height="150" rx="4"/>
<rect class="q2" x="420" y="40" width="280" height="150" rx="4"/>
<rect class="q3" x="130" y="200" width="280" height="150" rx="4"/>
<rect class="q1" x="420" y="200" width="280" height="150" rx="4"/>
<line class="line strong" x1="120" y1="355" x2="120" y2="28" marker-end="url(#pm3-f)"/>
<line class="line strong" x1="120" y1="355" x2="712" y2="355" marker-end="url(#pm3-f)"/>
<text x="140" y="64" class="title">Snabba vinster</text>
<circle class="dot" cx="150" cy="100" r="5"/><text x="162" y="105">Bekräftelsemejl vid bokning</text>
<circle class="dot" cx="150" cy="140" r="5"/><text x="162" y="145">Avboka-knapp</text>
<text x="430" y="64" class="title">Stora satsningar</text>
<circle class="dot" cx="440" cy="100" r="5"/><text x="452" y="105">Inloggning med konto</text>
<circle class="dot" cx="440" cy="140" r="5"/><text x="452" y="145">Kalendervy för veckan</text>
<text x="140" y="224" class="title">Utfyllnad</text>
<circle class="dot" cx="150" cy="260" r="5"/><text x="162" y="265">Mörkt läge</text>
<circle class="dot" cx="150" cy="300" r="5"/><text x="162" y="305">Ny ikon i menyn</text>
<text x="430" y="224" class="title">Slöseri</text>
<circle class="dot" cx="440" cy="260" r="5"/><text x="452" y="265">Egen chattfunktion</text>
<circle class="dot" cx="440" cy="300" r="5"/><text x="452" y="305">Animationer överallt</text>
<text x="112" y="52" text-anchor="end" class="muted">Högt</text>
<text x="112" y="200" text-anchor="end" class="title">Värde</text>
<text x="112" y="350" text-anchor="end" class="muted">Lågt</text>
<text x="130" y="375" class="muted">Liten</text>
<text x="415" y="375" text-anchor="middle" class="title">Insats</text>
<text x="700" y="375" text-anchor="end" class="muted">Stor</text>
</svg>

Resultatet blir en ordning för backloggen:

1. **Snabba vinster först** — bekräftelsemejl och avboka-knapp tas in i nästa sprint.
2. **Stora satsningar delas upp** — "Kalendervy för veckan" blir tre mindre user stories: visa dagens pass, visa veckan, bläddra framåt.
3. **Utfyllnad hamnar längst ner** — mörkt läge görs om det blir tid över sista veckan.
4. **Slöseri stryks** — chatten tas bort ur backloggen. Om kunden frågar har teamet nu ett tydligt svar på varför.

Samma uppgifter i en **Eisenhowermatris** för Product Owner sista veckan före demo:

| | Brådskande | Inte brådskande |
|---|---|---|
| **Viktigt** | **Gör nu:** Fixa buggen där dubbelbokningar går igenom | **Planera:** Skriv tester för bokningslogiken |
| **Inte viktigt** | **Delegera:** Ta skärmdumpar till demon (någon i teamet) | **Eliminera:** Byta färg på knapparna |

## Mall att kopiera

**Eisenhowermatris**

```markdown
## Eisenhowermatris: <Fokusområde / projekt>

| | Brådskande | Inte brådskande |
|---|---|---|
| **Viktigt** | **Gör nu** (gör det i dag) <br> - | **Planera** (boka in tid) <br> - |
| **Inte viktigt** | **Delegera** (ge till någon annan) <br> - | **Eliminera** (stryk det) <br> - |
```

**Prioriteringslista med matris**

```markdown
## <Titel>

**Tidsram:** <t.ex. sprint 4, v.12–13>
**Mål:** <vad ska vara klart när tiden är slut?>

### Att göra-lista
- [ ]
- [ ]
- [ ]

### Gör direkt
-
### Planera
-
### Delegera (till vem?)
-
### Stryk
-

### Anteckningar
```

**Värde/insats-matris**

```markdown
| | Liten insats | Stor insats |
|---|---|---|
| **Högt värde** | **Snabba vinster** (gör först) <br> - | **Stora satsningar** (dela upp) <br> - |
| **Lågt värde** | **Utfyllnad** (om tid finns) <br> - | **Slöseri** (stryk) <br> - |
```

## När ska du välja vilken?

| Välj… | När… |
|-------|------|
| **Eisenhowermatrisen** | Det handlar om *tid* — vad gör jag eller vi den här veckan? Deadlines spelar roll |
| **Värde/insats-matrisen** | Det handlar om *vad som är värt att bygga* — prioritera en [backlog](../begrepp/backlog-och-sprint.md) eller välja innehåll i en [MVP](../begrepp/user-story-och-mvp.md) |
| Något annat: [SWOT](swot.md) | Ni ska fatta ett större strategiskt beslut, inte sortera uppgifter |
| Något annat: [Venndiagram](venndiagram.md) | Ni vill hitta det som uppfyller flera villkor samtidigt, inte rangordna |

## Vanliga misstag

- **Allt är viktigt och brådskande.** Om ruta 1 är full har ni inte prioriterat — ni har bara flyttat listan. Tvinga fram en fördelning.
- **En person gissar insatsen.** Insats ska uppskattas av dem som gör jobbet, gärna med story points.
- **Matrisen ritas en gång och glöms.** Läget ändras varje sprint. Gör om den på sprintplaneringen.
- **Ingen vågar stryka.** Det som hamnar i "Eliminera" eller "Slöseri" ska faktiskt bort — annars är övningen meningslös.

## Övning

Ta tio poster från en backlog ni har (eller hitta på tio för en bokningsapp). Placera dem i en värde/insats-matris tillsammans i gruppen — var och en uppskattar insatsen först utan att visa de andra. Var hamnade ni olika, och varför?

## TL;DR

| Begrepp | Vad det är |
|---------|-----------|
| Eisenhowermatrisen | Brådskande × viktigt → gör nu / planera / delegera / eliminera |
| Värde/insats-matrisen | Värde × insats → snabba vinster / stora satsningar / utfyllnad / slöseri |
| Snabba vinster | Mycket värde för lite jobb — gör först |
| Ruta 2 (Planera) | Viktigt men inte bråttom — det som oftast glöms |
