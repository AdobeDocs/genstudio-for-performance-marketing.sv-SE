---
title: Översikt över annonsplacering
description: Se en översikt över kundengagemang, budget och utgifter för annonser och annonsplaceringsprestanda i Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 63134aab89053616ea6190c958e8bf5b64ee9793
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# Översikt över annonsplacering

Vyn [!DNL Insights] _[!UICONTROL Ads]_&#x200B;visar en lista med annonser för det anslutna kanalannonskontot. En_ annons _är en kampanjresurs som innehåller visuellt och interaktivt innehåll som är avsett för distribution till en viss målgrupp som en del av en marknadsföringskampanj.

{{connect-insights}}

Tabellen _[!UICONTROL Ads]_&#x200B;är ordnad med [!UICONTROL Ad names]. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas.

![Lägger till filter och tabell](/help/assets/insights-ads-filter.png){zoomable="yes"}

I gallerivyn _[!UICONTROL Ad]_&#x200B;visas ett collage med förhandsvisningar av annonser och ett mått, till exempel klickfrekvens. Klicka på inställningsikonen (cog) ovanför den högra sidan av galleriet för att öppna **[!UICONTROL Card settings]**&#x200B;och växla en av tre mätvärden som kan visas:

- CPA (kostnad per åtgärd)
- CTR (klickfrekvens)
- CPC (kostnad per klick)
- Utgift

{{filter-table}}

## Annonsinformation

Välj en annons och visa de resultatvärden, textattribut och placeringar som är kopplade till varje annons. _[!UICONTROL Ad details page]_&#x200B;innehåller mått för annonsen `click-through rate`, `cost per action` och `spend` - hur mycket av budgeten som har använts för annonsen. Eftersom annonser kan ha flera placeringar, t.ex. en feed eller en banner, kan du se en uppdelning av samma mätvärden för varje annonsplacering. Använd vänster- och högerpilarna under **[!UICONTROL Performance by ad placement]**&#x200B;för att bläddra igenom placeringsmåtten.

![Lägg till information med mått och annonsplaceringar](/help/assets/insights-ad-details.png){zoomable="yes"}

### Annonsattribut

Under annonsförhandsvisningen finns en lista med attribut som är kopplade till annonsen.

{{$include /help/_includes/generated-attributes.md}}

### Annonsformat

Annonsformaten avser de olika kreativa element och layouter som används för att anpassa er efter era kampanjmål, engagera målgruppen och hjälpa er att spåra resultatvärden.

[!DNL Insights] i GenStudio for Performance Marketing har för närvarande stöd för följande tillgängliga annonsformat.

| Stöds | Stöds inte |
|----------------------------------|-----------------------------------|
| Dynamiska annonser<br>Länka annonser<br>Enkla bildannonser<br>Enkla videoklipp | Shop Ads<br>Advantage+ Shopping Ads<br>Advantage+ Catalog Ads<br>Carousel Ads<br>Messenger Ads<br>Lead Ads<br>Collection Ads<br>Call Ads<br>Owned Page Post Ads<br>Partnership Ads<br>Flexibla annonser |

### Annonsplaceringar

Annonsplaceringar avser de specifika platser eller plattformar där annonserna visas i en kampanj. Dessa placeringar avgör hur och var era målgrupper interagerar med ert innehåll. Annonsplaceringar breddar målgruppens räckvidd, vilket hjälper till att maximera synlighet, engagemang och den övergripande kampanjeffektiviteten.

När du skapar en kampanj med Meta-annonser kan du ha valt var annonserna ska köras baserat på kampanjens [mål](channels.md#objectives).

Här följer en lista över annonsplaceringar som stöds:

| Målgruppsnätverk | Facebook/Meta \* | Instagram | Messenger |
|--------------------|--------------------|-------------------------|---------------------|
| Återgiven video | Feed<br>Videoflöden<br>Artiklar<br>Marketplace<br>Högerkolumn<br>Reels<br>Reels-övertäckning<br>In-stream-video<br>Search<br>Business discofeed<br>Profilfeed | Artiklar<br>Feed<br>Utforska<br>Reels<br>Utforska stödrastrets startsida<br>Profilflöde<br>Sök<br>Stream | Artiklar<br>Inkorg |

\* Se [Om annonsplaceringar mellan metatekniker](https://www.facebook.com/business/help/407108559393196?id=369787570424415) i _Meta Business Help Center_.

## Annonsprestanda

Insikter kan hjälpa er att utvärdera vilka annonser som bidrar till framgången för en kampanj och vilka annonsplaceringar som är mest effektiva.

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i tabellvyn [!UICONTROL Ads]. Varje mätvärde innehåller en kort definition av annonsnamn, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på en annons.

| Mått | Definition | Insikt |
| ---------------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Ad name]** | En lista med annonser för det anslutna kanalkontot. Filtrera annonser genom att välja en kampanj. | Sortera annonslistan genom att klicka på någon av nyckelmätarna. |
| **[!UICONTROL Campaign]** | En kampanj är en uppsättning annonser som utformats för att uppnå ett visst mål. | När du filtrerar annonstabellen efter kampanj kan sammanfattningsmåtten för alla annonser för kampanjen vara annorlunda än kampanjens sammanfattningsrad i [!UICONTROL Channels]-vyn. Skillnaden kan uppstå om kanalkällan, t.ex. Meta, och GenStudio använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL Placements]** | Antal annonser [praktik](#ad-placements), platser där en annons visades i kampanjen. | Placeringar ökar publikens räckvidd.<p>Annonser som visar noll-placeringar och noll-media kan indikera en [annonstyp som inte stöds](#unsupported-placements).</p> |
| **[!UICONTROL Media]** | Antalet resurser som används i annonsen och annonsplaceringar | Antalet i annonstabellen kan skilja sig från antalet i vyn Ad details. Skillnaden kan uppstå om kanalkällan, t.ex. Meta, och GenStudio använder något olika sammanfattningsberäkningar. |
| **[!UICONTROL Impressions]** | Antal varje gång annonsplaceringen eller annonsen läses in i kanalen, oavsett interaktion eller visning. | Ett högt visningsvärde kan visa på bred synlighet, men för verkliga prestandainsikter bör du tänka på det i relation till andra engagemangsmått. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med ett klickbart element, som en länk eller en call-to-action-knapp, på en annonsplacering. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i klickningar på annonsen i en kampanj.<br>**Beräkning**: `clicks` delat med `impressions` | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Genomsnittskostnaden för var tusen annonsvisningar.<br>**Beräkning**: totalt belopp `spent` dividerat med räckvidd, multiplicerat med 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Den genomsnittliga kostnaden för att utföra en viss kundåtgärd, till exempel ett köp eller en prenumeration.<br>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder | Använd för att övervaka utgifter för annonser som resulterar i värdefulla kundaktiviteter. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Den genomsnittliga kostnad som är associerad med varje klick i en annonsplacering.<br>**Beräkning**: totalt belopp `spent` delat med `clicks` | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Spend]** | Det belopp som har använts från kampanjbudgeten under en viss tidsperiod för att placera den här annonsen. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
| **Attribut** | Lista över inbyggda funktioner i den här annonsen. | Attribut hjälper er att identifiera kreativa element som intresserar er bäst. Se [Kategorier](/help/user-guide/insights/attributes.md#categories). |

## Placering

I vyn _[!UICONTROL Ad details page]_&#x200B;återspeglar de tre översta måtten den valda annonsens totala prestanda. Avsnittet_ Prestanda efter placering _visar emellertid detaljerade mått för varje annonsplacering. Använd höger- och vänsterpilarna för att navigera mellan olika annonsplaceringar.

I följande tabell finns definitioner för prestandamätningar för annonsplacering:

| Mått | Definition | Insikt |
| ---------------------------- | ----------------------------- | --------------------------------- |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar för en enskild annonsplacering som resulterade i klickningar.<p>**Beräkning**:`clicks` delat med `impressions`<p>Denna mätmetod hjälper till att avgöra hur effektiv annonsplaceringen är när det gäller att engagera publiken. | En hög CTR indikerar att annonsplaceringen är relevant och lockande för publiken, vilket leder till fler interaktioner. |
| **[!UICONTROL CPA]**<br>_Kostnad per åtgärd _ | Den genomsnittliga kostnad som läggs på en enskild annonsplacering för att uppnå önskad kundåtgärd, till exempel ett köp eller en prenumeration.<p>**Beräkning**: totalt belopp `spent` delat med antalet slutförda kundåtgärder<p>Denna mätmetod hjälper till att utvärdera annonsplaceringens kostnadseffektivitet när det gäller att få värdefulla åtgärder. | Ett lägre CPA tyder på att annonsplaceringen är effektiv när det gäller att konvertera målgruppsinteraktioner till önskat agerande till en lägre kostnad. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Den genomsnittliga kostnad som är associerad med varje klick på en enda annonsplacering.<p>**Beräkning**: totalt belopp `spent` delat med `clicks`<p>Denna mätning gör det enklare att bedöma hur kostnadseffektiv annonsplaceringen är när det gäller att generera klickningar. | En lägre CPC visar att annonsplaceringen genererar klickningar till en lägre kostnad, vilket kan vara fördelaktigt för att maximera avkastningen på investeringen. |
| **[!UICONTROL Spend]** | Det belopp som läggs på en enda annonsplacering, vilket motsvarar en bråkdel av det totala beloppet som spenderas på hela annonsen. Det här måttet hjälper till att spåra budgetallokeringen och utgiftseffektiviteten för varje annonsplacering. | Övervakning av utgifter kan bidra till att resurser används effektivt på olika platser. |
| **Attribut** | Lista över inbyggda funktioner i den här annonsplaceringen. | Attribut hjälper er att identifiera kreativa element som intresserar er bäst. Se [Kategorier](/help/user-guide/insights/attributes.md#categories). |
