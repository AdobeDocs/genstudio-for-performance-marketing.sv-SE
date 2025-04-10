---
title: Bästa tillvägagångssätt för mallar
description: Följ vedertagna standarder när du använder mallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 0f296fe6ec92178498e2e0eeb3e190a194e46aa0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Bästa tillvägagångssätt för att använda mallar

Mallar minskar avsevärt den tid och det arbete som krävs för att generera nytt innehåll genom att tillhandahålla en startpunkt med förkonfigurerade layouter och designelement.

Använd följande rekommendationer när du använder mallar med GenStudio for Performance Marketing:

1. Lär dig mer om [mallelement](#know-about-template-elements)
1. Konfigurera [kanalriktlinjer](#configure-channel-guidelines) för effektiv personalisering av innehåll
1. Designa med [tillgänglighetsstandarder](accessibility-for-templates.md) för en optimal upplevelse
1. Följ [kanalspecifika riktlinjer för mallar](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Läs mer om grundläggande mallelement och procedurer i [Arbeta med mallar](use-templates.md). Och fördjupa dig i [att anpassa en mall](customize-template.md) för användning i nästa kampanj.

## Lär dig mer om mallelement

Ett tips är att bekanta sig med delarna i en mall. Varje malltyp använder olika element för att skapa en struktur för kanalspecifik innehållsutveckling. Om du vill anpassa mallen använder du fältnamnen i stället för dessa element där du behöver GenStudio for Performance Marketing för att generera innehåll.

Se [Mallelement](use-templates.md#template-elements).

## Konfigurera kanalriktlinjer

Konfigurera kanalriktlinjer för varje varumärke innan du använder mallar i GenStudio for Performance Marketing. Kanalriktlinjerna påverkar direkt vilken typ av innehåll som skapas när mallen används. Du kan t.ex. ange teckenbegränsningar för brödtexten i ett e-postmeddelande.

![Specifikationer för brödtext](/help/assets/channel-email-body.png)

Se [kanalriktlinjer](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Följ kanalspecifika riktlinjer för mallar

När du skapar mallar måste du se till att de uppfyller de specifika kraven för den avsedda kanalen. Skapa mallar som passar de layoutkrav och visuella krav som gäller för varje kanal. Det finns allmänna riktlinjer som gäller för alla mallar, till exempel:

- Använd rena och responsiva HTML och inline CSS
- Använda Adobe- eller Google-teckensnitt
- Använd **inte** JavaScript

Tänk på följande när du arbetar med varje malltyp för att få optimala prestanda och kompatibilitet:

>[!BEGINTABS]

>[!TAB E-post]

Följ de här designmetoderna när du anpassar e-postmallar för att arbeta med GenStudio for Performance Marketing:

- Använda Adobe- eller Google-teckensnitt
- Använd rena och responsiva HTML och inline CSS
- Använd **inte** JavaScript
- Använd **inte** fast bredd i brödtext eller behållare
- Använd **inte** base64-kodning för bilder eftersom det kan öka mallstorleken avsevärt

**Begränsningar**:

- Användning av [avsnitt](customize-template.md#sections-or-groups):
   - En grundläggande mall (endast ett avsnitt) kan generera en enda uppsättning mallelement.
   - En komplex mall (flera avsnitt) kan generera upp till tre uppsättningar mallelement.
- Det högsta tillåtna antalet fält i en mall är 20
- Den största filstorleken för HTML är 102 kB

**Identifierade fältnamn**:

För e-post inkluderas fältet `subject` automatiskt. Använd innehållsplatshållare för följande fält:

- `pre_header`
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (markerat från JPEG, PNG eller GIF)

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](customize-template.md#content-placeholders) .

>[!TAB Metaannons]

Följ de här designmetoderna när du anpassar metadatamallar för GenStudio for Performance Marketing:

- Använd 360 pixlar bred för kolumnlayouter
- Använd en lägsta upplösning på 1 080 x 1 080 pixlar för bilder
- Använd den relativa teckenstorleken **inte**
- Definiera **inte** visningsruta
- Använd **inte** JavaScript
- Åsidosätt **inte** ett HTML-element i CSS
- Använd taggen `<img>` i stället för `background-image`
- Använd maskning för att förbättra textläsbarheten över bakgrundsbilder

**Begränsningar**:

- Användning av [avsnitt](customize-template.md#sections-or-groups):
   - Endast ett avsnitt kan användas, vilket genererar en enda uppsättning mallelement.

**Proportioner som stöds**:

- Fyrkant 1:1 (1 080 x 1 080 pixlar)
- Lodrät 4:5 (1 080 x 1 350 pixlar)
- Artikel 9:16 (1 080 x 1 920 pixlar)
- Anpassad bildstorlek: (minsta bildbredd på 50 x 50 pixlar)

**Identifierade fältnamn**:

För Metaannonser genereras fälten `headline`, `body` och `CTA` automatiskt. Använd innehållsplatshållare för följande fält:

- `image` (markerat från JPEG, PNG eller GIF)
- `on_image_text`

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](customize-template.md#content-placeholders) .

>[!TAB Banner &amp; Display ad ]

Följ de här designmetoderna när du anpassar mallar för banners och displayannonser så att de fungerar med GenStudio for Performance Marketing:

- Använda Adobe- eller Google-teckensnitt
- Förbered resurser som visas bra i tunna dimensioner
- Använd **inte** inbäddade eller kodade bakgrundsbilder
- Använd bakgrundsbilder (`image` fält) överförda till GenStudio for Performance Marketing innehållsdatabas
- Använd **inte** JavaScript

**Begränsningar**:

- Användning av [avsnitt](customize-template.md#sections-or-groups):
   - Endast ett avsnitt kan användas, vilket genererar en enda uppsättning mallelement.

**Dimensioner som stöds**:

- Lodrät: (pixlar)
   - 300 x 600
   - 160 x 600 &#x200B;
- Vågrät: (pixlar)
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250 &#x200B;
- Egen: (pixlar)
   - 50 x 50 till 2 000 x 2 000

**Identifierade fältnamn**:

För banner- och visningsannonser genereras fältet `CTA` automatiskt. Använd innehållsplatshållare för följande fält:

- `headline`
- `sub_headline`
- `body`
- `image` (markerat från JPEG, PNG eller GIF)

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](customize-template.md#content-placeholders) .

>[!TAB LinkedIn och]

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Följ dessa designtips när du anpassar LinkedIn-annonsmallar så att de fungerar med GenStudio for Performance Marketing:

**Begränsningar**:

- Användning av [avsnitt](customize-template.md#sections-or-groups):
   - Endast ett avsnitt kan användas, vilket genererar en enda uppsättning mallelement.
- Största bildstorlek på 5 MB
- Max. rubrik 70 tecken
- Max introduktionstext 150 tecken

**Proportioner som stöds**:

- Fyrkant 1:1
   - dator eller mobil
   - Min: 360 x 360 pixlar
   - Max: 4 320 x 4 320 pixlar
- Vågrät 1,91:1
   - desktop
   - Min: 640 x 360 pixlar
   - Max: 7 680 x 4 320 pixlar
- Lodrät 1:1.91
   - mobil
   - Min: 360 x 640 pixlar
   - Max: 2 430 x 4 320 pixlar
- Lodrätt 2.3
   - mobil
   - Min: 360 x 640 pixlar
   - Max: 2 430 x 4 320 pixlar
- Vertikal 4.5 (rekommenderas)
   - mobil
   - Min: 360 x 640 pixlar
   - Max: 2 430 x 4 320 pixlar

**Identifierade fältnamn**:

För LinkedIn-annonser genereras fälten `headline`, `introductory_text` och `CTA` automatiskt. Använd innehållsplatshållare för följande fält:

- `image` (markerat från JPEG, PNG eller GIF)
- `on_image_text`

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](customize-template.md#content-placeholders) .

>[!ENDTABS]
