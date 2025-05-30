---
title: Riktlinjer för annonseringsmallar
description: Följ vedertagna standarder när du använder mallar för displayannonser och banderoller med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
source-git-commit: 78313c2a2177a2ccb39e37a87ca3c657e7906d0a
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Riktlinjer för annonseringsmallar

Visningsmallar är fördesignade layouter som används för att skapa visuellt engagerande banners och displayannonser. De utgör ett flexibelt ramverk för att införliva bilder, text och call to action, vilket ger enhetlighet och effektivitet vid produktion av olika annonsvarianter. När du förbereder mallen för användning i GenStudio for Performance Marketing måste du se till att alla resurser är optimerade för webbvisning och att de uppfyller de filformat och storlekar som krävs.

Följ de här designmetoderna när du anpassar mallar för banners och displayannonser så att de fungerar med GenStudio for Performance Marketing:

- Använda Adobe- eller Google-teckensnitt
- Förbered resurser som visas bra i tunna dimensioner
- Exakt ett bildfält krävs
- Använd **inte** inbäddade eller kodade bakgrundsbilder
- Använd bakgrundsbilder (`image` fält) överförda till GenStudio for Performance Marketing innehållsdatabas
- Använd **inte** JavaScript
- Endast ett avsnitt kan användas och en uppsättning mallelement genereras

## Identifierade fältnamn

För banner- och visningsannonser genererar GenStudio for Performance Marketing automatiskt fältet `cta`. När du anpassar mallen använder du platshållare för innehåll för följande obligatoriska fält:

- `headline`
- `sub_headline`
- `body`
- `image` (obligatoriskt, markerat från JPEG, PNG eller GIF)

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](/help/user-guide/content/customize-template.md#content-placeholders) .

## Dimensioner som stöds

Bredd x höjd (pixlar) måste anges.

| Orientering | Mått (pixlar) | Anteckningar |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Lodrätt | 300 x 600<br>160 x 600 | Vanligt för skyskrapa och halvsidesbanderoller |
| Vågrät | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standardstorlek för rankbräde, medelstor rektangel och banderoll |
| Egen | 50 x 50 till 2 000 x 2 000 | Används för icke-standardiserade eller unika placeringar; kontrollera plattformsbegränsningar |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
