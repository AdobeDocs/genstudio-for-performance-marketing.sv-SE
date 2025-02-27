---
title: Assets - översikt
description: Lär dig hur du utvärderar resursprestanda i Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Assets - översikt

Vyn [!DNL Insights] _[!UICONTROL Assets]_visar en lista över resurser som används i upplevelser och annonskampanjer för det valda kanalkontot.

{{connect-insights}}

Tabellen _[!UICONTROL Assets]_är ordnad med [!UICONTROL Asset ID]. Du kan växla mellan vyerna med hjälp av ikonen Visa lista (tabell) och ikonen för gallerivy (stödraster). Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas. Filterikonen (trattikonen) ovanför den vänstra sidan av tabellen öppnar menyn **[!UICONTROL Filter]**där du kan välja från flera listor. Klicka på&#x200B;**Återställ**om du vill ta bort alla filterval.

![Assets-filter och tabell](/help/assets/insights-assets-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

I gallerivyn _[!UICONTROL Assets]_visas ett kollage med förhandsvisningar av resurser och ett mått, till exempel klickfrekvens. Klicka på inställningsikonen (cog) ovanför den högra sidan av galleriet för att öppna **[!UICONTROL Card settings]**och växla en av tre mätvärden som kan visas:

- CPA (kostnad per åtgärd)
- CTR (klickfrekvens)
- CPC (kostnad per klick)
- Utgift

## Resursinformation

En _resurs_ är en bild, video, text eller annat kreativt innehåll som är godkänt för användning i dina marknadsföringssatsningar.

I vyn med resursinformation kan du se vilka upplevelser som använder den valda resursen. Detaljer omfattar totala prestanda för tillgångar, användardefinierade attribut och AI-identifierade funktioner som är kopplade till resursen.

![Resursinformation](/help/assets/insights-asset-details.png){zoomable="yes"}

## Resultat

Insikter kan hjälpa er att utvärdera vilka resurser som bidrar till framgången för en kampanj och vilka resursattribut som är mest effektiva.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Assets]. Varje mätvärde innehåller en kort definition av en tillgång, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en tillgång.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Asset ID]** | Namnet som är associerat med resursen. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Impressions]** | Antal varje gång resursen läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med ett klickbart element, till exempel en länk, på resursen. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i tillgångsklick inom en upplevelse.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och engagerande för publiken. Det tyder på att meddelanden och design effektivt fångar publikens intresse och får dem att vidta åtgärder. En hög CTR kan dessutom antyda att resursen är välriktad och svarar mot den avsedda målgruppen, vilket leder till bättre övergripande kampanjresultat. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kostnad för ett tusen annonsexponeringar.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittlig kostnad för att utföra en viss kundåtgärd, t.ex. ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Hjälper till att identifiera resurser som resulterar i värdefulla kundåtgärder. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad som är associerad med varje klick på en resurs.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som spenderas från budgeten i dess förhållande till enskilda tillgångar under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
| **[!UICONTROL Experiences count]** | Antalet upplevelser som använder resursen. | |
| **[!UICONTROL Attributes]** | En lista över attribut som har identifierats och tillämpats på den här resursen. | |
