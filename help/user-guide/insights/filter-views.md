---
title: Filtrera insikter
description: Lär dig använda de förbättrade filterfunktionerna med Insights.
level: Intermediate
feature: Reporting and Insights
source-git-commit: 656395e517fcb334b64865dcdbde09d8d982dc0a
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Filter för Insights-vyer

Instrumentpanelen [!DNL Insights] innehåller en omfattande uppsättning filter för en effektiv datautforskningsupplevelse. När du analyserar kanaler, annonser, medier eller specifika attribut kan du med filtreringsalternativen anpassa vyn och effektivisera arbetsflödet. Använd nyckelordsfilter för exakt målgruppsanpassning eller utforska fördefinierade listor för att förfina sökningen och fokusera på de data som betyder mest.

## Grundläggande om filter

I varje vy i [!DNL Insights] finns en lista med filteralternativ. Filterikonen (tratten) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]**. Oavsett om du visar tabellen eller galleriet visas använda filter i listan **[!UICONTROL Filter by]** ovanför tabellen eller galleriet. Som standard väljs en kanal och ett konto.

![Filtrera efter](/help/assets/insights-filter-by.png "Filtrera efter"){width=600 zoomable="yes"}

Tillämpade filter finns kvar i alla vyer. Välj **[!UICONTROL Clear all]** ovanför tabellen eller galleriet om du vill ta bort alla markerade filter.

### Sökfält

Klicka på sökningsikonen (förstoringsglas) om du vill använda en sökterm för att söka efter specifika objekt i tabellen eller galleriet. Om du till exempel anger termen `pink` i tabellen [!UICONTROL Ads] filtreras resultaten så att endast annonser visas med termen `pink` i namnet.

![Exempel på sökfält](/help/assets/insights-search.png "Sök efter annonser med rosa"){width=600 zoomable="yes"}

### Datumintervall

Väljaren för datumintervall är ett kraftfullt verktyg för att anpassa de visade data till analysmålen. Använd datumintervallväljaren för att justera tidsramen för de data som visas i tabellen eller gallerivyn. Som standard är datumintervallet inställt på de senaste 30 dagarna. Om du vill inkludera mer data eller fokusera på en viss period utökar du datumintervallet.

![Datumintervallväljare](/help/assets/insights-date-range.png "Välj ett datumintervall"){width=400}

Om inga objekt visas i tabellen eller gallerivyn kan det bero på det valda datumintervallet exklusive relevanta data. I så fall kan du öka datumintervallet för att se till att önskade data inkluderas.

### Sidor

Vissa tabeller kan omfatta flera sidor, vilket anges under tabellen till höger. Använd de mångsidiga sök- och filteralternativen för att förfina resultatet. Om du vill navigera mellan sidor använder du sidnumreringskontrollerna till höger (framåt) och vänster (bakåt). Se till att du använder filter på rätt sätt för att inkludera alla relevanta data på alla sidor.

### Bildstyrning

Vissa filteralternativ innehåller en bildkontroll som gör att du kan välja ett värde inom ett definierat intervall. I _[!UICONTROL Attributes]_kan du till exempel använda skjutreglaget **[!UICONTROL Media count]**för att filtrera attribut baserat på antalet associerade bilder eller videoklipp. Dra skjutreglaget för att ange ett intervall, från minst 0 till maximalt 100.

## Avancerad filtrering

Med filtren _[!UICONTROL Campaigns]_och_[!UICONTROL Ads]_ kan du använda exakta nyckelord för att förfina listan. Nyckelordsfilter är särskilt användbara för filtreringskampanjer eller annonser som använder en komplex namnkonvention med flera unika identifierare. Ett kampanjnamn kan till exempel innehålla följande:

- Namn eller kod för den specifika regionen: `NA`, `EMEA`
- Akronymer för innehållstyp: `EB`, `CHT` eller `DSP`
- Erbjudandekoder eller akronymer: `OFFER2023`, `PROMO`

Med tiden växer listan över kampanjer och annonser exponentiellt. Titta på följande scenario för att använda filtret _[!UICONTROL Campaigns]_för att förfina tabellen [!UICONTROL Ads].

**Så här förfinar du annonstabellen med Campaigns-filtret**:

1. I _[!DNL Insights]_väljer du vyn **[!UICONTROL Ads]**.

   ![Lägger till filter och tabell](/help/assets/insights-ads-filter.png "Lägger till vy med filterlista"){zoomable="yes"}

1. Klicka på filterikonen (trattikonen) ovanför den vänstra sidan av tabellen för att öppna menyn **[!UICONTROL Filter]**.

1. Kontrollera att rätt kanal och konto för `Filter by` har valts.

1. Expandera filtret **[!UICONTROL Campaigns]** och klicka på **[!UICONTROL Select]**.

   ![Filtrera kampanjer](/help/assets/insights-filter-campaigns-expand.png "Utöka kampanjfilter"){width=200}

1. Ange nyckelord avgränsade med kommatecken i sökfältet _[!UICONTROL Select campaigns]_.

   - Använd så många nyckelord som behövs för att förfina listan. Följande exempel söker efter kampanjer med `evergreen`, `ROI` och `Meta` i namnet:

     ![Nyckelordssökning](/help/assets/insights-select-campaigns-keywords.png "Ange nyckelord för att söka efter kampanjnamn"){width=500}

   - Du kan lägga till ytterligare en uppsättning nyckelord för att bredda sökningen. Om du använder flera uppsättningar nyckelord kan du inkludera kampanjer som matchar antingen den första uppsättningen nyckelord eller den andra uppsättningen nyckelord. Du kan till exempel söka efter kampanjer med etiketterna `evergreen` och `web` _OR_ med etiketterna `photoshop` och `roi`:

     ![Sök med flera uppsättningar nyckelord](/help/assets/insights-advanced-or.png "Sök efter kampanjnamn med flera uppsättningar nyckelord"){width=500}

1. Välj en eller flera kampanjer från den resulterande sökningen och klicka på **[!UICONTROL Apply]**.

   ![Lista över kampanjer](/help/assets/insights-select-campaigns-list.png "Välj kampanjer att inkludera")

Dina valda kampanjer visas nu i listan _[!UICONTROL Filter by]_ovanför annonstabellen eller galleriet. Ni kan fokusera enbart på annonser som är kopplade till de valda kampanjerna. I det här exemplet innehåller de filtrerade resultaten 28 annonser, vilket ger en mer målinriktad vy för analys.

![Tabell filtrerad efter kampanjer](/help/assets/insights-filter-by-campaigns.png "Tabell med kampanjfilter"){zoomable="yes"}

Du kan filtrera tabellen [!UICONTROL Media] ytterligare på ett liknande sätt för annonsnamn. Expandera filtret **[!UICONTROL Ads]** och klicka på **[!UICONTROL Select]** så kan du utföra ett liknande nyckelordsfilter för att förfina medietabellen eller gallerivyn.

## Hämta tabellresultat

Du kan hämta de filtrerade resultaten från tabellvyn för ytterligare analys eller delning. Klicka på nedladdningsikonen (pilen pekar nedåt) ovanför den högra sidan av tabellen för att ladda ned en CSV-fil baserat på den visningsbara tabellen. Hämtningen startar automatiskt och placerar CSV-filen på din standardplats för hämtning.

Vissa tabeller kan ha flera sidor, som du ser nedanför den högra sidan av tabellen. CSV-filen innehåller data från _alla_ sidor i tabellen.
