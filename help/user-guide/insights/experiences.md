---
title: Översikt över upplevelser
description: Se en översikt över kundengagemang, budget och utgifter för upplevelser och annonsplacering i Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences
source-git-commit: 87a8833549569aaeaa60f5760b4e9a8b710a6033
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Översikt över upplevelser

I vyn [!DNL Insights] _[!UICONTROL Experiences]_visas en lista med upplevelser för det anslutna kanalannonskontot. För Facebook är upplevelserna Meta-annonsnamn.

Tabellen _[!UICONTROL Experiences]_är ordnad med [!UICONTROL Ad names]. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas. Filterikonen (trattikonen) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]**där du kan välja i listorna [!UICONTROL Account] och [!UICONTROL Campaign] för att filtrera annonsnamnen i tabellen.

![Upplevelsfilter och tabell](/help/assets/insights-experiences-filter.png){zoomable="yes"}

## Upplevelseinformation

En _upplevelse_ är en marknadsföringsresurs som innehåller visuellt och interaktivt innehåll som är avsett för distribution till en viss målgrupp som en del av en marknadsföringskampanj.

Välj en upplevelse (annonsnamn) och visa prestandamått, textattribut och placeringar som är kopplade till varje annons. I detaljvyn kan ni analysera en upplevelses statistik utifrån dess annonsplacering och marknadsföring inom ett visst datumintervall.

Detaljvyn innehåller ett helhetsmått för annonsen `click-through rate`, `cost per action` och `spend` - hur mycket av budgeten som har använts i annonsen. Eftersom annonser kan ha flera placeringar, t.ex. en feed eller en banner, kan du se en uppdelning av samma mätvärden för varje annonsplacering. Använd vänster- och högerpilarna under **[!UICONTROL Performance by ad placement]** för att bläddra igenom placeringsmåtten.

![Lägg till information med mått och annonsplaceringar](/help/assets/insights-experience-details.png){zoomable="yes"}

### Textattribut

Under förhandsgranskningen av upplevelsen finns en lista med [!UICONTROL Text attributes] som är associerad med annonsen. När resurser och upplevelser har godkänts och lagrats i [!DNL Content] genererar GenStudio for Performance Marketing taggar baserat på deras inneboende funktioner. Mer information om systemmetadata finns i [Resursinformation](../content/asset-details.md#system-metadata).

### Annonsplaceringar

När du skapade en kampanj med Meta-annonser kan du ha valt var annonserna ska köras baserat på kampanjens [mål](channels.md#objectives). Annonsplaceringar breddar räckvidden för era annonser.

GenStudio for Performance Marketing har stöd för annonsformat som resursflöden, länkannonser och en enda bild eller video. Nedan följer en lista över annonsformat per plattform:

| Instagram | Facebook/Meta | Messenger | Målgruppsnätverk |
| ------------ | ---------------- | ------------ | ---------------- |
| Utforska<br>Utforska startsidan<br>Utforska startsidan för stödraster<br>Feed<br>Reels<br>Profilfeed<br>Sök<br>Handla<br>Artiklar | Business Explore<br>Feed<br>Video i strömmen<br>Marketplace<br>Reels<br>Reels Overlay<br>Right column<br>Search results<br>Stories<br>Video Feeds<br>Ads on Facebook Reels | Inkorg<br>artiklar | Intern video, banderoll och interstitiell<br>återgiven video |

## Mätvärden för upplevelser

Insikter kan hjälpa er att utvärdera vilka upplevelser som bidrar till framgången för en kampanj och vilka annonsplaceringar som är mest effektiva.

<!-- For example, -->

### Mätvärdesdetalj

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Experiences]. Varje mätvärde innehåller en kort definition av annonsnamn, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en upplevelse.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Experience name]** | En lista över upplevelser för det anslutna kanalkontot. Filtrera annonser genom att välja en kampanj. | Sortera upplevelselistan genom att klicka på någon av nyckelmätarna. |
| **[!UICONTROL Campaign]** | En kampanj är en uppsättning upplevelser som utformats för att uppnå ett visst mål. | |
| **[!UICONTROL Placements]** | Antal annonser [praktik](#ad-placements), platser där en upplevelse påträffades i kampanjen. | Placeringar ökar publikens räckvidd. |
| **[!UICONTROL Assets]** | Antal resurser som används i annonsen eller upplevelsen. | |
| **[!UICONTROL Impressions]** | Antal varje gång annonsplaceringen eller upplevelsen läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du överväga andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antal gånger som användare interagerar med ett klickbart element, t.ex. en länk eller en knapp för att ringa upp, på en upplevelseplacering. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av intryck som resulterade i klickningar på upplevelseplaceringen i en kampanj.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kostnad ($) för var tusende annonsexponeringar för upplevelseplacering.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittskostnad ($) som använts för att utföra en viss kundåtgärd, till exempel ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Använd för att övervaka utgifter för upplevelser som resulterar i värdefulla kundaktiviteter. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittskostnad ($) som associeras med varje klick på en upplevelseplacering.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp ($) som använts från budgeten under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra utgiftsbeloppet mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
