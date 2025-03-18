---
title: Förbered en e-postmall för Adobe GenStudio for Performance Marketing
description: Lär dig hur du skapar en anpassad e-postmall för Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
hidefromtoc: true
recommendations: noCatalog
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Förbered e-postmall för Adobe GenStudio for Performance Marketing

Vanligtvis skapar en designer den visuella designen för en mall i ett designprogram som Adobe XD. När du har utformat, kodat och testat en e-postmall kan du förbereda den för överföring och användning i GenStudio for Performance Marketing.

Se [Mallelement](use-templates.md#template-elements).

## Lägg till riktlinjer

Innan du förbereder en mall för Meta-annonser måste du se till att du har lagt till [riktlinjer](/help/user-guide/guidelines/overview.md) i din GenStudio for Performance Marketing och fyllt i dem med omfattande information om relevanta varumärken. [varumärkesriktlinjerna](/help/user-guide/guidelines/brands.md) påverkar det genererade innehållet direkt.

**Exempel**: Om du vill att brödtexten i en e-postmall inte ska vara längre än 500 tecken lägger du till det kravet i [kanalriktlinjerna](/help/user-guide/guidelines/brands.md#channel-guidelines) för fältet&quot;brödtext&quot;.

Om inga riktlinjer läggs till i GenStudio for Performance Marketing används standardvärden.

## Koda en e-postmall

När en mall har designats kodas den med HTML och infogad CSS. Koden ska vara ren och responsiv för olika enheter.

Se [Mallexempel](/help/user-guide/content/customize-template.md#template-examples).

### E-post med flera avsnitt

Du kan använda [strukturerade uppmaningar](/help/user-guide/effective-prompts.md#structured-prompts) under innehållsgenereringen för att instruera GenStudio for Performance Marketing att generera varierande innehåll per avsnitt i ett e-postmeddelande.

Om avsnitten i din e-postmall till exempel har prefixet `Pod`—`Pod1` och `Pod2` kan den strukturerade prompten för innehållsgenerering innehålla specifika direktiv för de e-postavsnitten. GenStudio for Performance Marketing matchar det avsnittsspecifika direktivet i din uppmaning till det relaterade e-postavsnittet och genererar innehåll som är anpassat till direktiven.

Se [Strukturerade uppmaningar](/help/user-guide/effective-prompts.md#structured-prompts).

## Testa en e-postmall

Använd din e-postleverantör eller korrekturplattform för att testa din e-post och verifiera att den återges korrekt på olika e-postklienter och enheter.

Testa om e-postmallen uppfyller följande:

* Layouten justeras för olika skärmstorlekar med CSS-mediefrågor
* Knapparna går att klicka på och navigerar till den avsedda platsen
* E-postmallen kan läsas och användas på mobila enheter

## Definiera genererade innehållsområden

Definiera de områden i e-postmallen som ska fyllas i dynamiskt med innehåll från GenStudio for Performance Marketing.

Så här definierar du genererade innehållsområden:

* Identifiera textelementen i mallen som GenStudio for Performance Marketing ska generera automatiskt, till exempel rubriken eller CTA.
* Anpassa din HTML-mall genom att infoga platshållare i den med hjälp av syntaxen Handlebars.

Se [Platshållare för innehåll](/help/user-guide/content/customize-template.md#content-placeholders).

## Förhandsgranska mallen

Styr hur specifika innehållsområden ska visas med inbyggda stödfunktioner. Du kan till exempel inkludera spårningsparametrar till länkar i en exporterad mall samtidigt som du behåller rena förhandsgranskningslänkar.

Se [Förhandsvisning av mall](/help/user-guide/content/customize-template.md#template-preview).

## Överför och använd mall

När mallen har designats, kodats, testats och förhandsgranskats kan du överföra den till GenStudio for Performance Marketing för att använda den för att generera helt nytt marknadsföringsmaterial.

Se [Arbeta med mallar](use-templates.md).
