---
title: Översikt över media
description: Lär dig hur du utvärderar medieprestanda i Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 817a7bf425732cefd57da55e6bb41154567bca46
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Översikt över media

Vyn [!DNL Insights] _[!UICONTROL Media]_visar en lista över medier som används i annonser och annonskampanjer för det valda kontot._ Media _representerar en bild, video, text eller annat kreativt innehåll som är godkänt för användning i dina marknadsföringssatsningar.

{{connect-insights}}

Tabellen _[!UICONTROL Media]_är ordnad med **[!UICONTROL Media ID]**. Du kan växla mellan vyerna med hjälp av ikonen Visa lista (tabell) och ikonen för gallerivy (stödraster). Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas.

![Mediefilter och tabell](/help/assets/insights-media-filter.png){zoomable="yes"}

I gallerivyn _[!UICONTROL Media]_visas ett kollage med medieförhandsvisningar och ett mått, till exempel klickfrekvens. Klicka på inställningsikonen (cog) ovanför den högra sidan av galleriet för att öppna **[!UICONTROL Card settings]**och växla en av tre mätvärden som kan visas:

- CPA (kostnad per åtgärd)
- CTR (klickfrekvens)
- CPC (kostnad per klick)
- Utgift

{{empty-table}}

## Filtrera media

Filterikonen (trattikonen) ovanför den vänstra sidan öppnar menyn **[!UICONTROL Filter]** där du kan välja från flera listor. Välj **[!UICONTROL Clear all]** ovanför annonstabellen eller galleriet om du vill ta bort alla markerade filter.

Med vissa filter kan du använda exakta nyckelord för att förfina listan med villkor. Nyckelordsfilter är särskilt användbara för kampanjer och annonser som följer en komplex namnkonvention med flera unika identifierare, till exempel följande:

- Namn eller kod för den specifika regionen: `NA`, `EMEA`
- Akronymer för innehållstyp: `EB`, `CHT` eller `DSP`
- Erbjudandekoder eller akronymer: `OFFER2023`, `PROMO`

**Så här filtrerar du efter kampanjer**:

1. Expandera filtret **[!UICONTROL Campaigns]** och klicka på **[!UICONTROL Select]**.
1. Ange nyckelord avgränsade med kommatecken i sökfältet.

   Använd så många nyckelord som behövs för att förfina listan:

   ![Välj kampanjer](/help/assets/insights-select-campaign.png){width=400}

1. Välj en eller flera kampanjer från den resulterande sökningen och klicka på **[!UICONTROL Apply]**.

   Dina valda kampanjer visas nu i listan _[!UICONTROL Filter by]_ovanför annonstabellen eller galleriet, så att du kan fokusera på media som är associerade med de valda kampanjerna.

1. _Valfritt_: Om du vill filtrera media ytterligare utför du ett liknande nyckelordsfilter på **[!UICONTROL Ads]**.

>[!NOTE]
>
>Det använda filtret finns kvar i alla vyer i [!DNL Insights]. Välj **[!UICONTROL Clear all]** ovanför annonstabellen eller galleriet om du vill ta bort alla markerade filter.

### Hämta tabellresultat

{{$include /help/_includes/download-insights.md}}

## Medieinformation

I vyn _Medieinformation_ kan du se vilka annonser som använder de valda medierna. Detaljerna omfattar totala medieprestanda, annonser som använder media, användardefinierade attribut och AI-identifierade funktioner som är kopplade till mediet.

![Medieinformation](/help/assets/insights-media-details.png){zoomable="yes"}

### Medieattribut

{{$include /help/_includes/generated-attributes.md}}

## Medieprestanda

Insikter kan hjälpa er att utvärdera vilka medier som bidrar till framgången för en kampanj och vilka medieattribut som är mest effektiva.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Media]. Varje mätvärde innehåller en kort definition vad gäller media, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Media ID]** | Namnet som är associerat med en bild, video, text eller annat kreativt innehåll. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Impressions]** | Antal varje gång mediet läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med ett klickbart element, till exempel en länk, på mediet. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i medieklickningar i en annons.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att mediet är mycket relevant och engagerande för publiken. Det tyder på att meddelanden och design effektivt fångar publikens intresse och får dem att vidta åtgärder. En hög CTR kan dessutom antyda att medierna är välinriktade och får genklang hos den avsedda målgruppen, vilket leder till bättre övergripande kampanjresultat. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Den genomsnittliga kostnaden för varje tusen mediepresentationer.<br>**Beräkning**: totalt belopp `spent` dividerat med antalet visningar, multiplicerat med 1000 | Ett lågt CPM-värde kan indikera kostnadseffektiva mediaprestanda, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittlig kostnad för att utföra en viss kundåtgärd, t.ex. ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Hjälper till att identifiera medier som resulterar i värdefulla kundåtgärder. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad för varje klick på mediet.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som spenderas från budgeten i förhållande till enskilda medier under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
| **[!UICONTROL Used in these ads]** | Antalet annonser som använder mediet. | |
| **Attribut** | Lista över inbyggda funktioner i mediet. | Attribut hjälper er att identifiera kreativa element som intresserar er bäst. |
