---
title: User story och MVP
description: "En kort beskrivning av en funktion ur användarens perspektiv — inte en teknisk kravspecifikation."
parent: Begrepp & artefakter
nav_order: 20
---

# User story och MVP

## User story

En kort beskrivning av en funktion ur **användarens perspektiv** — inte en teknisk kravspecifikation. Standardformen:

> Som **[roll]** vill jag **[göra något]** så att **[nytta]**.

**Exempel:** "Som kund vill jag kunna spara mitt kort så att jag slipper knappa in kortnumret vid varje köp."

Formen tvingar fram *varför* något ska byggas, inte bara *vad*. Det gör det lättare för teamet att avgöra om en lösning faktiskt löser problemet, eller bara tekniskt uppfyller en instruktion.

### Story point

Ett relativt mått på hur komplex eller tidskrävande en user story är — används för att uppskatta arbete istället för att gissa exakta timmar. Poängen jämförs mot varandra ("den här är dubbelt så komplex som den där"), inte mot en absolut tidsenhet. Vanlig skala: Fibonacci-liknande tal (1, 2, 3, 5, 8, 13...) eftersom det tvingar fram tydliga skillnader mellan uppskattningarna istället för falsk precision (är något verkligen "6" och inte "7"?).

## MVP — Minimum Viable Product

Den minsta versionen av en produkt som är **användbar nog** för att testa en idé på riktiga användare — inte den minsta versionen som är tekniskt möjlig att bygga, utan den minsta som faktiskt löser användarens problem.

```mermaid
flowchart LR
    A["Fel tolkning:\nen trasig bilhalva"] -.- B["Rätt tolkning:\nen enkel men hel skateboard,\nsedan cykel, sedan bil"]
```

Klassiskt exempel: om målet är en bil, är en MVP inte "halva en bil" (odugligt för alla) — det är en skateboard (fungerar, löser transportbehovet i miniatyr, ger riktig feedback att bygga vidare på).

### Varför bygga en MVP istället för hela produkten på en gång?

- Du vet om idén faktiskt löser ett problem **innan** du investerat allt
- Riktiga användare ger feedback som ingen intern diskussion kan ersätta
- Om idén var fel, har du bara förlorat tiden det tog att bygga MVP:n — inte hela projektet

## Hur hänger de ihop?

En MVP byggs oftast av ett litet antal user stories — de som tillsammans utgör den minsta kompletta upplevelsen. Story points används för att uppskatta hur mycket arbete det är, vilket i sin tur avgör hur mycket som får plats i varje sprint (se [Backlog och Sprint](backlog-och-sprint.md)).
