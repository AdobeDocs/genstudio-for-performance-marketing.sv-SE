---
title: Riktlinjer för e-postmallar
description: Följ vedertagna standarder när du använder e-postmallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Riktlinjer för e-postmallar

En e-postmall för marknadsföring fungerar som grund för visuellt engagerande och responsiva e-postkampanjer. I allmänhet kan du med HTML-mallar styra layout, typografi, färger och bilder så att de passar dina varumärkesriktlinjer. När du förbereder mallen för användning i GenStudio for Performance Marketing bör du använda semantiska HTML och infogad CSS för formatering och undvika skript och externa beroenden. Välstrukturerade HTML-mallar kan förbättra mottagarens upplevelse och förbättra leveransmöjligheterna och engagemangsfrekvensen.

Följ de här designmetoderna när du anpassar e-postmallar för att arbeta med GenStudio for Performance Marketing:

- Använda Adobe- eller Google-teckensnitt
- Använd rena och responsiva HTML och inline CSS
- Använd **inte** JavaScript
- Använd **inte** fast bredd i brödtext eller behållare
- Använd **inte** base64-kodning för bilder eftersom det kan öka mallstorleken avsevärt
- Den största filstorleken för HTML är 102 kB

## Identifierade fältnamn

GenStudio for Performance Marketing genererar automatiskt fältet `subject` för e-post. När du anpassar mallen använder du platshållare för innehåll för följande obligatoriska fält:

- `pre_header` (RTF är inte aktiverat)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (markerat från JPEG, PNG eller GIF)

Det högsta tillåtna antalet fält i en mall är 20. Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](/help/user-guide/content/customize-template.md#content-placeholders) .

## E-post med flera avsnitt

Med _Avsnitt_ kan du ordna innehåll i distinkta grupper, som har stöd för mer komplexa layouter. I Genstudio for Performance Marketing kan du definiera varje avsnitt med hjälp av en gruppnamnkonvention. Se [Anpassa mallavsnitt](/help/user-guide/content/customize-template.md#sections-or-groups).

Mallar med flera avsnitt kan ha 0, 2 eller 3 avsnitt:

- En grundläggande mall (nollavsnitt) kan generera en enda uppsättning mallelement, vilket inte kräver gruppnamnkonventionen.
- En komplex mall (flera avsnitt) kan generera upp till tre uppsättningar mallelement, vilket kräver att du följer gruppnamnkonventionen: (`groupname_fieldname`)

Exempelfältsnamn för två avsnitt:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

## Exempel på mallar

+++Exempel: E-postmall med ett avsnitt

Nedan följer ett grundläggande exempel på en HTML-mall för ett e-postmeddelande som innehåller ett avsnitt. Huvudet innehåller enkel, infogad CSS för formatering. Innehållet innehåller en `pre_header`, `headline` och `image` [platshållare](#content-placeholders) som GenStudio for Performance Marketing kan använda för att mata in innehåll under e-postgenereringsprocessen.

```html {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Exempel: E-postmall med flera avsnitt

Följande är samma HTML-mall i exemplet ovan, men med ytterligare två avsnitt. Huvudet innehåller infogad CSS för att formatera en grupp. Brödtexten använder två grupper med [platshållare för innehåll](#content-placeholders) som använder ett prefix.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
            .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
            }
            .pod h2 {
            color: #333;
            }
            .pod p {
                color: #666;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
