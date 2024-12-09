---
title: Skapa tillgängliga mallar
description: Skapa mallar i Adobe GenStudio for Performance Marketing som kan nå ut till fler av er målgrupp och ge en optimal upplevelse.
feature: Templates, Content
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: cc1d750a8a520c793b1b605747c091f8a5f5e1a2
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Skapa tillgängliga mallar

Adobe strävar efter att tillhandahålla en optimal upplevelse för alla målgrupper. Mer information finns i [Tillgänglighetsinitiativ på Adobe](https://www.adobe.com/trust/accessibility/initiatives.html).

I GenStudio for Performance Marketing kan du överföra resurser och mallar som gör det möjligt att skapa innehåll för en mängd olika upplevelser. Genom att följa tillgänglighetsstandarder kan ert innehåll nå er avsedda målgrupp.

Använd följande rekommendationer för att förbereda mallarna med hjälp av optimala tillgänglighetsstandarder.

## Alternativ text

Ange textalternativ för innehåll som inte är text, till exempel bilder.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Idékollage, böcker, man som håller en enorm penna, dator](/help/assets/card-create-assets.png){width="400"}

## Typsnitt

Använd lättlästa teckensnitt. Sans Serif-teckensnitt har till exempel ett rent, blockliknande utseende, vilket gör det lättare att läsa.

Ange en lämplig kontrast mellan text och bakgrund. Undvik att använda teckensnittsfärger som ger mörk text mot mörk bakgrund och ljus text mot ljus bakgrund. Tänk på kontrastriktlinjerna för att få ett optimalt förhållande:

- Text och bilder av text: kontrastförhållande på minst 4,5:1
- Stor text och bilder av storskalig text: kontrastförhållande på minst 3:1

## Länksyfte (endast länk)

Skapa tydlig länktext som beskriver länkens syfte och plats.

Om du till exempel använder länktext som&quot;Klicka här&quot; eller&quot;Läs mer&quot; beskrivs inte syftet med länken tydligt:

```html
<a href="product-site.html">Click here</a>
```

Det bästa sättet är att använda text som tydligt beskriver var länken går. I ett bättre exempel kan namnet på länkkällan och syftet användas:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Språk

Många produkter och tjänster använder språket på ett kreativt eller unikt sätt. Undvik jargon, långa meningar och komplexa fraser. Använd ett tydligt, koncist och lättläst språk som är kompatibelt med målgruppen.

- Använd tydliga beskrivningar, textbundna definitioner eller relaterade exempel när det är möjligt. Det kan vara svårt att översätta ett unikt språk.

- Skriv ut eller länka till en definition för de första förekomsterna av en akronym eller förkortning. Det kan vara svårt att översätta förkortningar.

- Använd visuella element för att komplettera text eller komplexa idéer när det är möjligt.
