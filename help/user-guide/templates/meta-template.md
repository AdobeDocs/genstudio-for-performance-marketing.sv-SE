---
title: Riktlinjer för metadata och mallar
description: Följ vedertagna standarder när du använder metadatamallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Riktlinjer för metadata och mallar

Med metadatamallar kan ni skapa visuellt enhetliga och effektiva annonser på olika Meta-plattformar. Genom att följa rekommenderade designrutiner och använda fält som stöds kan du se till att mallarna är optimerade för GenStudio for Performance Marketing. Den här guiden förklarar hur du strukturerar, anpassar och förbereder mallar för Meta-annonser för smidig integrering och slagkraftiga resultat.

Följ de här designmetoderna när du anpassar metadatamallar för GenStudio for Performance Marketing:

- Använd 360 pixlar bred för kolumnlayouter
- Använd en lägsta upplösning på 1 080 x 1 080 pixlar för bilder
- Exakt ett bildfält krävs
- Använd den relativa teckenstorleken **inte**
- Definiera **inte** visningsruta
- Använd **inte** JavaScript
- Åsidosätt **inte** ett HTML-element i CSS
- Använd taggen `<img>` i stället för `background-image`
- Använd maskning för att förbättra textläsbarheten över bakgrundsbilder
- Endast ett avsnitt kan användas och en uppsättning mallelement genereras

## Identifierade fältnamn

När du anpassar mallen Meta ads ska du lägga till platshållare för innehållet i följande obligatoriska fält:

- `image` (obligatoriskt, markerat från JPEG, PNG eller GIF)
- `on_image_text` (text som visas över bilden)

GenStudio for Performance Marketing genererar automatiskt följande fält. Du behöver inte använda platshållare för innehåll för:

- `headline`
- `body`
- `cta`

Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](/help/user-guide/content/customize-template.md#content-placeholders) .

## Proportioner som stöds

| Proportioner | Mått (pixlar) | Anteckningar |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Fyrkant 1:1 | 1 080 x 1 080 | Standard för de flesta metaersättningar. Rekommenderas för bred kompatibilitet. |
| Stående 4:5 | 1 080 x 1 350 | Optimerat för mobila flöden, ger mer vertikalt utrymme. |
| Artikel 9:16 | 1 080 x 1 920 | Idealiskt för Stories och Reels; fyller hela den mobila skärmen. |
| Liggande 1,91:1 | 1 080 x 566 | Passar bäst för länkannonser och nyhetsfeedplaceringar, brett format. |
| Egen | Minst 50 x 50 (bredd) | Använd bara om det behövs. Kan leda till beskärning eller skalförändring. |

Om annonsen inte är utformad i någon av dessa proportioner beskärs bilden automatiskt i lämplig storlek av GenStudio for Performance Marketing.

## Exempel på mall

+++Exempel: Meta ad template

<!-- Does this need to be a precise size? -->

Följande är ett grundläggande exempel på en Meta-annonsmall. Huvudet innehåller infogad CSS för formatering. Brödtexten använder [platshållare för innehåll](#content-placeholders), till exempel `image` och `on_image_text`, för att ange var GenStudio for Performance Marketing kan generera innehåll.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
