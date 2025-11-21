---
title: Metodtips för mallar
description: Följ vedertagna standarder när du använder mallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 71b46454fa6fe2037ea6b103c0dfeedad74b8919
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Bästa tillvägagångssätt för att använda mallar

Mallar minskar avsevärt den tid och det arbete som krävs för att generera nytt innehåll genom att tillhandahålla en startpunkt med förkonfigurerade layouter och designelement.

Följ följande rekommendationer när du använder mallar med GenStudio for Performance Marketing:

1. Lär dig mer om [mallelement](#know-about-template-elements)
1. Konfigurera [kanalriktlinjer](#configure-channel-guidelines) för effektiv personalisering av innehåll
1. Designa med [tillgänglighetsstandarder](accessibility-for-templates.md) för en optimal upplevelse
1. Följ [kanalspecifika riktlinjer för mallar](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Lär dig grunderna för mallelement och procedurer i [Arbeta med mallar](use-templates.md). Och fördjupa dig i [att anpassa en mall](customize-template.md) för specifika instruktioner som kan användas i nästa kampanj.

## Använda rätt mallelement

Varje malltyp använder olika element för att skapa en struktur för kanalspecifik innehållsutveckling. [Bekanta dig med delarna i en mall](use-templates.md#template-elements) och inkludera de bästa elementen för ditt innehåll och din malltyp.

När du anpassar mallen ska du använda fältnamnen i stället för dessa element där du behöver GenStudio for Performance Marketing för att generera innehåll.

Se [Mallelement](use-templates.md#template-elements).

## Använda platshållartext i mallar

Platshållartext kan hjälpa till att definiera syntax eller struktur för innehåll som ska fyllas i senare i en mall av en användare. Exempel: {first_name}.{last_name}@email.etc. för att definiera en e-postadress. Vissa vanliga avgränsare är dock redan reserverade för andra betydelser i GenStudio for Performance Marketing:

❌ &lt; > - Används för HTML-taggar.
❌ {{ }}{{ }} - Används för Handlebar-uttryck.

Använd klammerparenteser (raka eller klammerparenteser) för att ange platshållartext, så att du slipper trassel med befintliga taggar.

✅ {first_name} - Platshållare för förnamn.

## Konfigurera kanalriktlinjer

Det är viktigt att definiera tydliga riktlinjer för kanalerna för att säkerställa att det innehåll ni skapar är anpassat till varumärkets krav och mål. Med kanalriktlinjer kan du ange regler för element som ton, längd och format som används i mallen. Du kan till exempel ange ett maximalt antal tecken för brödtexten eller kräva ett visst call-to-action-format. Genom att ange dessa riktlinjer i förväg minskar du behovet av att skriva detaljerade anvisningar i varje AI-prompt, vilket effektiviserar innehållsgenereringsprocessen och säkerställer enhetlighet i alla e-postmeddelanden.

Granska och definiera varumärkets [kanalriktlinjer](/help/user-guide/guidelines/brands.md#channel-guidelines) för alla nyckelfält i mallen. Om du inte definierar några riktlinjer används [standardkanalriktlinjerna](/help/user-guide/guidelines/brands.md#default-channel-guidelines), vilket kanske inte helt återspeglar ditt varumärkes krav.

![Specifikationer för brödtext](/help/assets/channel-email-body.png)

Lär dig hur riktlinjerna [Varumärken, produkter och personer](/help/user-guide/guidelines/overview.md) påverkar det innehåll som genereras och hur du skräddarsyr dem för dina marknadsföringsmål.

## Överföra bilder för mallar

Bilder som används i mallar ska komma från innehållsdatabasen och måste överföras korrekt för att bilden ska visas korrekt.

När en mall innehåller en bild från kant till kant (helt utfall) ändras storleken automatiskt på den markerade bilden så att den passar de fullständiga malldimensionerna. Om bilden inte matchar mallens proportioner beskärs bilden så att den passar mallens dimensioner och visas eventuellt inte som förväntat.

Det finns ingen autopassningsfunktion för bilder som ingår i mallar.

För att lösa bildbeskärning måste användarna definiera bildens proportioner som ska användas i mallen när den överförs till innehållsdatabasen. När du överför en godkänd mall:

1. [Fortsätt genom mallöverföringsprocessen](/help/user-guide/templates/use-templates.md#add-a-template) tills du når sidan **[!UICONTROL Add details]**.

2. Definiera bildens proportioner som ska användas i mallen i **[!UICONTROL Ad width (px)]** och **[!UICONTROL Ad height (px)]**. Detta definierar bildfönstret för den del av mallen som visar bilden.

3. I avsnittet **[!UICONTROL More details]** markerar du listrutan **[!UICONTROL Image size]** och väljer _Beskär till en fast storlek_.
   ![Beskuren till fast storlek](images/crop-to-fixed-size.png "Beskuren till fast storlek"){width="80%"}

Så här avgör du en bilds storlek och proportioner i webbläsaren:

1. Granska bilden.
   - I Windows/Linux:
      - Tryck på F12.
   - På macOS:
      - Tryck på Kommando + Alt + I.

1. Hovra över bilden.

1. Observera proportionerna. Använd detta för att definiera bildens proportioner i mallen.

När dessa detaljer inte används vid överföring antas bilden vara mallens hela proportioner och bilder som inte matchar proportionerna visas som beskurna.

![Bild beskuren i en bildskärm och](images/cropped-display.png "Bildbeskärning"){width="60%"}

**❌Beskuren bild i en visningsannonsmall**

![Bilden visas i en visningsannons](images/full-fit.png "Bilden visas i visningsannons"){width="60%"}

**✅Bilden visas helt**

## Följ kanalspecifika riktlinjer för mallar

När du skapar mallar måste du se till att de uppfyller de specifika kraven för den avsedda kanalen. Skapa mallar som passar de layoutkrav och visuella krav som gäller för varje kanal. Det finns allmänna riktlinjer som gäller för alla mallar, till exempel:

- Använd rena och responsiva HTML och inline CSS
- Använda Adobe- eller Google-teckensnitt
- Använd **inte** JavaScript

{{note-css-effects}}

Se fler tips och begränsningar när du arbetar med varje malltyp för att säkerställa optimala prestanda:

- [E-post](/help/user-guide/templates/email-template.md)
- [Visa och skapa banners](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta annonser](/help/user-guide/templates/meta-template.md)
