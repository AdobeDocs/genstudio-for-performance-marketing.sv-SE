---
title: Riktlinjer för LinkedIn-mallar
description: Följ vedertagna standarder när du använder LinkedIn-mallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# LinkedIn-mallriktlinjer

LinkedIn-mallar är ett strukturerat sätt att skapa och anpassa annonskampanjer för LinkedIn-kampanjer. Riktlinjerna säkerställer att era annonser uppfyller LinkedIn:s specifikationer samtidigt som den kreativa processen i GenStudio for Performance Marketing effektiviseras. Den här guiden hjälper dig att förbereda dig för enhetlig varumärkesprofilering och effektiva prestanda på LinkedIn-datorplattformar och mobila plattformar.

Följ dessa designtips när du anpassar LinkedIn-annonsmallar så att de fungerar med GenStudio for Performance Marketing:

- Exakt ett bildfält krävs
- Största bildstorlek på 5 MB
- Max. rubrik 70 tecken
- Max introduktionstext 150 tecken
- Endast ett avsnitt kan användas och en uppsättning mallelement genereras

## Identifierade fältnamn

När du anpassar din LinkedIn-mall kan du lägga till platshållare för innehållet i följande obligatoriska fält:

- `image` (obligatoriskt, markerat från JPEG, PNG eller GIF)
- `on_image_text` (text som visas över bilden)

GenStudio for Performance Marketing genererar automatiskt följande fält. Du behöver inte använda platshållare för innehåll för:

- `headline`
- `introductory_text`
- `cta` (Call to action)

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](/help/user-guide/content/customize-template.md#content-placeholders) .

## Proportioner som stöds

| Proportioner | Plattform | Minsta storlek (px) | Maximal storlek (px) | Anteckningar |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| Fyrkant 1:1 | Dator, mobil | 360 x 360 | 4320 x 4320 | Mest mångsidiga. Perfekt för enhetligt utseende på olika enheter och enheter. |
| Vågrät 1.91:1 | Skrivbord | 640 x 360 | 7680 x 4320 | Standardliggande format. Används vanligen för sponsrat innehåll och nyhetsfeed-annonser. |
| Lodrätt 1:1.91 | Mobil | 360 x 640 | 2430 x 4320 | Helt lodrätt format. Optimerat för mobilvisning, med större skärmnärvaro. |
| Lodrät 2:3 | Mobil | 360 x 640 | 2430 x 4320 | Något mindre högt än 1:1.91. Bra för kampanjer som sätter mobilen först. |
| Lodrät 4:5 | Mobil | 360 x 640 | 2430 x 4320 | Rekommenderas för mobiler. Balanserar synlighet och innehåll, vilket ofta ger större effekt. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
