---
title: Mallkodredigerare
description: Lär dig använda mallkodsredigeraren i GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Mallkodredigerare

Mallkodredigeraren är utformad för att hjälpa dig att verifiera och förfina mallen för optimal användning när du skapar nya upplevelser med GenStudio for Performance Marketing. Redigeraren har stöd för Handlebars-syntaxen, som använder platshållare i mallen för att ange var GenStudio for Performance Marketing ska generera innehåll åt dig.

>[!TIP]
>
>Innan du överför din HTML-mallkod till vyn [!DNL Content] _Mallar_ förbereder du mallen genom att infoga platshållare för innehåll som definieras i vägledningen för [Anpassa mallar](customize-template.md) .

## Kontrollera identifierade fält

I rutan _[!UICONTROL Check detected fields]_&#x200B;visas en lista med fält som GenStudio for Performance Marketing känner igen i din mall. Granska listan och bläddra igenom HTML-koden för att se hur mallen har skapats.

![Vyn Kodredigeraren](/help/assets/template-detected-fields.png "Kontrollera identifierade fält"){width="600" zoomable="yes"}

Om du upptäcker att ett fält saknas i listan söker du efter mallkoden och letar reda på platsen för det fält som saknas. Infoga rätt platshållare med hjälp av Handlebars-syntaxen och ett [igenkänt fältnamn](/help/user-guide/content/customize-template.md#recognized-field-names). Använd formuläret Sök och ersätt, som visas längst ned i kodredigeraren, om du vill söka efter särskilda strängar i koden. (Windows `CTRL`+`F` eller macOS `CMD`+`F`)

### Korrigera

Om det finns fel i mallen kan du se ett `Template is invalid`-meddelande med en kort förklaring av problemet. I följande exempel anger meddelandet att fältet `_image` inte överensstämmer med den fältnamnkonvention som har upprättats i mallen för flera punkter. Meddelandet talar också om att du måste uppdatera fältnamnet med rätt prefix. Leta reda på fältet `_image` i mallkodsredigeraren och uppdatera namnet enligt anvisningarna.

![Korrigera ogiltig mall](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

Panelen _[!UICONTROL Check detected fields]_&#x200B;uppdateras för att återspegla de ändringar du har gjort. När du är säker på att fälten är korrekta och fullständiga klickar du på&#x200B;**[!UICONTROL Next]**&#x200B;för att fortsätta [överföra mallen](/help/user-guide/content/use-templates.md#add-a-template).
