---
title: Hantera resurser och upplevelser
description: Förenkla och förbättra hanteringen av varumärkesgodkända mediefiler för användning och återanvändning i er digitala marknadsföringsresa.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 600d4a37be22bd057074b4dd3773b75f0273a567
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Hantera resurser och upplevelser

Adobe GenStudio for Performance Marketing [!DNL Content] förenklar och förbättrar hanteringen av varumärkesgodkända mediefiler för användning och återanvändning i den digitala marknadsföringsresan.

## Assets gallery

Galleriet [!UICONTROL Assets] visar en inventering av godkända resurser. Filterikonen (trattikonen) ovanför den vänstra sidan av tabellen öppnar menyn **[!UICONTROL Filter]** där du kan välja bland många kategorier för att filtrera resurserna som visas i galleriet. Klicka på sökningsikonen (förstoringsglas) om du vill använda ett nyckelord för att söka efter en resurs.

Följande visar en sökning på termen `dog` i galleriet [!UICONTROL Assets]:

![Assets-vy med sökning på hund](../../assets/content-assets.png)

### Assets

Som standard lagras resurser som du lägger till i [!DNL Content] genom [!DNL Create]-processen eller genom överföring i `GenStudio assets`-databasen. Databasen `GenStudio assets` är en läs- och skrivdatabas i GenStudio for Performance Marketing. Det innebär att du kan spara, redigera och ta bort resurser i databasen `GenStudio assets`.

I listan **[!UICONTROL Location]** ovanför galleriet till höger kan du välja mellan anslutna Adobe Experience Manager-databaser (AEM) [!DNL Assets Content Hub]. När du väljer en AEM databas visar galleriet en inventering av resurser från den databasen, vilket gör att du kan använda godkända resurser från dessa databaser som indata när du skapar innehåll. Filteralternativen ändras så att de återspeglar de kategorier som konfigurerats i [!DNL AEM Assets Content Hub].

Mer information om hur du lägger till din [!DNL AEM Assets Content Hub]-databas i GenStudio for Performance Marketing finns i [Anslut en AEM](connect-aem-repo.md).

Den AEM databasen är skrivskyddad, vilket innebär att du inte kan spara utkast, nya resurser eller metadata i den AEM databasen. Alla utkast och slutliga uppdateringar för resurser, upplevelser och mallar sparas i databasen `GenStudio assets` med nya [systemmetadata](asset-details.md#system-metadata).

{{note-aem-assets}}

## Assets

I [!UICONTROL Content] kan Performance Marketing enkelt lagra, hämta och hantera sina digitala resurser. Genom att utnyttja både databasen `GenStudio assets` och AEM kan användarna se till att deras resurser är välorganiserade och tillgängliga för olika marknadsföringskampanjer. Detta tillvägagångssätt med flera databaser ger flexibilitet och kontroll över resursanvändningen i olika miljöer, vilket säkerställer att endast godkända och aktuella resurser används i marknadsföringsarbetet.

### Lägga till resurser

När du lägger till resurser i [!DNL Content] lagras de som standard i databasen `GenStudio assets`. Knappen _[!UICONTROL Add assets]_är bara tillgänglig när_[!UICONTROL Location]_ är `GenStudio assets`-databasen.

![Platsfält](../../assets/content-location.png){width="350" align="center"}

**Så här lägger du till en eller flera resurser**:

1. Klicka på **[!UICONTROL Add assets]** i _[!DNL Content]_.

1. I vyn _Lägg till godkända resurser_ släpper du en eller flera filer i släppområdet. Du kan också välja mellan lokala filer med **[!UICONTROL Browse]** eller importera filer från Dropbox eller Microsoft OneDrive.

1. I avsnittet _Lägg till information_ väljer du **[!UICONTROL Campaign name]** eller anger ett nytt namn.

1. Om du vill förbättra identifieringsmöjligheterna lägger du till valfri information som _Varumärkesnamn_, _Personas_, _Region_ och _Nyckelord_ i avsnittet **Mer information** .

   Ju mer information du ger, desto mer upplever du GenStudio for Performance Marketing robusta funktioner. Välj en eller flera detaljer i listan eller ange en ny där det är tillämpligt, t.ex. med nyckelord. Varje detalj som du lägger till visas under listan. Klicka på **`x`** om du vill ta bort en detalj.

   All information som du lägger till gäller för alla resurser som läggs till i den här åtgärden.

   Se [Information om metadata](/help/user-guide/content/asset-details.md#system-metadata).

1. Klicka på **[!UICONTROL Add assets]**.

1. När överföringen av resursen är slutförd klickar du på **Klar**.

1. Om du vill visa dina nya överförda resurser klickar du på **[!UICONTROL Refresh]** i meddelandet _Nya resurser tillgängliga_ längst ned på arbetsytan.

<!--
In the future, need guidance on template upload errors. For now, the UI just says error.
-->

### Sök innehåll

Filtrerings- och sökgränssnittet är snabbt och responsivt och ger en produktiv sökupplevelse. Varje [!DNL Content]-vy innehåller filteralternativ som begränsar sökningen efter den idealiska resursen, upplevelsen eller mallen. För resurser och upplevelser kan du välja en kampanj och specifika riktlinjer, till exempel innehåll som har skapats för en viss produkt.

Det finns filter som baseras på [nyckelord](asset-details.md#user-defined-metadata) och [attribut](/help/user-guide/insights/attributes.md) för att begränsa sökresultaten. Du kanske vill hitta en resurs av en viss filtyp eller ett visst ämne som hjälper dig att skapa en ny upplevelse av kampanjen.

När du söker efter _upplevelser_ kan du använda filtret **[!UICONTROL Created by]** för att begränsa listan så att endast de upplevelser som du eller en viss person har skapat visas.

**Så här söker du efter innehåll som ska återanvändas**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Assets]**.

1. Välj en resurskatalog i listan **[!UICONTROL Location]** eller verifiera att du tittar på rätt resurskatalog. `GenStudio assets` är standarddatabas.

   >[!IMPORTANT]
   >
   >Listan _Plats_ är bara tillgänglig när du [ansluter till en AEM](connect-aem-repo.md).

1. Klicka på **[!UICONTROL Search]** (förstoringsglas) för att ange ett nyckelord eller en beskrivning.

1. Begränsa sökningen genom att välja en kategori i listan _[!UICONTROL Filter]_. Om du till exempel söker efter en PNG-fil klickar du på&#x200B;**[!UICONTROL File format]**och väljer **PNG**.

   Ju mer du begränsar sökningen, desto färre filteralternativ är tillgängliga. Klicka på **[!UICONTROL Clear all]** om du vill ta bort alla filter.

1. Välj en resurs för en fullständig vy och en lista med detaljer.

   Klicka på **[!UICONTROL Download]** (nedpil) om du vill använda resursen på den lokala arbetsstationen.
