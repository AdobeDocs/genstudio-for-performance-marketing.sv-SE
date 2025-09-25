---
title: Metodtips för mallar
description: Följ vedertagna standarder när du använder mallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '384'
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

Det är viktigt att definiera tydliga riktlinjer för kanalerna för att säkerställa att det innehåll ni skapar är anpassat till varumärkets krav och mål. Med kanalriktlinjer kan du ange regler för element som ton, längd och format som används i mallen. Du kan till exempel ange ett maximalt antal tecken för brödtexten eller kräva ett visst call-to-action-format. Genom att ange dessa riktlinjer i förväg minskar du behovet av att skriva detaljerade anvisningar i varje AI-prompt, vilket effektiviserar innehållsgenereringsprocessen och säkerställer enhetlighet i alla e-postmeddelanden.

Granska och definiera varumärkets [kanalriktlinjer](/help/user-guide/guidelines/brands.md#channel-guidelines) för alla nyckelfält i mallen. Om du inte definierar några riktlinjer används [standardkanalriktlinjerna](/help/user-guide/guidelines/brands.md#default-channel-guidelines), vilket kanske inte helt återspeglar varumärkeskraven.

![Specifikationer för brödtext](/help/assets/channel-email-body.png)

Lär dig hur riktlinjerna [Varumärken, produkter och personer](/help/user-guide/guidelines/overview.md) påverkar det innehåll som genereras och hur du skräddarsyr dem för dina marknadsföringsmål.

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
