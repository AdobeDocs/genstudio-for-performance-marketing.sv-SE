---
title: Översikt över media
description: Lär dig hur du utvärderar medieprestanda i Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 9c4df8d5b9e45d0c26bee8db9085e3ad21b02742
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Översikt över media

Vyn [!DNL Insights] _[!UICONTROL Media]_visar en lista över medier som används i annonser och annonskampanjer för det valda kontot._ Media _representerar en bild, video, text eller annat kreativt innehåll som är godkänt för användning i dina marknadsföringssatsningar.

{{connect-insights}}

Tabellen _[!UICONTROL Media]_är ordnad med **[!UICONTROL Media ID]**. Du kan växla mellan vyerna med hjälp av ikonen Visa lista (tabell) och ikonen för gallerivy (stödraster). Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas. Filterikonen (trattikonen) ovanför den vänstra sidan av tabellen öppnar menyn **[!UICONTROL Filter]**där du kan välja från flera listor. Markera **[!UICONTROL Clear all]**ovanför tabellen om du vill ta bort alla filter.

![Mediefilter och tabell](/help/assets/insights-media-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

I gallerivyn _[!UICONTROL Media]_visas ett kollage med medieförhandsvisningar och ett mått, till exempel klickfrekvens. Klicka på inställningsikonen (cog) ovanför den högra sidan av galleriet för att öppna **[!UICONTROL Card settings]**och växla en av tre mätvärden som kan visas:

- CPA (kostnad per åtgärd)
- CTR (klickfrekvens)
- CPC (kostnad per klick)
- Utgift

## Medieinformation

I vyn _Medieinformation_ kan du se vilka annonser som använder de valda medierna. Detaljerna omfattar totala medieprestanda, annonser som använder media, användardefinierade attribut och AI-identifierade funktioner som är kopplade till mediet.

![Medieinformation](/help/assets/insights-media-details.png){zoomable="yes"}

## Medieprestanda

Insikter kan hjälpa er att utvärdera vilka medier som bidrar till framgången för en kampanj och vilka medieattribut som är mest effektiva.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Media]. Varje mätvärde innehåller en kort definition vad gäller media, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Media ID]** | Namnet som är associerat med en bild, video, text eller annat kreativt innehåll. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Impressions]** | Antal varje gång mediet läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med ett klickbart element, till exempel en länk, på mediet. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i medieklickningar i en annons.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att mediet är mycket relevant och engagerande för publiken. Det tyder på att meddelanden och design effektivt fångar publikens intresse och får dem att vidta åtgärder. En hög CTR kan dessutom antyda att medierna är välinriktade och får genklang hos den avsedda målgruppen, vilket leder till bättre övergripande kampanjresultat. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kostnad för varje tusen mediemått.<br>**Beräkning**: totalt belopp `spent` dividerat med antalet visningar, multiplicerat med 1000 | Ett lågt CPM-värde kan indikera kostnadseffektiva mediaprestanda, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittlig kostnad för att utföra en viss kundåtgärd, t.ex. ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Hjälper till att identifiera medier som resulterar i värdefulla kundåtgärder. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad för varje klick på mediet.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som spenderas från budgeten i förhållande till enskilda medier under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
| **[!UICONTROL Used in these ads]** | Antalet annonser som använder mediet. | |
| **[!UICONTROL Attributes]** | En lista över attribut som har identifierats och tillämpats på mediet. | |
