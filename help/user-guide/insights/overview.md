---
title: Översikt över insikter
description: Lär dig optimera annonser baserat på innehållsprestandamätningar i realtid.
level: Intermediate
feature: Reporting and Insights
exl-id: 26402a06-f776-42be-9d8d-fc498c0f75a8
source-git-commit: 42a211956854126798024a97fc0befc3626160b7
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing Insights

Adobe GenStudio for Performance Marketing [!DNL Insights] tillhandahåller avancerade analyser och insikter om innehållsprestanda som kan hjälpa dig att fatta datadrivna beslut.

Från kontrollpanelen [!DNL Insights] kan du:

- **Identifiera det mest effektiva innehållet**: Identifiera vilket innehåll som fungerar bäst för olika målgrupper och skräddarsy framtida innehåll eller kampanjer för trendinställningar.
- **Optimera innehåll med låg prestanda**: Hitta innehåll som inte fungerar bra och använd den integrerade generativa AI-koden för att skapa variationer direkt, vilket kan förbättra dess effektivitet utan att börja från början.
- **Revitalisera högpresterande innehåll**: Använd lyckat innehåll och justera det för att uppdatera annonsen för målgruppen eller anpassa hjälteinnehållet för användning i nya kampanjer, vilket kan förlänga dess livscykel och prestanda.

## Dataanslutningar

Första gången du öppnar [!DNL Insights] kan du se en banderoll som hjälper dig att ansluta Adobe GenStudio for Performance Marketing till ett kanalkonto.

Med den här anslutningen kan GenStudio for Performance Marketing ta emot statistiska data från era aktiva marknadsföringskampanjer, medier och annonser. Till att börja med importerar GenStudio for Performance Marketing in de sista sex månaderna av data så att du har verktygen för att analysera de senaste data och vidta åtgärder.

{{connect-insights}}

## Kontrollpanel

Kontrollpanelen [!DNL Insights] har en konfigurerbar tabell för varje innehållstyp: [!UICONTROL Channels], [!UICONTROL Ads], [!UICONTROL Media] och [!UICONTROL Attributes].

![[!DNL Insights] instrumentpanel](/help/assets/insights-dashboard.png)

I varje vy visas en motsvarande tabell, som du kan söka efter nyckelord, filtrering och datumintervall. Du kan klicka på inställningsikonen (cog) ovanför den högra sidan av tabellen för att växla mellan olika kolumntyper. Raden _[!UICONTROL Summary]_kan visa summor eller medelvärden för en kolumn.

[!UICONTROL Ads], [!UICONTROL Media] och [!UICONTROL Attributes] innehåller en gallerivy där du kan skanna och sortera resurser med kort med en bild- eller videominiatyr. Det finns ett alternativ för att visa en av tre nyckelmått på varje kort: `Click-through rate`, `Cost per click` och `Spend`.

### Kanaler

[[!DNL Insights] _[!UICONTROL Channels]_-vyn ](channels.md) är standardvy och visar en lista med aktiv kampanjinformation, till exempel mål, budget, startdatum och aktivitet. Se till att [ansluta ett kanalkonto](/help/user-guide/connectors/connect-channel.md) så att GenStudio for Performance Marketing börjar ta emot dina statistiska data.

### Annonser

[[!DNL Insights] _[!UICONTROL Ads]_-vyn ](ads.md) fokuserar på att utvärdera effekten av en annons. I vyn [!UICONTROL Ads] kan du analysera en annons mått baserat på dess annonsplacering inom ett angivet datumintervall. Genom att klicka på en_[!UICONTROL Ad name]_ kan du visa annonsens prestandamått, prestanda per annonsplacering och attribut.

### Media

[[!DNL Insights] _[!UICONTROL Media]_-vyn ](media.md) är utformad för att hjälpa dig att analysera prestandan för kreativt innehåll. Du kan identifiera medieattribut som bidrar till att förbättra ett markerat mätresultat, t.ex. klick eller visningar.

Om du klickar på medieinnehåll får du ytterligare information om hur det fungerar i olika annonser och på olika annonsplaceringar:

![Medieinformation](/help/assets/insights-media-details.png){width="600" zoomable="yes"}

I vyn Medieinformation visas en miniatyrbild av resursen och en lista med attribut till vänster. Det finns tre markerade mått: `Click-through rate`, `Cost per click` och `Spend`. Prestandamarkeringarna visar hur faktiska värden (heldragen linje) jämförs med det genomsnittliga värdet (streckad linje) under den valda tidsperioden (standardvärdet är `Last 30 days`).

### Attribut

Media _attributes_ hjälper till att identifiera det kreativa innehållet med hjälp av inbyggda detaljer som färg, ton, komposition (t.ex. motiv, teckensnitt, visuella element) och andra viktiga komponenter. Attribut är ofta den minst uppmätta och analyserade uppsättningen med innehållsinformation.

[[!DNL Insights] _[!UICONTROL Attributes]_-vyn ](attributes.md) kan hjälpa dig att utforska och identifiera vilka attribut som fungerar bättre med vissa målgrupper, kanaler, regioner och kan hjälpa dig att lyfta fram säsongstrender. Med dessa insikter kan ni använda resultatattribut för att skapa varianter, inrikta er på en viss målgrupp eller experimentera med olika kampanjstrategier.
