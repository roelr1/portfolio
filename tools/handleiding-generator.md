---
layout: default
title: Handleiding-generator
---

# Handleiding-generator

## Doel

Tooling om instructiehandleidingen voor Microsoft 365-applicaties te maken op basis van screenshots, met automatische pijlannotaties en een uniforme opmaak in Word. Het doel: elke handleiding ziet er hetzelfde uit, ongeacht wie hem aanlevert.

## Hoe het werkt

1. De auteur maakt screenshots en schrijft de stappen, en markeert daarin het doelwit van elke stap, bijvoorbeeld «Kanalen».
2. De tool plaatst automatisch een pijl op het juiste UI-element, in vaste volgorde van betrouwbaarheid: cursorpositie vlak vóór de klik, OCR-tekstmatch op de doelterm, UI-parsing, en als laatste vallen een vision-model.
3. Screenshots worden genormaliseerd naar één vast formaat zodat alle handleidingen identiek ogen.
4. De oplevering is een .docx met een vaste sjabloon: huisstijl, versieblok, datum en applicatieversie.
5. Altijd menselijke review vóór publicatie; de AI schrijft niet zelfstandig, hij helpt annoteren en taal schonen.

## Techniek

- Python (python-docx voor de Word-oplevering)
- OCR en UI-detectie voor het plaatsen van annotaties
- Uitbreiding onderweg: een gesproken variant (tekst-naar-spraak/avatar) naast de geschreven handleiding, vanuit dezelfde stappen tekst. Dit ondersteunt ook medewerkers met een leesbeperking.

## Status

Werk in uitvoering. Demo met een Teams-handleiding is succesvol; verder uitbouwen vindt plaats naast het dagelijkse werk.

[Terug naar overzicht](../index.html)
