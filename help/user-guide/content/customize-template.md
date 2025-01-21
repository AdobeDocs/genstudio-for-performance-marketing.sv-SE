---
title: Anpassa en mall
description: Lär dig hur du anpassar och optimerar din mall för Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 62ab3849296195ca4d9525cb5688f74ce8bede54
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# Anpassa en mall

Du kan anpassa en mall för användning i GenStudio for Performance Marketing genom att infoga platshållare för innehåll, eller fält, som används av den generativa AI-filen för att infoga innehåll.

I de följande avsnitten beskrivs hur du anpassar dina HTML-mallar för GenStudio for Performance Marketing med hjälp av mallspråket _[!DNL Handlebars]_. Syntaxen [!DNL Handlebars] använder vanlig text med dubbla klammerparenteser som innehållsplatshållare. Se [Vad är  [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) i_ Handlebars språkguide _om du vill lära dig hur du förbereder mallen.


När mallen är klar kan du [överföra den till GenStudio for Performance Marketing](use-templates.md#upload-a-template) och börja generera anpassade e-postmeddelanden baserat på din anpassade mall.

>[!TIP]
>
>Följ [hjälpmedelsriktlinjerna](accessibility-for-templates.md) och [bästa praxis](/help/user-guide/content/best-practices-for-templates.md) så att du kan nå ut till fler av din publik och skapa en optimal upplevelse.

## Platshållare för innehåll

GenStudio for Performance Marketing känner igen vissa [element](use-templates.md#template-elements) i en mall, men bara om du identifierar dem med ett känt fältnamn.

I mallens huvud eller brödtext kan du använda syntaxen [!DNL Handlebars] som en innehållsplatshållare där du kräver att GenStudio for Performance Marketing ska fylla i mallen med faktiskt innehåll. GenStudio for Performance Marketing känner igen och tolkar platshållarna för innehåll baserat på det [identifierade _fältnamnet_](#recognized-field-names).

Du kan till exempel använda `{{ headline }}` med syntaxen [!DNL Handlebars] för att ange var rubriken i e-postmeddelandet ska placeras:

```handlebars
<div>{{headline}}</div>
```

### Identifierade fältnamn

I följande tabell visas de fältnamn som GenStudio for Performance Marketing har identifierat för ifyllning i mallar. Lägg till de här fältnamnen med syntaxen [!DNL Handlebars] i mallen där du behöver GenStudio for Performance Marketing för att generera innehåll.

| Fält | Roll | Kanalmall |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | Förrubrik | e-post |
| `{{headline}}` | Headline | e-post <br>Meta ad <br> Visa annons |
| `{{body}}` | Body copy | e-post <br>Meta ad <br> Visa annons |
| `{{cta}}` | Uppmaning | e-post <br>Meta ad <br> Visa annons |
| `{{on_image_text}}` | På bildtext | Meta ad |
| `{{image}}` | Bild - välj från innehåll | e-post <br>Meta ad <br> Visa annons |
| `{{brand_logo}}` | Logotyp för markerat varumärke<br>Se [Fältnamn för logotyp för varumärke](#brand-logo-field-name) för rekommenderad användning. | e-post<br>Meta ad |

GenStudio for Performance Marketing fyller i vissa fält automatiskt i följande mallar:

- **E-postmallen** kräver inte att du identifierar fältet `subject`
- Mallen **Metaannonser** kräver inte att du identifierar fälten `headline`, `body` och `CTA`
- **Mallen för visningsannonser** kräver inte att du identifierar fältet `CTA`

>[!WARNING]
>
>För Instagram-annonser visas den genererade rubriken inte i den slutliga versionen.

Det finns en gräns på 20 fält när en mall överförs till GenStudio for Performance Marketing. Eftersom fältet `subject` genereras automatiskt i ett e-postmeddelande räknas det som ett fält. Det innebär att 19 fält tillåts i en e-postmall.

>[!TIP]
>
>Du kan verifiera mallen med [mallförhandsgranskning](#template-preview) i GenStudio for Performance Marketing.

#### Fältnamn för märkeslogotyp

För närvarande kan du inte välja logotypen för mallöverföringen. I följande exempel visas två metoder som villkorligt återger varumärkeslogotypen. Varje metod verifierar källan, ger en standardbild eller alternativ bild om logotypen inte är tillgänglig och använder en stil:

**Exempel 1**: Använder [!DNL Handlebars] villkor för inbyggda hjälpredor direkt i HTML-attributet `img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Exempel 2**: Använder [!DNL Handlebars] inbyggd villkorssats för att kapsla in HTML-taggen `img`:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Manuella fältnamn

Alla andra fältnamn behandlas som manuellt ifyllda fält.

Om du vill skapa ett redigerbart avsnitt lägger du till dubbla hakparenteser runt avsnittsnamnet:

```handlebars
{{customVariable}}
```

### Avsnitt eller grupper

_Avsnitt_ informerar GenStudio for Performance Marketing om att fälten i det här avsnittet kräver hög grad av konsekvens. Genom att etablera relationen kan AI generera innehåll som matchar de kreativa elementen i avsnittet.

Använd ett prefix som du väljer i fältnamnet för att ange att ett fält är en del av ett avsnitt eller en grupp. Använd ett fältnamn (`headline`, `body`, `image` eller `cta`) efter understrecket (`_`). Följande rubrik och brödtext tillhör till exempel avsnittet `pod1`:

- `pod1_headline`
- `pod1_body`

Varje avsnitt kan bara använda en av varje fälttyp. I exemplet ovan kan avsnittet `pod1` bara använda ett `pod1_headline`-fält. På grund av den här regeln kan avsnitten inte kapslas.

Varje malltyp, som e-post eller Meta-annons, har kanalspecifika begränsningar för användning av avsnitt. Se [kanalspecifika riktlinjer](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) i avsnittet _Bästa metoder för att använda mallar_.

En e-postmall kan t.ex. innehålla upp till tre avsnitt. Därför kan du ha tre rubrikavsnitt och innehållsavsnitt:

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing förstår att `pod1_headline` är närmare relaterat till `pod1_body` än till `pod2_body`.

Se [Strukturerade uppmaningar](/help/user-guide/effective-prompts.md#structured-prompts) om du vill lära dig hur du skapar en prompt som genererar varierande innehåll för varje avsnitt i ett e-postmeddelande.

### Utmaningar

En Call to action (CTA) innehåller en fras och en länk. För att CTA _[!UICONTROL Rephrase]_- och_[!UICONTROL Add link]_-funktionerna ska fungera korrekt under genereringsprocessen för varianter måste du ta med platshållare för länken och frasen i mallen.

Använd följande vägledning för att konfigurera CTA-platshållare:

- CTA omfras finns och länken kan redigeras

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTA omfras är tillgänglig, men länken är **inte** redigerbar eftersom den faktiska länken anges i mallen

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- CTA-länken kan redigeras, men omfrasen är **inte** tillgänglig eftersom frasen anges i mallen

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing kan även tillhandahålla olika uppmaningar att vidta åtgärder. Se [Ändra uppmaning](/help/user-guide/create/manage-variants.md#revise-call-to-action).

## Förhandsgranska mall

När du [överför en mall](use-templates.md#upload-a-template) söker GenStudio for Performance Marketing igenom filen HTML efter identifierade fält. Använd förhandsgranskningen för att granska dina [mallelement](use-templates.md#template-elements) och bekräfta att du har identifierat dem korrekt med de [igenkända fältnamnen](#recognized-field-names).

Exempel på Förhandsgranska för en e-postmall:

![Förhandsgranskningsfält har identifierats](/help/assets/template-detected-fields.png){width="650"}

### Förhandsgranska kontroll

Du kan styra visningen av specialinnehåll med hjälp av inbyggda hjälpredor (specialuttryck i mallspråket [!DNL Handlebars] som utför vissa åtgärder). Du kan till exempel lägga till en villkorssats som lägger till spårningsparametrar till länkar i den exporterade mallen samtidigt som förhandsgranskningslänkarna hålls rena.

Värdet `_genStudio.browser` anges när en mall återges och värdet `genStudio.export` anges när en mall exporteras. Du kan välja att ta med visst innehåll högst upp i ett e-postmeddelande med en villkorlig omslutning, till exempel när mallen används för export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ett annat exempel kan vara att förhindra att spårningskoder används när en mall förhandsgranskas i GenStudio for Performance Marketing. I följande exempel visas hur du lägger till spårningsparametrar till länkar i den exporterade mallen, samtidigt som du håller förhandsgranskningslänkarna rena:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Statiskt innehåll

E-post- och metamallar länkar ofta till bilder och CSS-filer på andra domäner. När GenStudio for Performance Marketing genererar miniatyrbilder för mallförhandsvisningar eller de upplevelser som härletts från dem, valideras innehållskällan och en kopia bäddas in för förhandsgranskning.

Externa filer bäddas bara in tillfälligt i syfte att skapa mallförhandsvisningen, vilket gör att förhandsvisningen korrekt återger innehållet så som det ser ut när du skapar mallen. Dessa externa filer lagras **inte** permanent i GenStudio for Performance Marketing. När mallförhandsgranskningen har skapats fortsätter GenStudio for Performance Marketing att referera till den ursprungliga källlänken som finns i mallen.

### Uppdatera innehåll

Om källan ändras efter att den inledande förhandsgranskningen har skapats använder du funktionen [Uppdatera](/help/user-guide/content/use-templates.md#refresh-template) för att uppdatera mallförhandsvisningen med den senaste versionen av innehållet från de externa källorna.

## Exempel på mallar

+++Exempel: E-postmall med ett avsnitt

Nedan följer ett grundläggande exempel på en HTML-mall för ett e-postmeddelande som innehåller ett avsnitt. Huvudet innehåller enkel, infogad CSS för formatering. Innehållet innehåller en `pre-header`, `headline` och `image` [platshållare](#content-placeholders) som GenStudio for Performance Marketing kan använda för att mata in innehåll under e-postgenereringsprocessen.

```handlebars {line-numbers="true" highlight="13"}
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
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Exempel: E-postmall med flera avsnitt

Följande är samma HTML-mall i exemplet ovan, men med ytterligare två avsnitt. Huvudet innehåller infogad CSS för att formatera en grupp. Brödtexten använder två grupper med [platshållare för innehåll](#content-placeholders) som använder ett prefix.

```handlebars {line-numbers="true" highlight="33"}
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
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Exempel: Meta ad template

Följande är ett grundläggande exempel på en Meta-annonsmall. Huvudet innehåller infogad CSS för formatering. Brödtexten använder [platshållare för innehåll](#content-placeholders) med ett prefix.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
