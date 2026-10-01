---
title: Diagram & analysverktyg
description: "Diagram och mallar för team och projekt — processkartor, kundresor, tidsplaner, organisationsscheman, SWOT, prioriteringsmatriser, rotorsaksanalys och grafer för uppföljning."
nav_order: 35
has_children: true
---

# Diagram & analysverktyg

Ett diagram i ett projekt har ett enda jobb: att få människor att **förstå samma sak**. Det kan vara en kund som ska se hur ett ärende vandrar genom organisationen, ett team som ska enas om vad som ska göras först, eller en styrgrupp som vill veta om sprinten håller.

De här verktygen handlar om arbetet, människorna och besluten runt systemet. Diagram för själva koden — klassdiagram, sekvensdiagram, ER-diagram, arkitektur — finns i [C#-boken](https://marcusjobb.github.io/programmering-csharp/diagram/).

## Vilket verktyg ska vi välja?

Börja med frågan: **vad behöver vi förstå just nu?**

<svg class="dg" viewBox="0 0 720 430" role="img" aria-labelledby="pmi-t" xmlns="http://www.w3.org/2000/svg">
<title id="pmi-t">Översikt: sex behov — processer, planering, organisation, idéer, beslut och uppföljning — med diagramtyperna som passar varje behov</title>
<text x="10" y="28" class="title">Vad behöver teamet förstå?</text><text x="250" y="28" class="muted">→ verktyg som passar</text>
<rect class="q2" x="10" y="50" width="172" height="48" rx="6"/><text x="96" y="79" text-anchor="middle" class="title">Processflöden</text>
<line class="line" x1="182" y1="74" x2="200" y2="74"/>
<rect class="box" x="200" y="57" width="167" height="34" rx="17"/><text x="284" y="79" text-anchor="middle">BPMN och simbanor</text>
<rect class="box" x="377" y="57" width="92" height="34" rx="17"/><text x="423" y="79" text-anchor="middle">Kundresa</text>
<rect class="q4" x="10" y="112" width="172" height="48" rx="6"/><text x="96" y="141" text-anchor="middle" class="title">Planering</text>
<line class="line" x1="182" y1="136" x2="200" y2="136"/>
<rect class="box" x="200" y="119" width="234" height="34" rx="17"/><text x="317" y="141" text-anchor="middle">Roadmap, tidslinje, Gantt</text>
<rect class="box" x="444" y="119" width="84" height="34" rx="17"/><text x="486" y="141" text-anchor="middle">Sitemap</text>
<rect class="q3" x="10" y="174" width="172" height="48" rx="6"/><text x="96" y="203" text-anchor="middle" class="title">Organisation</text>
<line class="line" x1="182" y1="198" x2="200" y2="198"/>
<rect class="box" x="200" y="181" width="184" height="34" rx="17"/><text x="292" y="203" text-anchor="middle">Organisationsschema</text>
<rect class="hl" x="10" y="236" width="172" height="48" rx="6"/><text x="96" y="265" text-anchor="middle" class="title">Jämföra idéer</text>
<line class="line" x1="182" y1="260" x2="200" y2="260"/>
<rect class="box" x="200" y="243" width="109" height="34" rx="17"/><text x="254" y="265" text-anchor="middle">Tankekarta</text>
<rect class="box" x="319" y="243" width="117" height="34" rx="17"/><text x="378" y="265" text-anchor="middle">Venndiagram</text>
<rect class="q1" x="10" y="298" width="172" height="48" rx="6"/><text x="96" y="327" text-anchor="middle" class="title">Beslut och analys</text>
<line class="line" x1="182" y1="322" x2="200" y2="322"/>
<rect class="box" x="200" y="305" width="59" height="34" rx="17"/><text x="230" y="327" text-anchor="middle">SWOT</text>
<rect class="box" x="269" y="305" width="200" height="34" rx="17"/><text x="369" y="327" text-anchor="middle">Prioriteringsmatriser</text>
<rect class="box" x="479" y="305" width="92" height="34" rx="17"/><text x="525" y="327" text-anchor="middle">5 Varför</text>
<rect class="box" x="581" y="305" width="101" height="34" rx="17"/><text x="632" y="327" text-anchor="middle">SMART-mål</text>
<rect class="q2" x="10" y="360" width="172" height="48" rx="6"/><text x="96" y="389" text-anchor="middle" class="title">Uppföljning</text>
<line class="line" x1="182" y1="384" x2="200" y2="384"/>
<rect class="box" x="200" y="367" width="159" height="34" rx="17"/><text x="280" y="389" text-anchor="middle">Diagram för data</text>
<rect class="box" x="369" y="367" width="167" height="34" rx="17"/><text x="452" y="389" text-anchor="middle">Retro och standup</text>
</svg>

| Vi behöver… | Välj | Typisk situation |
|-------------|------|------------------|
| Se hur ett arbete går mellan personer och avdelningar | [BPMN och simbanor](bpmn-och-simbanor) | "Var fastnar supportärendena?" |
| Förstå användarens upplevelse, steg för steg | [Kundresa](kundresa) | "Varför avbryter folk bokningen?" |
| Planera vilka sidor en webbplats ska ha | [Sitemap](sitemap) | Innan wireframes och user stories |
| Visa vad som händer när | [Roadmap, tidslinje och Gantt](roadmap-och-tidslinje) | Projektplan, LIA-planering, release-plan |
| Visa vem som ansvarar för vad | [Organisationsschema](organisationsschema) | Ny i bolaget, nytt projekt |
| Samla idéer kring ett ämne | [Tankekarta](tankekarta) | Brainstorm vid projektstart |
| Se vad två eller tre saker har gemensamt | [Venndiagram](venndiagram) | Jämföra metoder, hitta MVP |
| Bedöma ett läge inför ett beslut | [SWOT](swot) | "Ska vi satsa på det här?" |
| Bestämma vad som ska göras först | [Prioriteringsmatriser](prioriteringsmatriser) | Backlog, att-göra-lista som växer |
| Hitta orsaken bakom ett problem | [5 Varför](fem-varfor) | Efter en incident eller ett misslyckat release |
| Formulera ett mål som går att följa upp | [SMART-mål](smart-mal) | Sprintmål, personliga lärandemål |
| Följa upp och visa siffror | [Diagram för data](diagram-for-data) | Burndown, velocity, rapport till kund |
| Reflektera och synka i teamet | [Retro och standup](retro-och-standup) | Varje sprint, varje dag |

## Tre tumregler

1. **Rita tillsammans.** Ett diagram som teamet har ritat ihop vid en whiteboard är värt mer än ett snyggt som en person gjort ensam.
2. **Ett diagram — en fråga.** Försöker du visa allt i samma bild visar du ingenting.
3. **Mallen är en start, inte ett facit.** Ta bort rutor som inte hjälper er och lägg till det som saknas.
