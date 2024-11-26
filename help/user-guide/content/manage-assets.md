---
title: Hantera resurser och upplevelser
description: Förenkla och förbättra hanteringen av varumärkesgodkända mediefiler för användning och återanvändning i er digitala marknadsföringsresa.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 3a32c26ff746989798842afa5798ffa397a19ef8
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 0%

---

# Hantera resurser och upplevelser

Adobe GenStudio for Performance Marketing [!DNL Content] förenklar och förbättrar hanteringen av varumärkesgodkända mediefiler för användning och återanvändning i den digitala marknadsföringsresan.

## Innehållsgalleri

I galleriet visas en förteckning över godkända resurser, upplevelser eller mallar beroende på den valda vyn. Filterikonen (tratten) ovanför tabellens vänstra sida öppnar menyn **[!UICONTROL Filter]** där du kan välja bland många kategorier för att filtrera innehållet som visas i galleriet. I vyn _[!UICONTROL Assets]_klickar du på sökningsikonen (förstoringsglas) för att använda ett nyckelord för att hitta en resurs.


Följande visar en sökning på termen `dog` i galleriet [!UICONTROL Assets]:

![Assets-vy med sökning på hund](../../assets/content-assets.png)

### Sök innehåll

Filtrerings- och sökgränssnittet är snabbt och responsivt och ger en produktiv sökupplevelse. Varje [!DNL Content]-vy innehåller filteralternativ som begränsar sökningen efter den idealiska resursen, upplevelsen eller mallen. För resurser och upplevelser kan du välja en kampanj och specifika riktlinjer, till exempel innehåll som har skapats för en viss produkt.

Det finns filter som baseras på [nyckelord](asset-details.md#user-defined-metadata) och [attributkategorier](/help/user-guide/insights/attribute-category.md) för att begränsa sökresultaten. Du kanske vill hitta en resurs av en viss filtyp eller ett visst ämne som hjälper dig att skapa en ny upplevelse av kampanjen.

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

### Plats

Som standard lagras resurser som du lägger till i [!DNL Content] genom [!DNL Create]-processen eller genom överföring i `GenStudio assets`-databasen. Databasen `GenStudio assets` är en läs- och skrivdatabas i GenStudio for Performance Marketing. Det innebär att du kan spara, redigera och ta bort resurser i databasen `GenStudio assets`.

I listan **[!UICONTROL Location]** ovanför galleriet _[!UICONTROL Assets]_till höger kan du välja mellan anslutna Adobe Experience Manager-databaser (AEM) [!DNL Assets Content Hub].

![Platslista för databaser](../../assets/content-location-selection.png){width="350"}


När du väljer en AEM databas visar galleriet en inventering av resurser från den databasen, vilket gör att du kan använda godkända resurser från dessa databaser som indata när du skapar innehåll. Filteralternativen ändras så att de återspeglar de kategorier som konfigurerats i [!DNL AEM Assets Content Hub].

Mer information om hur du lägger till din [!DNL AEM Assets Content Hub]-databas i GenStudio for Performance Marketing finns i [Anslut en AEM](connect-aem-repo.md).

Den AEM databasen är skrivskyddad, vilket betyder att du kan komma åt innehållet men inte kan spara utkast, nya resurser eller metadata i den AEM databasen. Alla utkast och slutliga uppdateringar för resurser, upplevelser och mallar sparas i databasen `GenStudio assets` med nya [systemmetadata](asset-details.md#system-metadata).

{{note-aem-assets}}

## Assets

I [!UICONTROL Content] kan Performance Marketing enkelt lagra, hämta och hantera sina digitala resurser. Genom att utnyttja både databasen `GenStudio assets` och AEM kan användarna se till att deras resurser är välorganiserade och tillgängliga för olika marknadsföringskampanjer. Detta tillvägagångssätt med flera databaser ger flexibilitet och kontroll över resursanvändningen i olika miljöer, vilket säkerställer att endast godkända och aktuella resurser används i marknadsföringsarbetet.

### Lägga till resurser

När du lägger till resurser i [!DNL Content] lagras de som standard i databasen `GenStudio assets`. Knappen _[!UICONTROL Add assets]_är bara tillgänglig när_[!UICONTROL Location]_ är `GenStudio assets`-databasen.

![Platsfält](../../assets/content-location.png){width="350"}

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

### Hämta resurser

**Så här hämtar du en resurs**:

1. Välj en bildresurs i _[!DNL Content]_. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. I resursvyn klickar du på ikonen **[!UICONTROL Download]** (pilen pekar nedåt) i det övre högra hörnet.

1. Hämtningen börjar med att placera en kopia av resursen på din standardplats för hämtning.

### Ta bort resurser

**Ta bort en resurs**:

1. Välj en bildresurs i _[!DNL Content]_. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. I resursvyn klickar du på ikonen **[!UICONTROL Delete]** (papperskorgen) längst upp till höger.

1. Verifiera resursen i popup-fönstret _Ta bort resurs_ och klicka på **[!UICONTROL Delete]**.

## Redigera i Express

Du kan redigera bildresurser (JPG eller PNG) direkt i GenStudio for Performance Marketing med hjälp av Adobe Express. Arbetsytan i _[!UICONTROL Powered by Adobe Express]_har praktiska funktioner för att förbättra dina bilder utan att behöva lämna GenStudio-programmet. Du kan enkelt ta bort bakgrunder, använda generativa fyllningar, justera effekter och beskära bilder.

>[!BEGINSHADEBOX]

Kriterier för att förbättra bilder med funktionen [!DNL Edit in Adobe Express]:

- MIME-typer som stöds är `image/png` och `image/jpeg`
- Minsta bildstorlek är 50 x 50 pixlar
- Högsta bildstorlek är 8 000 × 8 000 pixlar
- Den maximala storleken är 40 MB (40 000 000 byte)

>[!ENDSHADEBOX]

**Så här redigerar du en resurs med Express**:

1. Välj en bildresurs i _[!DNL Content]_. När du klickar på en resurs öppnas en fokuserad vy över resursen.

1. I resursvyn klickar du på ikonen **[!UICONTROL Edit in Adobe Express]** i det övre högra hörnet.

1. Använd Express-kontrollerna på den vänstra panelen för att förbättra bilden på arbetsytan i _[!UICONTROL Powered by Adobe Express]_.

1. När du är nöjd med den uppdaterade bilden klickar du på **[!UICONTROL Save a copy]** uppe till höger.

1. Markera filformatet - JPG eller PNG - och klicka på **[!UICONTROL Save a copy]**.

1. Uppdatera **[!UICONTROL Asset name]** på popup-menyn _[!UICONTROL Save a copy of asset]_.

   - Välj **[!UICONTROL Same details as original asset]** om du vill överföra resursinformationen till den nya bilden.

   - Expandera avsnittet **[!UICONTROL More details]** för att uppdatera kampanjen, riktlinjerna och andra metadata.

   >[!TIP]
   >
   >Ju mer information du ger, desto mer upplever du GenStudio for Performance Marketing robusta funktioner. Välj en eller flera detaljer i listan eller ange en ny där det är tillämpligt, t.ex. med nyckelord. Varje detalj som du lägger till visas under listan. Klicka på **`x`** om du vill ta bort en detalj.

1. Klicka på **[!UICONTROL Save]**.
