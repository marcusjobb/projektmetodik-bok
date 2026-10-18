---
title: MoSCoW
description: "MoSCoW-metoden delar krav i fyra kategorier — Must have, Should have, Could have och Won't have — för att tvinga teamet att välja vad som faktiskt krävs för en leverans."
parent: Agilt & Scrum
nav_order: 40
---

# MoSCoW

## Grundidén

I varje projekt finns det fler saker att göra än tid att göra dem. MoSCoW-metoden tvingar teamet att svara på en enkel fråga för varje krav:

**Är det ett måste, eller vill vi bara ha det?**

Svaret hamnar i en av fyra kategorier. Bokstäverna bildar akronymen — vokalerna i mitten är stummade och ger uttalet *Moscow*:

| Bokstav | Kategori | Vad det innebär |
|---------|----------|-----------------|
| **M** | Must have | Utan detta levereras ingenting. Systemet fungerar inte eller affärsmålet uppnås inte. |
| **S** | Should have | Viktiga krav men inte livsavgörande. Kan utelämnas om tid saknas utan att allt rasar. |
| **C** | Could have | Trevliga funktioner — tas med om det finns tid och kapacitet kvar. |
| **W** | Won't have *(this time)* | Erkänt ute ur den här leveransen. Inte ett nej för alltid — ett dokumenterat nej nu. |

<svg class="dg" viewBox="0 0 700 200" role="img" aria-labelledby="moscow-t" xmlns="http://www.w3.org/2000/svg">
<title id="moscow-t">MoSCoW-skalan från vänster till höger: Must have (kritiskt), Should have (viktigt), Could have (trevligt), Won't have (inte nu). Pilarna visar fallande prioritet.</title>
<defs>
<marker id="mc-f" viewBox="0 0 10 10" refX="10" refY="5" markerUnits="userSpaceOnUse" markerWidth="10" markerHeight="10" orient="auto"><path d="M0 0L10 5L0 10z" class="solid"/></marker>
</defs>
<rect class="q1" x="20" y="60" width="145" height="80" rx="6"/>
<rect class="q2" x="185" y="60" width="145" height="80" rx="6"/>
<rect class="q3" x="350" y="60" width="145" height="80" rx="6"/>
<rect class="box" x="515" y="60" width="165" height="80" rx="6"/>
<text x="92" y="95" text-anchor="middle" class="title">M — Must</text>
<text x="92" y="116" text-anchor="middle" class="muted">Kritiskt</text>
<text x="257" y="95" text-anchor="middle" class="title">S — Should</text>
<text x="257" y="116" text-anchor="middle" class="muted">Viktigt</text>
<text x="422" y="95" text-anchor="middle" class="title">C — Could</text>
<text x="422" y="116" text-anchor="middle" class="muted">Trevligt</text>
<text x="597" y="95" text-anchor="middle" class="title">W — Won't</text>
<text x="597" y="116" text-anchor="middle" class="muted">Inte nu</text>
<line class="line strong" x1="20" y1="175" x2="680" y2="175" marker-end="url(#mc-f)"/>
<text x="20" y="195" class="muted">Hög prioritet</text>
<text x="660" y="195" text-anchor="end" class="muted">Låg prioritet</text>
</svg>

## Vad MoSCoW inte är

- Det är inte ett tekniskt verktyg. Det är ett **kommunikationsverktyg**.
- Det ersätter inte en backlog — det hjälper dig prioritera den.
- Det är inte ett sätt att skjuta upp svåra beslut. Won't är ett aktivt val som dokumenteras.

Samtalet om vad som är Must och vad som är Won't är mer värdefullt än den färdiga listan. Där synliggörs antaganden, konflikter och missförstånd mellan kund, Product Owner och team.

## Var används MoSCoW?

- **Kravhantering** inför en sprint eller leverans
- **MVP-beslut** — vad måste vara med i minsta möjliga produkt som ger värde?
- **Databasdesign** — vilka tabeller och relationer behöver finnas nu?
- **Tidsbegränsade projekt** — skoluppgifter, hackathons, kundprojekt med fast deadline

## Exempel — bokningsapp för gym

Gruppen som bygger en bokningsapp har tolv krav och fyra veckor. De kör en MoSCoW-session:

| Krav | Kategori | Motivering |
|------|----------|------------|
| Boka ett pass | **Must** | Appens syfte |
| Se tillgängliga tider | **Must** | Utan detta kan ingen boka |
| Avboka ett pass | **Should** | Viktig men systemet lever utan dag ett |
| Bekräftelsemejl | **Should** | Förväntat av användarna |
| Filtrera på instruktör | **Could** | Trevligt, men man kan scrolla |
| Mörkt läge | **Could** | Efterfrågat men inte avgörande |
| Betalning i appen | **Won't** | För komplex — sparas till version 2 |
| Sociala funktioner | **Won't** | Utanför scope för det här projektet |

Resultatet: teamet vet exakt vad som ska finnas på demo-dagen, och allt annat är satt på is med ett gemensamt beslut.

## Kopplingen till Must → MVP

Must have-kraven är i praktiken din **MVP** (Minimum Viable Product) — det minsta som ger ett fungerande system med värde för användaren.

```
Must have = MVP
Should have = version 1.1
Could have = version 2
Won't have = dokumenterat icke-beslut
```

Se [User stories och MVP](../begrepp/user-story-och-mvp.md) för hur du formulerar kraven som user stories.

## Vanliga misstag

- **Allt är Must.** Om allt är Must har ni inte prioriterat — ni har kopierat kravlistan. Tvinga fram fördelningen: minst 20 % bör vara Should eller lägre.
- **Won't tolkas som nej.** Won't have betyder "inte i den här leveransen" — inte "aldrig". Dokumentera det så kunden förstår att det är ett aktivt beslut, inte ett glömskebort.
- **En person bestämmer.** MoSCoW ska göras i teamet, med kund eller Product Owner med. Annars är det bara en persons gissning.
- **Listan görs en gång.** Prioriteringen ska uppdateras varje sprint eller när scope ändras. En gammal MoSCoW-lista är farligare än ingen.

## Övning

Ta tio krav för ett system ni kan (eller hittar på) och kör en MoSCoW-session i gruppen:

1. Skriv varje krav på en lapp.
2. Alla sorterar tyst var sin lapp — Must, Should, Could, Won't.
3. Jämför. Var hamnade ni olika? Diskutera varför.
4. Kom överens om en gemensam lista.

Målet är inte att listan ska bli perfekt — det är att meningsskiljaktigheten ska synas.

## TL;DR

| Begrepp | Vad det är |
|---------|------------|
| Must have | Leveransen misslyckas utan det |
| Should have | Viktigt men systemet överlever utan det dag ett |
| Could have | Trevligt om tid finns |
| Won't have | Medvetet bortvalt — dokumenterat, inte glömt |
| MVP | = Must have-kraven |
