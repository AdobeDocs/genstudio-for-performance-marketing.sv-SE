---
title: Bildfunktioner
description: Läs mer om bildfunktionen i de attributkategorier som används i GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: 808ffdb7f55f7ff938e9346b8513fab46f86df7c
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 0%

---

# Bildfunktioner

Bildfunktioner representerar distinkta och informativa element eller mönster i en bild som används för analys med [!DNL Insights]. Dessa funktioner hjälper till att kategorisera och förstå det visuella innehållet, vilket ger mer korrekta och detaljerade insikter. Genom att identifiera olika attribut, som stil, färg och objekt, kan AI ge en omfattande analys av bilden, vilket ger bättre beslutsunderlag och strategisk utformning.

## Stilidentifiering

Att fastställa _bildformatet_ fungerar som grund för att identifiera andra bildegenskaper. AI kan använda lämpliga analystekniker och identifiera relevanta funktioner, vilket ger en mer heltäckande bild. Varje format har distinkta visuella egenskaper som påverkar hur bilden uppfattas och analyseras.

Om bildformatet identifieras som `photograph` analyserar AI ytterligare egenskaper för `camera settings`, `camera proximity` och `Photography genres`. Dessa egenskaper är specifika för fotografier och ger djupare insikter om bildens komposition och kvalitet. Se [28 typer av fotostilar](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) i Adobe _Lär dig fotografi_ och lär dig mer om vanliga typer av fotografi och grundläggande terminologi.

Om bildformatet identifieras som `sketch` eller `digital cartoon` kan en annan uppsättning egenskaper vara relevanta. Denna hierarkiska metod säkerställer att analysen är exakt och skräddarsydd för just den typ av bild som undersöks.

## Sök efter bildfunktioner

**Så här visar du bilder i en specifik attributkategori**:

1. I _[!DNL Insights]_väljer du vyn **[!UICONTROL Attributes]**.

1. Ändra tabellvyn genom att välja **[!UICONTROL Images]**.

1. Välj en bildfunktion i listan **[!UICONTROL Attribute category]**, till exempel `Scenes`.

1. Välj ett attribut för en detaljerad vy över bilder som delar den kategorin.

   Kategorin `Scenes` kan till exempel ha `restaurant` som attribut.

1. Sidan _Attributinformation_ visar alla bilder med det här attributet.

I följande tabell visas de bildfunktionskategorier som känns igen av GenStudio for Performance Marketing AI. Den identifierade attributlistan för mediainnehåll är inte uttömmande. Media som innehåller en mängd funktioner kan begränsas till de tre dominerande funktionerna som identifieras av AI.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Kategori | Beskrivning | Exempel |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Attention-distribution | Visningsprogrammets uppmärksamhet sprids över en bild, vilket anger hur mycket fokus olika delar av bilden kan få. En högre fördelning innebär att inget enskilt område dominerar betraktarens fokus, medan en lägre fördelning innebär att en eller två fokuspunkter fångar betraktarens uppmärksamhet. | `high`, `medium`, `low`<p>Exempel på `low`-distribution till vänster och `high`-distribution till höger:<p>![Låg och hög fördelning - boll spelas](/help/assets/category/image-attn-lowhigh.png "Skillnad i låg och hög distribution"){width="200" zoomable="yes"} |
| Kameravinkel | Det perspektiv från vilket kameran fångar motivet, vilket påverkar tittarens uppfattning och tolkning av bilden. Om bildformatet är `photograph` identifieras den här egenskapen. | `Low angle`, `High angle`, `Eye level`, `Overhead view`, `Dutch angle`, `Bird's eye view`<p>Exempel på `eye level`:<p>![ögonnivå](/help/assets/category/image-camera-angle.png "Personer som sitter i olika vinklar"){width="200" zoomable="yes"} |
| Kamerainställning | De specifika justeringar och konfigurationer av kamerans kontroller som påverkar bildens slutliga utseende och kvalitet. Om bildformatet är `photograph` identifieras den här egenskapen. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Surreal`, `Double-exposure`, `Macro`, `Normal mode`<p>Exempel på en `macro`-inställning:<p>![Makronärbild](/help/assets/category/image-subject-distance.png "Makroinställning för närblomma och smyckesbi"){width="200" zoomable="yes"} |
| Färg och ton | Färger och tonala egenskaper i en bild. Identifierar upp till tre färger från en fördefinierad uppsättning med 40 färger i olika bildlager:<p>**[!UICONTROL Foreground colors]** - färger i bildens framsida <br>**[!UICONTROL Background colors]**- färger i bildens baksida | Färgvärden: `Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta`, {11 9}, `Yellow`, `Cyan`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald` `Orange` 36}, `Beige`, `Lilac`, `Olive` |
| Färgtemperatur | Beskriver den allmänna värmen eller färheten för färgerna i bilden. | Ton- eller temperaturvärden: `warm`, `cool`, `neutral`<br>![färger och svala toner](/help/assets/category/image-color-temp.png "Färgtemperatur med sval bakgrund och flera färgade objekt"){width="200" zoomable="yes"} |
| Innehållstäthet | Koncentrationen av visuella element och detaljer i en bild, vilket anger hur mycket information som packas in i det visuella utrymmet.<p>Till skillnad från uppmärksamhetsfördelningen, som mäter hur visningsprogrammets fokus sprids över olika områden i en bild, fokuserar innehållets täthet på mängden visuell information som finns. En högre innehållstäthet innebär att det finns fler element. | `high`, `medium`, `low`<p>Exempel på `low` densitet till vänster och `high` densitet till höger:<p>![Låg och hög densitet ball play](/help/assets/category/image-attn-lowhigh.png "Differens i låg och hög densitet"){width="200" zoomable="yes"} |
| Bildformat | Visuell behandling av en bild, till exempel ett fotografi eller en skiss. När AI avgör bildformatet kan andra egenskaper identifieras. Om bilden till exempel är ett fotografi kan kamerainställningar, kamerans närhet och ljusförhållanden gälla. | `Photograph`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Exempel på en `digital cartoon`-bildstil![seriebildstil](/help/assets/category/image-style.png "Bildstilserie för en katt"){width="200" zoomable="yes"} |
| Ljusvillkor | Beskriver kvaliteten på och egenskaperna hos ljuset i en bild, vilket påverkar stämningsläget, tonen och synligheten. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `High-key`, `Low-key`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Exempel på `daylighting`-villkor:<p>![Person och hund på trottoarkanten i dagsljus](/help/assets/category/image-lighting.png "Dagsljus"){width="200" zoomable="yes"} |
| Objekt | Identifierar ett eller flera objekt, enheter och element som utgör bilden. | Värdena är för många, men några exempel är: `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Exempel på `toucan` och `bird` objekt:<p>![Fågel, pekskärmsobjekt](/help/assets/category/image-objects-bird.png "Grafisk design av Toucan-fågelobjekt"){width="200" zoomable="yes"} |
| Orientering | Bildens justering i förhållande till dess bredd och höjd. Identifierar om den är bredare än den är hög (liggande), högre än bred (stående) eller lika med bredd och höjd (fyrkant). | `landscape`, `portrait`, `square`<p>Exempel på en `square`-orientering:<p>![fyrkantig skiss](/help/assets/category/image-orientation-square.png "Fyrkantig blomskiss"){width="200" zoomable="yes"} |
| Folk | När det finns minst en person kan ett eller flera attribut beskriva personen eller personerna i bilden. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Exempel på personer `woman` och `person` kategorier:<p>![personlig kvinna med kamera](/help/assets/category/image-people.png "Person som hanterar en kamera"){width="200" zoomable="yes"} |
| Fotografigenrer | Identifierar motivet och tekniken som används för att hämta en bild, till exempel `abstract` eller `landscape` (inte detsamma som liggande orientering). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite`<p>Se [Typer av foton](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) |
| Scener | Identifierar inställningen eller miljön i en bild och anger sammanhang för var bilden togs eller vilken typ av plats som avbildades. | Värdena är för många, men några exempel är: `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Exempel på `snow`, `sky`, `winter` och `mountain` scener som reflekteras på en hjälm:<p>![vintersnöscen](/help/assets/category/image-scenes.png "Vintern, snö, himmel och spegling av bergsområden"){width="200" zoomable="yes"} |
| Objektets avstånd | Avståndet mellan kameran och motivet i en bild. | `close up`, `mid shot`, `long shot`<p>Exempel på en `closeup shot`:<p>![närbild](/help/assets/category/image-subject-distance.png "Närbild av blomma och smyckesbi"){width="200" zoomable="yes"} |
| Stilar | Upptäcker visuella effekter som används på bildelement, t.ex. de som används i Lightroom eller Photoshop. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Exempel på `circular`-stil:<p>![cirkulär gateway i korallref](/help/assets/category/image-styles-circular.png "Cirkulär portal i en korallref"){width="200" zoomable="yes"} |
| Taggar | Identifierar andra bildegenskaper som inte faller under en viss klassificering. Taggar ger ytterligare kontext och metadata om bilden. AI kan till exempel identifiera `helmet`- och `motorobike`-objekt i en bild och inkludera `riding` som en tagg. | Värdena är för många, men några exempel är: `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Exempel på `dancer`- och `dancing`-taggar:<p>![taggar för dansare och dansare](/help/assets/category/image-tags.png "Dansande person"){width="200" zoomable="yes"} |
