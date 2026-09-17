---
title: V-modellen
parent: Vattenfallsmodellen
nav_order: 20
---

# V-modellen

## Grundidén

V-modellen är en variant av vattenfallsmodellen som gör en sak annorlunda: varje utvecklingsfas kopplas explicit till en motsvarande testfas. Ritad ger det formen av ett V — därav namnet.

```mermaid
flowchart LR
    subgraph Vänster sida — nedåt
    A[Kravanalys] --> B[Systemdesign]
    B --> C[Detaljdesign]
    end
    C --> D[Implementation]
    subgraph Höger sida — uppåt
    E[Enhetstest] --> F[Integrationstest]
    F --> G[Systemtest]
    G --> H[Acceptanstest]
    end
    D --> E
    A -.motsvarar.- H
    B -.motsvarar.- G
    C -.motsvarar.- F
```

## Varje fas har sin testmotsvarighet

| Utvecklingsfas (vänster) | Testfas (höger) |
|---|---|
| Kravanalys | Acceptanstest — testar mot de ursprungliga kraven |
| Systemdesign | Systemtest — testar hela systemet mot arkitekturen |
| Detaljdesign | Integrationstest — testar att komponenter samverkar |
| Implementation | Enhetstest — testar enskild kod |

Poängen: när du skriver kraven, planerar du samtidigt *hur du ska verifiera* att de kraven är uppfyllda — istället för att komma på testfallen först i slutet.

## Jämfört med vanlig vattenfall

V-modellen löser inte vattenfallets grundproblem (sen upptäckt av fel, svårt att hantera ändrade krav) — men den gör en sak bättre: testplanering börjar *samtidigt* som kravställning, inte efteråt. Det minskar risken att viktiga testfall glöms bort eller läggs till som en eftertanke.

## Var används den?

V-modellen är vanlig i branscher med höga krav på spårbarhet och verifiering — inbyggda system, medicinteknik, flyg- och fordonsindustri — där varje krav måste kunna knytas till ett specifikt test som bevisar att det är uppfyllt.
