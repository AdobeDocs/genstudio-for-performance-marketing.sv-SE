---
title: Videofunktioner
description: Läs mer om videofunktionen i de attributkategorier som används i GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Videofunktioner

Videofunktionerna representerar distinkta och informativa element, ljud eller mönster i en video som kan analyseras med [!DNL Insights]. Dessa funktioner hjälper till att kategorisera och förstå videoinnehållet, vilket ger mer korrekta och detaljerade insikter. Genom att identifiera olika attribut, t.ex. ljudstämning, musikgenre och objekt, kan AI ge en omfattande analys av videon, vilket ger bättre beslutsunderlag och strategisk utformning.

## Ljudavkänning

Ljudidentifiering i GenStudio for Performance Marketing innebär att analysera ljudspåret i en video för att identifiera olika attribut. Den här avkänningsprocessen avgör ljudets övergripande stämning genom att identifiera de olika typerna av ljud, tagga specifika genrer eller musikkategorier och extrahera nyckelord från tal. Genom att förstå dessa ljudelement kan AI ge djupare insikter i videons innehåll och sammanhang, vilket förbättrar den övergripande analys- och kategoriseringsprocessen.

## Sök efter videofunktioner

**Så här förhandsgranskar du en video och hör ett exempel på ljudet**:

1. I _[!DNL Insights]_väljer du vyn **[!UICONTROL Attributes]**.

1. Ändra tabellvyn genom att välja **[!UICONTROL Video]**.

1. Välj en funktion i listan **[!UICONTROL Attribute category]**. Om du vill se ett ljudexempel väljer du **Musikgenre**.

1. Välj ett attribut för en detaljerad vy av videoklipp som delar den kategorin.

   Kategorin `Music genre` kan till exempel ha `electronic` som attribut.

1. Sidan _Attributinformation_ visar alla videoklipp med det här attributet. Håll muspekaren över valfri video i listan för att starta en videoförhandsvisning.

1. Växla knappen **slå på** (som finns i det nedre vänstra hörnet av en videoförhandsvisning) och lyssna på ljudet i videoförhandsvisningen.

I följande tabell visas de videofunktionskategorier som känns igen av GenStudio for Performance Marketing AI. Den identifierade attributlistan för ett medieinnehåll är inte uttömmande. Media som innehåller en mängd funktioner kan begränsas till de tre dominerande funktionerna som identifieras av AI.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategori | Beskrivning | Exempel |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Ljudläge | Avgör den övergripande känslomässiga tonen eller atmosfären i ljudspåret, till exempel `calm`, `upbeat` eller `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Ljudtyper | Taggar videon med en eller flera typer av ljud, till exempel `music` eller `speech`. | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Kategorier | Videon delas in i en eller flera kategorier med brett innehåll. | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education`, `Sales and offers` |
| Musikkategori | Omfattande klassificering av musikgenre när det finns musik i videon. Detta hjälper till att identifiera den allmänna typen av musik, till exempel `contemporary`- eller `traditional`-stilar. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Musikgenre | Specifik klassificering av musikstil när det finns musik i videon, vilket ger en mer detaljerad identifiering av musiken, till exempel `electronic` eller `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Objekt | Identifierar ett eller flera objekt, enheter och element som visas i videon. | Värdena är för många, men några exempel är: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Orientering | Videons justering i förhållande till dess bredd och höjd. Identifierar om den är bredare än den är hög (liggande), högre än bred (stående) eller lika med bredd och höjd (fyrkant). | `landscape`, `portrait`, `square` |
| Folk | När minst en person är närvarande kan ett eller flera attribut beskriva den eller de personer som är närvarande i videon. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Scener | Identifierar inställningen eller miljön i en video och anger sammanhang för var videon gjordes eller vilken typ av plats som avbildades. | Värdena är för många, men några exempel är: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge` |
| Stilar | Identifierar visuella effekter som används på videoelement, t.ex. de som används i After Effects eller Lightroom. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Taggar | Identifierar andra videoegenskaper som inte omfattas av en viss klassificering. Taggar ger ytterligare kontext och metadata om videon. | Värdena är för många, men några exempel är: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing` |
