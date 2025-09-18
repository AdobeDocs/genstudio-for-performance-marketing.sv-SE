---
title: Riktlinjer för e-postmall
description: Följ vedertagna standarder när du använder e-postmallar med Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 49d8d5daa2f3c93c18cd9132dab5207871b51237
workflow-type: tm+mt
source-wordcount: '441'
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

När du anpassar din e-postmall använder du innehållsplatshållare för följande obligatoriska fält:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (markerat från JPEG, PNG eller GIF)

GenStudio for Performance Marketing genererar automatiskt följande fält. RTF är inte aktiverat. Du behöver inte använda platshållare för innehåll för:

- `pre_header`
- `subject`

Det högsta tillåtna antalet fält i en mall är 20. Mer information om hur du använder fältnamn i mallar finns i [Innehållsplatshållare](/help/user-guide/content/customize-template.md#content-placeholders) .

## E-post med flera avsnitt

Med _Avsnitt_ kan du ordna innehåll i distinkta grupper med stöd för mer komplexa layouter. I GenStudio for Performance Marketing kan du definiera varje avsnitt med hjälp av en gruppnamnkonvention. Se [Anpassa mallavsnitt](/help/user-guide/content/customize-template.md#sections-or-groups).

Mallar med flera avsnitt kan ha 0, 2 eller 3 avsnitt:

- En grundläggande mall (noll avsnitt) kan generera en enda uppsättning mallelement, vilket inte kräver gruppnamnkonventionen.
- En komplex mall (flera avsnitt) kan generera upp till tre uppsättningar mallelement, vilket kräver att du följer gruppnamnkonventionen: `<groupname_fieldname>`.
- Om du använder flera avsnitt fylls inte element som är fristående utanför ett avsnitt i.

Här är exempel på fältnamn som använder gruppnamnkonventionen för två avsnitt:

- I avsnitt 1:`pod1_headline`, `pod1_body`, `pod1_cta`
- I avsnitt 2:`pod2_headline`, `pod2_body`, `pod2_cta`

## Exempel på mallar

+++Exempel: E-postmall med ett avsnitt

Här är ett grundläggande exempel på en e-postmall från HTML med ett avsnitt. `<head>` innehåller enkel infogad CSS för formatering, och `<body>` använder platshållare för innehåll som `pre_header`, `headline`, `sub_headline`, `body`, `cta` och `image` med länk och. Med dessa platshållare kan GenStudio for Performance Marketing lägga in dynamiskt innehåll när e-postmeddelanden skapas.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++Exempel: E-postmall med flera avsnitt

Här är samma HTML-mall i exemplet ovan, men med ytterligare två avsnitt. Huvudet innehåller infogad CSS för att formatera en grupp. Brödtexten använder två grupper med [platshållare för innehåll](#content-placeholders) som använder ett prefix.

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
