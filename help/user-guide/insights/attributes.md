---
title: Attribut - översikt
description: Lär dig hur du utvärderar prestandan för specifika attribut i Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Attribut - översikt

Vyn [!DNL Insights] _[!UICONTROL Attributes]_visar en lista med attribut som används i annonskampanjer för det valda kanalkontot.

{{connect-insights}}

Tabellen _[!UICONTROL Attributes]_är ordnad med namnet [!UICONTROL Attribute]. Du kan växla mellan listtyperna med knappen **[!UICONTROL Images]**och knappen **[!UICONTROL Video]**. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas.

![Attributfilter och tabell](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{filter-table}}

## Attributinformation

Attribut hjälper till att identifiera [annonser](ads.md#ad-details) och [medier](media.md#media-details) med hjälp av deras inneboende detaljer, som färg, komposition, visuella element och andra egenskaper.

I vyn för attributinformation kan du se vilka annonser som använder det valda attributet. Detaljerna innehåller totala attributprestanda och en uppdelning av resultatvärdena för varje annons.

![Attribut för prestandamått](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing identifierar vissa funktioner och använder rätt attribut för mediainnehåll eller annons som en tagg. Exempel på de här taggarna finns i [Kategorier](#categories). Om du vill visa alla attribut som är kopplade till en annons klickar du på inställningsikonen (cog) ovanför den högra sidan av tabellen för att markera kolumnen **[!UICONTROL Attributes]**.

## Kategorier

Ett attribut _kategori_ är en klassificeringsgrupp som organiserar relaterade attribut som delar en gemensam egenskap. Dessa kategorier hjälper till att effektivisera identifiering, identifiering och förståelse av specifika attribut genom att ge ett större sammanhang och underlätta deras tillämpning och användning.

GenStudio for Performance Marketing använder Adobe AI och maskininlärningsfunktioner för att studera [bilder](image-features.md), [videor](video-features.md) och [text](text-features.md) och tillämpa attribut på annonser och media baserat på sannolikheten för att de ska vara korrekta.

Den identifierade attributlistan för annonser och mediainnehåll är inte uttömmande. Innehåll som innehåller en mängd funktioner kan begränsas till de tre dominerande funktionerna som identifieras av AI. Följande bild innehåller till exempel flera identifierade bildattribut, inklusive flera objekt, för- och bakgrundsfärger:

![bildattribut](/help/assets/category/asset-attributes.png "Toucan-bilden innehåller flera identifierade attribut"){width="300" zoomable="yes"}

>[!INFO]
>
>Du kan inte redigera taggar som identifieras och används automatiskt.

## Attributprestanda

Insikter kan hjälpa er att utvärdera vilka attribut som inspirerar till mer kundengagemang.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Attributes]. Varje mätvärde innehåller en kort definition vad gäller attribut, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en annonskampanj.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]** | Attributnamnet. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Category]** | Den [kategori](#categories) som representerar den inbyggda kvaliteten för ett attribut. |  |
| **[!UICONTROL # of images]** | Antalet bilder som har det här attributet. | Antalet i attributtabellen kan vara ett annat än antalet i vyn Attributinformation. Skillnaden kan uppstå om kanalkällan, t.ex. Meta och GenStudio, använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL # of videos]** | Antalet videor som har det här attributet. | Antalet i attributtabellen kan vara ett annat än antalet i vyn Attributinformation. Skillnaden kan uppstå om kanalkällan, t.ex. Meta och GenStudio, använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL Impressions]** | En mängd varje gång en bild eller videor med det här attributet läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med en bild eller video med det här attributet. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i klickningar på bilder eller videor med det här attributet.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kosta för varje tusen annonsvisningar av en bild eller video med det här attributet.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittlig kostnad för att utföra en viss kundåtgärd, t.ex. ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Hjälper till att identifiera attribut som leder till värdefulla kundåtgärder. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad för varje klick på bilder eller videor med det här attributet.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som spenderas från budgeten i förhållande till attribut under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
