---
title: Kampanjöversikt
description: Se en översikt över kundengagemang, resultat, budget och utgifter för marknadsföringskampanjer i Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Ad Performance
exl-id: 99059c81-0fef-4759-b52b-d6f7f9f82a52
source-git-commit: 494afe3f823c78eecd10ccc321cd83d69336077b
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Kampanjöversikt

Vyn [!DNL Insights] _[!UICONTROL Campaigns]_visar en lista med kampanjer för det anslutna kanalannonskontot.

{{connect-insights}}

Tabellen _[!UICONTROL Campaigns]_är organiserad med den kanalbaserade annonskampanjen. Klicka på inställningsikonen ovanför den högra sidan av tabellen för att växla mellan de kolumner som kan visas.

![Kampanjfilter och tabell](/help/assets/insights-campaigns-filter.png){zoomable="yes"}

När du väljer en kampanj öppnas fliken [[!UICONTROL Ads] ](ads.md) med en lista över annonsnamn som är associerade med den kampanjen, som gör att du kan identifiera vilka annonser som har bidragit till kampanjens övergripande framgång.

{{filter-table}}

## Mål

När ni skapade en kampanj med annonser från Meta kan ni ha valt ett mål som är anpassat till era affärsmål. Det finns sex tydliga mål från Meta-annonser i GenStudio for Performance Marketing:

1. **Kännedom**: Nå ut till största möjliga publik och nå ut till ert företag.
1. **Trafik**: Öka trafiken till din webbplats eller ditt program.
1. **Engagemang**: Interagera med befintliga och potentiella kunder.
1. **Leads**: Skapa anslutningar för att utöka er målgrupp.
1. **Appkampanj**: Befordra ditt program.
1. **Försäljning**: Fokusera på att nå de personer som mest sannolikt kommer att använda din produkt.

## Kanalprestanda

Beroende på dina prestationsmål kan [!DNL Insights]-mätvärden hjälpa dig att utvärdera om du uppnår ditt mål.

Om du till exempel har som mål att öka medvetenheten kan en ökning av hastigheten `impressions` tyda på att du utökar din räckvidd. Om du vill förstå om det uppnår ditt mål kan du titta på mätvärden som anger att ditt innehåll är engagerande, till exempel `clicks` eller `video plays`. Hur effektivt interagerar er målgrupp med ert innehåll?

Följande tabell innehåller definitioner och insikter för viktiga mätvärden för digital marknadsföring i kanalvyn. Varje mätvärde innehåller en kort definition vad gäller kanaler, hur mätvärdet beräknas och en eller flera insikter som hjälper till att förstå dess betydelse och påverkan på marknadsföringskampanjer.

| Mått | Definition | Insikt |
| ----------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Meta campaign name]** | En lista med kampanjnamn för det anslutna kanalkontot. Kampanjstatus kan vara `Active`, `Paused`, `Deleted` eller `Archived`. Filtrera kampanjer efter status och mål. | Sortera tabellen genom att klicka på kolumnrubriken för något av nyckelmåtten. |
| **[!UICONTROL Launch]** | Det datum då kampanjen släpptes eller publicerades på marknaden. | Ett högt antal visningar kan tyda på att annonsen når den avsedda målgruppen. |
| **[!UICONTROL Impressions]** | Antal gånger innehållet läses in i kanalen, oavsett interaktion eller visning. | Ett högt intryck kan visa på bred synlighet, men för att få en riktig prestandainsikter bör du överväga det tillsammans med andra interaktionsvärden. |
| **[!UICONTROL Clicks]** | Antalet gånger som användare interagerar med ett klickbart element, t.ex. en länk eller en call-to-action-knapp, i annonskampanjen. | Ett högt klickningsantal visar starkt intresse och engagemang för innehållet, vilket kan vara effektivt och nå rätt målgrupp. |
| **[!UICONTROL CTR]**<br>_Genomklickningsfrekvens _ | Procentandel (%) av visningar som resulterade i kampanjklickningar i en kanal.<br>**Beräkning**: (`clicks` dividerat med `impressions`) x 100 = % | En hög klickfrekvens visar att innehållet är mycket relevant och motiverat för målgruppen i budskapen och designen och att det effektivt riktar sig till målgruppens intressen. |
| **[!UICONTROL CPM]**<br>_Kostnad per tusen _ | Kostnad för ett tusen annonsvisningar för annonskampanjen. <br>**Beräkning**: (totalt belopp `spent` delat med `impressions`) x 1000 | Ett lågt värde kan indikera kostnadseffektiv synlighet, särskilt om det kombineras med en hög klickfrekvens. |
| **[!UICONTROL CPC]**<br>_Kostnad per klick _ | Genomsnittlig kostnad som associeras med varje klick i en annonskampanj.<br>**Beräkning**: totalt belopp `spent` dividerat med `clicks` = $ | Lägre genomsnittliga kostnader kan tyda på kostnadseffektiva annonskostnader, särskilt om man jämför med en ökning av antalet konverteringar. |
| **[!UICONTROL Video plays]** | Antalet gånger en video börjar spelas upp i en annonskampanj, exklusive repriser. En video börjar spelas upp när en användare klickar på Spela upp eller videon spelas upp automatiskt. | Ett stort antal videouppspelningar kan tyda på att videon fångar uppmärksamheten och kan betyda att miniatyren, titeln eller placeringen ritas effektivt i visningsprogrammen. |
| **[!UICONTROL Budget]** | Totala medel som anslagits för en annonskampanj för att uppnå kampanjmålen. | En hög budget innebär mer resurser för en bredare räckvidd och potentiellt större påverkan. |
| **[!UICONTROL Spend]** | Det belopp som läggs på annonser på olika plattformar från budgeten under en viss tidsperiod. | Ett högt utgiftsbelopp under en kort period kan tyda på snabb användning, vilket kan leda till att resurser tar slut i förtid. Spåra det belopp som spenderas mot nyckeltal för att övervaka den totala avkastningen på investeringen. |
