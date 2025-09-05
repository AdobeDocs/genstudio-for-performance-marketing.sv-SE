---
title: Mallkodsredigerare
description: Lär dig använda mallkodsredigeraren i GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: f9fec89a522f3c82367516b79dbc79db5a106bbf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Mallkodredigerare

Mallkodredigeraren är utformad för att hjälpa dig att verifiera och förfina mallen för optimal användning när du skapar nya upplevelser med GenStudio for Performance Marketing. Redigeraren har stöd för Handlebars-syntaxen, som använder platshållare i mallen för att ange var GenStudio for Performance Marketing ska generera innehåll åt dig.

>[!TIP]
>
>Innan du överför din HTML-mallkod till vyn [!DNL Content] _Mallar_ förbereder du mallen genom att infoga platshållare för innehåll som definieras i vägledningen för [Anpassa mallar](customize-template.md) .

## Kontrollera identifierade fält

I rutan _[!UICONTROL Check detected fields]_visas en lista med fält som GenStudio for Performance Marketing känner igen i din mall. Granska listan och bläddra igenom HTML-koden för att se hur mallen har skapats.

![Vyn Kodredigeraren](/help/assets/template-detected-fields.png "Kontrollera identifierade fält"){width="600"}

Om du upptäcker att ett fält saknas i listan söker du efter mallkoden och letar reda på platsen för det fält som saknas. Infoga rätt platshållare med hjälp av Handlebars-syntaxen och ett [igenkänt fältnamn](/help/user-guide/content/customize-template.md#recognized-field-names). Använd formuläret Sök och ersätt, som visas längst ned i kodredigeraren, om du vill söka efter särskilda strängar i koden. (Windows `CTRL`+`F` eller macOS `CMD`+`F`)

## Justera roller för en variabel

Du kan välja och ändra fältroller för textbaserade fältroller (till exempel `headline`, `sub_headline`, `body`, `cta`, `on_image_text`, `custom`) med en listruta under kontrollen av mallstrukturen. Fältrollval kvarstår under mallredigeringar så att anpassningarna inte går förlorade, vilket förbättrar arbetsflödets effektivitet.

>[!NOTE]
>
>Bildvariabler kan inte ha sina roller justerade.

![Markering av fält med flera roller](/help/assets/multirole-dropdown-field.png "Markering av fält med flera roller"){width="600"}

Tilldela en roll till en variabel:

1. Hitta variabeln i rutan _[!UICONTROL Check detected fields]_. Dessa variabler identifieras automatiskt.
2. Granska rollerna som tilldelats varje variabel. Roller tilldelas automatiskt men kan justeras med hjälp av listrutan för alla variabler i mallen.
3. Justera en roll genom att välja en ny roll i listrutan.
4. Klicka på **[!UICONTROL Next]** för att fortsätta.

## Korrigera

Om det finns fel i mallen kan du se ett `Template is invalid`-meddelande med en kort förklaring av problemet. I följande exempel anger meddelandet att fältet `_image` inte följer den fältnamnkonvention som har upprättats i mallen för flera punkter. Meddelandet talar också om att du måste uppdatera fältnamnet med rätt prefix. Leta reda på fältet `_image` i mallkodsredigeraren och uppdatera namnet enligt anvisningarna.

![Korrigera ogiltig mall](/help/assets/animation/template-code-editor.gif){width="600"}

Panelen _[!UICONTROL Check detected fields]_uppdateras för att återspegla de ändringar du har gjort. När du är nöjd med att fälten är korrekta och fullständiga klickar du på&#x200B;**[!UICONTROL Next]**för att fortsätta [överföra mallen](/help/user-guide/content/use-templates.md#add-a-template).

## Vanliga mallproblem och lösningar

| **Fel** | **Beskrivning** | **Lösning** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Det gick inte att analysera | Mallinnehållet kunde inte parsas som giltiga handtag. | Kontrollera om mallen innehåller syntaxfel för HTML och Handlebars och korrigera dem för att säkerställa giltig formatering för [innehållsplatshållare](/help/user-guide/content/customize-template.md#content-placeholders). |
| Gruppen har inte tilldelats | Ett bildfält i en e-postmall för flera grupper tilldelas ingen grupp. | Kontrollera om avsnittsprefix används på ett konsekvent sätt. Varje [avsnitt](/help/user-guide/content/customize-template.md#sections-or-groups) kan bara använda en av varje fälttyp (`headline`, `body`, `image` `cta`). Tilldela fältet `image` till en giltig grupp i mallen. |
| Bild saknas | Ett obligatoriskt bildfält saknas. | Exakt ett `image`-fält krävs för vissa malltyper, t.ex. en Meta-, display- eller banner-annons. Lägg till det obligatoriska `image`-fältet i mallen. |
| Ogiltig enskild grupp | E-postmallen innehåller exakt en grupp, vilket är ogiltigt. | En grundläggande e-postmall innehåller en enda uppsättning mallelement som inte kräver gruppnamnkonventionen enligt definitionen i [Avsnitt eller grupper](/help/user-guide/content/customize-template.md#sections-or-groups). Justera mallen så att den har noll avsnitt genom att ta bort all gruppnamnssyntax. |
| Inga fält | Mallen innehåller inga fält. | Lägg till [igenkända fältnamn](/help/user-guide/content/customize-template.md#recognized-field-names) med användarlistesyntaxen i mallen där du behöver GenStudio for Performance Marketing för att generera en viss typ av innehåll. |
| Obligatoriska egenskaper saknas | Vissa nödvändiga metadataegenskaper saknas. | Varje malltyp har krav och begränsningar baserade på kanalriktlinjerna. Meta kräver till exempel proportioner och visningsannonser kräver dimensioner. [Följ kanalspecifika riktlinjer för mallar](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Reserverat namn används | Ett förbjudet eller reserverat fältnamn används. | Vissa [fältnamn ](/help/user-guide/content/customize-template.md#recognized-field-names), till exempel `subject` eller `introductory_text`, är reserverade. Byt namn på fält som använder reserverade eller förbjudna namn. |
| För många fält | Antalet fält överskrider den globala gränsen på 20. | Ta bort onödiga fält för att säkerställa att summan inte överstiger 20. |
| För många grupper | Antalet grupper överskrider kanalens högsta tillåtna antal. | Meta-, display- och LinkedIn-mallar tillåter inte flera avsnitt. E-post kräver gruppnamngivning när två eller tre avsnitt definieras. Minska antalet grupper i mallen för att uppfylla [kanalens krav](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Fältet stöds inte | Mallen använder ett fält som kanalen inte stöder. | Ersätt eller ta bort fält som inte stöds enligt de [identifierade fältnamnen](/help/user-guide/content/customize-template.md#recognized-field-names). |
