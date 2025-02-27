---
title: Attribut - översikt
description: Lär dig hur du utvärderar prestandan för specifika attribut i Adobe GenStudio for Performance Marketing.
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Attribut - översikt

Vyn [!DNL Insights] _[!UICONTROL Attributes]_visar en lista med attribut som används i annonskampanjer för det valda kanalkontot.

{{connect-insights}}

Tabellen _[!UICONTROL Attributes]_är ordnad med namnet [!UICONTROL Attribute]. Du kan växla mellan listtyperna med knappen **[!UICONTROL Images]**och knappen **[!UICONTROL Video]**. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas.

Filterikonen (tratten) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]** där du kan välja mellan [!UICONTROL Account] och [!UICONTROL Attribute category] för att filtrera attributen i tabellen. I följande exempel visas en lista med attribut i kategorin `Lighting Condition`. Klicka på **Återställ** om du vill ta bort alla filterval.

![Attributfilter och tabell](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Attributinformation

Attribut hjälper till att identifiera resurser genom deras inneboende detaljer, som färg, komposition, visuella element och andra egenskaper.

I vyn för attributdetaljer kan du se vilka upplevelser som använder det valda attributet. Detaljerna innehåller totala attributprestanda och en uppdelning av prestandamätningarna för varje upplevelse.

![Attribut för prestandamått](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing identifierar vissa funktioner och använder rätt attribut för en resurs eller upplevelse som en tagg. Se [Kategorier](#categories) om du vill se exempel på de här taggarna. Om du vill visa alla attribut som är kopplade till en upplevelse klickar du på inställningsikonen (cog) ovanför den högra sidan av tabellen för att markera kolumnen **[!UICONTROL Attributes]**.

## Kategorier

En attributkategori är en klassificeringsgrupp som organiserar relaterade attribut som har en gemensam egenskap. Dessa kategorier hjälper till att effektivisera identifiering, identifiering och förståelse av specifika attribut genom att ge ett större sammanhang och underlätta deras tillämpning och användning.

GenStudio for Performance Marketing använder Adobe AI- och maskininlärningsfunktioner för att studera [bilder](image-features.md), [videor](video-features.md) och text och tillämpa [!UICONTROL Asset attributes] baserat på sannolikheten för att de ska vara korrekta.

Den identifierade attributlistan för en resurs är inte uttömmande. Assets som innehåller en mängd funktioner kan begränsas till de tre dominerande funktionerna som identifieras av AI. Följande bild innehåller till exempel flera identifierade bildattribut, inklusive flera objekt, för- och bakgrundsfärger.

![bildresursattribut](/help/assets/category/asset-attributes.png "Toucan-bilden innehåller flera identifierade attribut"){width="300" zoomable="yes"}

>[!INFO]
>
>Du kan inte redigera taggar som identifieras och används automatiskt.

## Attributprestanda

Insikter kan hjälpa er att utvärdera vilka attribut som inspirerar till mer kundengagemang.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Attributes]. Varje mätvärde innehåller en kort definition av vad den avser en mediefil, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en annonskampanj.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribute]** | Attributnamnet. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Category]** | Den [kategori](#categories) som representerar den inbyggda kvaliteten för ett attribut. |  |
| **[!UICONTROL # of images]** | Antalet bilder som har det här attributet. | Antalet i attributtabellen kan vara ett annat än antalet i vyn Attributinformation. Skillnaden kan uppstå om kanalkällan, t.ex. Meta, och GenStudio använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL # of videos]** | Antalet videor som har det här attributet. | Antalet i attributtabellen kan vara ett annat än antalet i vyn Attributinformation. Skillnaden kan uppstå om kanalkällan, t.ex. Meta, och GenStudio använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL Impressions]** | En mängd varje gång en bild eller videor med det här attributet läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med en bild eller video med det här attributet. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i klickningar på bilder eller videor med det här attributet.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kosta för varje tusen annonsvisningar av en bild eller video med det här attributet.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittlig kostnad för att utföra en viss kundåtgärd, t.ex. ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Hjälper till att identifiera attribut som leder till värdefulla kundåtgärder. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad för varje klick på bilder eller videor med det här attributet.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som spenderas från budgeten i förhållande till attribut under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
