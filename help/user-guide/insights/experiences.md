---
title: Översikt över upplevelser
description: Se en översikt över kundengagemang, budget och utgifter för upplevelser och annonsplacering i Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 0%

---

# Översikt över upplevelser

I vyn [!DNL Insights] _[!UICONTROL Experiences]_visas en lista med upplevelser för det anslutna kanalannonskontot. För Facebook är upplevelserna Meta-annonsnamn.

{{connect-insights}}

Tabellen _[!UICONTROL Experiences]_är ordnad med [!UICONTROL Ad names]. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas. Filterikonen (trattikonen) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]**där du kan välja i listorna [!UICONTROL Account] och [!UICONTROL Campaign] för att filtrera annonsnamnen i tabellen. Klicka på&#x200B;**Återställ**om du vill ta bort alla filterval.

![Upplevelsfilter och tabell](/help/assets/insights-experiences-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Upplevelseinformation

En _upplevelse_ är en marknadsföringsresurs som innehåller visuellt och interaktivt innehåll som är avsett för distribution till en viss målgrupp som en del av en marknadsföringskampanj.

Välj en upplevelse och visa prestandamått, textattribut och placeringar som är kopplade till varje annons. I detaljvyn kan ni analysera en upplevelses statistik utifrån dess annonsplacering och marknadsföring inom ett visst datumintervall.

Detaljvyn innehåller ett helhetsmått för annonsen `click-through rate`, `cost per action` och `spend` - hur mycket av budgeten som har använts i annonsen. Eftersom annonser kan ha flera placeringar, t.ex. en feed eller en banner, kan du se en uppdelning av samma mätvärden för varje annonsplacering. Använd vänster- och högerpilarna under **[!UICONTROL Performance by ad placement]** för att bläddra igenom placeringsmåtten.

![Lägg till information med mått och annonsplaceringar](/help/assets/insights-experience-details.png){zoomable="yes"}

### Textattribut

Under förhandsgranskningen av upplevelsen finns en lista med [!UICONTROL Text attributes] som är associerad med annonsen. När resurser och upplevelser har godkänts och lagrats i [!DNL Content] genererar GenStudio for Performance Marketing taggar baserat på deras inneboende funktioner. Mer information om systemmetadata finns i [Resursinformation](/help/user-guide/content/asset-details.md#system-metadata).

### Annonsplaceringar

När du skapade en kampanj med Meta-annonser kan du ha valt var annonserna ska köras baserat på kampanjens [mål](channels.md#objectives). Annonsplaceringar breddar räckvidden för era annonser.

GenStudio for Performance Marketing har stöd för annonsformat som resursflöden, länkannonser och en enda bild eller video. Nedan följer en lista över annonsformat per plattform:

| Instagram | Facebook/Meta | Messenger | Målgruppsnätverk |
| ------------ | ---------------- | ------------ | ---------------- |
| Utforska<br>Utforska startsida<br>Utforska startsida för stödraster<br>Utflöde<br>Reels<br>Profilflöde<br>Sök<br>Shop<br>Artiklar | Business Explore<br>Feed<br>Inströmsvideo<br>Marketplace<br>Reels<br>Reels-övertäckning<br>Right column<br>Search results<br>Stories<br>Video feeds<br>Ads on Facebook reels | Inkorg<br>artiklar | Inbyggd video, banderoll och interstitiell<br>återgiven video |

#### Platser som inte stöds

GenStudio for Performance Marketing stöder inte följande annonsplaceringar:

- Samarbete
- Katalog/Advantage+-katalog
- Instansupplevelse
- Carousel

## Upplevelseprestanda

Insikter kan hjälpa er att utvärdera vilka upplevelser som bidrar till framgången för en kampanj och vilka annonsplaceringar som är mest effektiva.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Experiences]. Varje mätvärde innehåller en kort definition av annonsnamn, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en upplevelse.

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Experience name]** | En lista över upplevelser för det anslutna kanalkontot. Filtrera annonser genom att välja en kampanj. | Sortera upplevelselistan genom att klicka på någon av nyckelmätarna. |
| **[!UICONTROL Campaign]** | En kampanj är en uppsättning upplevelser som utformats för att uppnå ett visst mål. | När du filtrerar tabellen Erfarenheter efter kampanj kan sammanfattningsmåtten för alla upplevelser för kampanjen vara annorlunda än kampanjens sammanfattningsrad i vyn [!UICONTROL Channels]. Skillnaden kan uppstå om kanalkällan, t.ex. Meta, och GenStudio använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL Placements]** | Antal annonser [praktik](#ad-placements), platser där en upplevelse påträffades i kampanjen. | Placeringar ökar publikens räckvidd.<p>Annonser som visar noll placeringar och noll resurser kan indikera en [annonstyp som inte stöds](#unsupported-placements).</p> |
| **[!UICONTROL Assets]** | Antalet resurser som används i annonsen eller upplevelsen. | Antalet i upplevelsetabellen kan skilja sig från antalet i vyn med upplevelseinformation. Skillnaden kan uppstå om kanalkällan, t.ex. Meta, och GenStudio använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL Impressions]** | Antal varje gång annonsplaceringen eller upplevelsen läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med ett klickbart element, till exempel en länk eller en knapp för att ringa upp, på en upplevelseplacering. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av intryck som resulterade i klickningar på upplevelseplaceringen i en kampanj.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kostnad för ett tusen annonsvisningar för upplevelseplacering.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Genomsnittlig kostnad för att utföra en viss kundåtgärd, t.ex. ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Använd för att övervaka utgifter för upplevelser som resulterar i värdefulla kundaktiviteter. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad som är associerad med varje klick på en upplevelseplacering.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som spenderats från Campaign-budgeten under en viss tidsperiod för att skapa den här annonsupplevelsen. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |

## Placering

I vyn _Upplevelseinformation_ återspeglar de tre viktigaste mätvärdena den övergripande prestandan för den valda upplevelsen. Avsnittet _Prestanda efter placering_ visar emellertid detaljerade mått för varje annonsplacering. Använd höger- och vänsterpilarna för att navigera mellan olika annonsplaceringar.

I följande tabell finns definitioner för prestandamätningar för annonsplacering:

| Mått | Definition | Insikt |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar för en enskild annonsplacering som resulterade i klickningar.<p>**Beräkning**:`clicks` delat med `impressions`<p>Denna mätmetod hjälper till att avgöra hur effektiv annonsplaceringen är när det gäller att engagera publiken. | En hög CTR indikerar att annonsplaceringen är relevant och lockande för publiken, vilket leder till fler interaktioner. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Den genomsnittliga kostnad som läggs på en enskild annonsplacering för att uppnå önskad kundåtgärd, till exempel ett köp eller en prenumeration.<p>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder<p>Denna mätmetod hjälper till att utvärdera annonsplaceringens kostnadseffektivitet när det gäller att få värdefulla åtgärder. | Ett lägre CPA tyder på att annonsplaceringen är effektiv när det gäller att konvertera målgruppsinteraktioner till önskat agerande till en lägre kostnad. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Den genomsnittliga kostnad som är associerad med varje klick på en enda annonsplacering.<p>**Beräkning**: totalt belopp `spent` delat med `clicks`<p>Denna mätning gör det enklare att bedöma hur kostnadseffektiv annonsplaceringen är när det gäller att generera klickningar. | En lägre CPC visar att annonsplaceringen genererar klickningar till en lägre kostnad, vilket kan vara fördelaktigt för att maximera avkastningen på investeringen. |
| **[!UICONTROL Spend]** | Det belopp som läggs på en enda annonsplacering, vilket motsvarar en bråkdel av det totala beloppet som spenderas på hela upplevelsen. Det här måttet hjälper till att spåra budgetallokeringen och utgiftseffektiviteten för varje annonsplacering. | Övervakning av utgifter kan bidra till att resurser används effektivt på olika platser. |
