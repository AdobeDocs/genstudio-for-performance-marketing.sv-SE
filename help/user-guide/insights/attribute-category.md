---
title: Attributkategorier
description: Läs mer om attributkategorier som används i GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
last-substantial-update: 2024-11-11T00:00:00Z
exl-id: c3b51ef2-56ac-4dd8-98b7-79185b5998d0
source-git-commit: 976358742e598b55b1f0c4ca4664d2bcd8f1e9b9
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Attributkategorier

En attributkategori är en klassificeringsgrupp som organiserar relaterade attribut som har en gemensam egenskap. Dessa kategorier hjälper till att effektivisera identifiering, identifiering och förståelse av specifika attribut genom att ge ett större sammanhang och underlätta deras tillämpning och användning.

GenStudio for Performance Marketing använder Adobe AI- och maskininlärningsfunktioner för att studera bilder, videor och text och tillämpar [!UICONTROL Asset attributes] baserat på sannolikheten för att de är korrekta. Attributlistan för en tillgång är inte uttömmande. Assets som innehåller en mängd funktioner kan begränsas till de tre dominerande funktionerna som identifieras av AI.

## Bildfunktioner

Bildfunktioner representerar distinkta och informativa element eller mönster i en bild som används för analys med [!DNL Insights]. I följande tabell visas de bildfunktionskategorier som känns igen av GenStudio for Performance Marketing AI.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategori | Beskrivning | Exempel |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Kameravinkel | Kamerans placering och vinkel i förhållande till motivet. |                                                                                                                                                                                |
| Objektets avstånd | Avståndet mellan kameran och motivet i en bild. | `close up`, `mid shot`, `long shot` |
| Kamerainställning | Konfigurationen av kamerans kontroller för att skapa bilden. |                                                                                                                                                                                |
| Färg och ton | Utvärderar färger som används i bildelement. Identifierar en till tre färger från en uppsättning med 40 förbestämda färger i följande bildlager:<br>**[!UICONTROL Foreground colors]**- element i bildens<br>**[!UICONTROL Background colors]** främre lager - element i bildens baksta lager | Färgvärden: `Red`, `Dark_Red`, `Green`, `Bright_Green`, `Dark_Green`, `Light_Green`, `Mud_Green`, `Blue`, `Dark_Blue`, `Light_Blue`, `Royal_Blue`, `Black`, `White`, `Off_White`, `Gray`, `Dark_Gray`, `Silver`, `Cream`, `Magenta`, {11 9}, `Yellow`, `Cyan`, `Mustard`, `Khaki`, `Brown`, `Dark_Brown`, `Violet`, `Pink`, `Dark_Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald` `Orange` 36}, `Beige`, `Lilac`, `Olive` |
| Färgtemperatur | Beskriver den allmänna värmen eller färheten för färgerna i bilden. | Ton- eller temperaturvärden: `warm`, `cool`, `neutral`<br>![färger och svala toner](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Bildformat | Visuell behandling av en bild. |                                                                                                                                                                                |
| Ljusvillkor | Typ av ljus i en bild. |                                                                                                                                                                                |
| Objekt | Identifierar ett eller flera objekt, enheter och element som utgör bilden. | ![solros, plan, blomobjekt](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Orientering | Bildens position i förhållande till proportionerna. | `landscape`, `portrait`, `square` |
| Folk | När det finns minst en person kan ett eller flera attribut beskriva personen eller personerna i bilden. | ![kvinnlig person som dansar](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Fotografigenrer | Identifierar motivet och tekniken som används för att hämta en bild, till exempel `abstract` eller `landscape` (inte detsamma som liggande orientering). |           |
| Scener | Identifierar inställningen eller miljön som avbildas i en bild. |                                             |
| Taggar | Identifierar objekt, element och andra bildegenskaper som inte omfattas av en viss klassificering. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Videofunktioner

Bildfunktionerna representerar distinkta och informativa element, ljud eller mönster i en video för analys med [!DNL Insights]. I följande tabell visas de videofunktionskategorier som känns igen av GenStudio for Performance Marketing AI.

| Kategori | Beskrivning | Exempel |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Ljudgenre | När det finns musik kan videon få en klassificering av musikstil, till exempel `electronic` eller `classical`. |          |
| Kategori för ljudgenre | När musik finns kan videon få en bred klassificering av musikgenre, som `acoustic` eller `traditional`. |          |
| Ljudläge | Beskriver den allmänna atmosfären eller tonen i ljudet, till exempel `relaxing` eller `energetic`. |          |
| Ljudtyper | När det finns ljud kan videon få en tagg för en eller flera ljudtyper, som `music` eller `speech`. |          |
| Objekt | Identifierar ett eller flera objekt, enheter och element som visas i videon. | ![objekt i video](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Orientering | Videons position i förhållande till bildrutans proportioner. | `landscape`, `portrait`, `square` |
| Folk | När det finns minst en person kan ett eller flera attribut beskriva personen eller personerna i videon. |        |
| Scener | Inställningen eller miljön som visas i videon. |        |
| Stilar | Identifierar visuella bearbetningar som används för element i videon, till exempel `matte` eller `neon`. |        |
| Taggar | Identifierar objekt, element och andra videoegenskaper som inte omfattas av en viss klassificering. |        |

## Textfunktioner

Textfunktioner inkluderar antal för vissa textelement, t.ex. ord, meningar, känslolägesikoner och klassificeringar för semantik, känslor och ton som används för analys med [!DNL Insights]. Texten kan också få ett läsbarhetspoäng. Kommer snart.

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
