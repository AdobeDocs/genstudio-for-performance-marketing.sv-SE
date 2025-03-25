---
title: Anpassa en mall
description: Lär dig hur du anpassar och optimerar din mall för Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 0a1f13db9a976bac026f49e908b6b8c124bc5df7
workflow-type: tm+mt
source-wordcount: '1439'
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

GenStudio for Performance Marketing känner igen vissa [element](use-templates.md#template-elements) i en mall, men bara om du identifierar dem med ett [igenkänt fältnamn](#recognized-field-names).

I en HTML-malls huvud eller brödtext kan du använda syntaxen [!DNL Handlebars] för att infoga en innehållsplatshållare där du kräver att GenStudio for Performance Marketing ska fylla i mallen med faktiskt innehåll. GenStudio for Performance Marketing känner igen och tolkar platshållarna för innehåll baserat på det [identifierade _fältnamnet_](#recognized-field-names).

Du kan till exempel använda `{{ headline }}` med syntaxen [!DNL Handlebars] för att ange var rubriken i e-postmeddelandet ska placeras. GenStudio känner igen det här fältet, genererar en rubrik baserad på dina riktlinjer och frågekriterier och infogar rubriken här:

```handlebars
<div>{{ headline }}</div>
```

### Identifierade fältnamn

I följande tabell visas de fältnamn som GenStudio for Performance Marketing känner igen för att lägga till en platshållare i en mall. Lägg till de här fältnamnen med syntaxen [!DNL Handlebars] i mallen där du behöver GenStudio for Performance Marketing för att generera en viss typ av innehåll.

| Fält | Roll | Kanalmall |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Förrubrik | e-post |
| `{{headline}}` | Headline | e-post <br>Meta ad <br>Banner and Display ad <br>LinkedIn ad |
| `{{introductory_text}}` | Introduktionstext | LinkedIn och |
| `{{body}}` | Body copy | e-post <br>Meta ad <br>Banner and Display ad |
| `{{cta}}` | Uppmaning | e-post <br>Meta ad <br>Banner and Display ad <br>LinkedIn ad |
| `{{image}}` | Bild - välj från [!DNL Content] | e-post <br>Meta ad <br>Banner and Display ad <br>LinkedIn ad |
| `{{on_image_text}}` | På bildtext | Meta ad <br>LinkedIn ad |
| `{{link}}` | Anrop till åtgärd på bild<br>Se [Länka till bild](#link-on-image). | e-post |
| `{{brand_logo}}` | Logotyp för markerat varumärke<br>Se [Fältnamn för logotyp för varumärke](#brand-logo-field-name). | e-post<br>Meta och <br>LinkedIn |

GenStudio for Performance Marketing fyller i vissa fält automatiskt i följande mallar:

- **E-postmallen** kräver inte att du identifierar fältet `subject`
- **Meta ad-mallen** kräver inte att du identifierar fälten `headline`, `body` och `CTA`
- **Banderoll och mall för visningsannons** kräver inte att du identifierar fältet `CTA`
- **LinkedIn-annonsmallar** kräver inte att du identifierar fälten `headline`, `introductory_text` och `CTA`

>[!WARNING]
>
>För Instagram-annonser visas den genererade rubriken inte i den slutliga versionen.

Det finns en gräns på 20 fält när en mall överförs till GenStudio for Performance Marketing. Eftersom fältet `subject` genereras automatiskt i ett e-postmeddelande räknas det som ett fält. Det innebär att 19 fält tillåts i en e-postmall.

>[!TIP]
>
>Du kan verifiera mallen med [mallförhandsgranskning](#template-preview) i GenStudio for Performance Marketing.

### Utmaningar

En Call to action (CTA) innehåller en fras och en länk. För att funktionerna _[!UICONTROL Rephrase]_och_[!UICONTROL Add link]_ ska fungera korrekt under genereringsprocessen för varianter måste du ta med platshållare för länken och frasen i mallen.

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

### Länka till bild

Du kan anpassa din e-postmall så att andra kan lägga till en länk till en bild. På samma sätt som för länken CTA använder du följande vägledning för att tillämpa en `link`-platshållare för en bildtagg:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="description"></a>
```

I detta exempel:

- `{{link}}` är en platshållare för den faktiska URL:en.
- `src="image-source.jpg"` ska ersättas med den faktiska URL-adressen för bildkällan.
- `alt="description"` innehåller en alternativ text för bilden, vilket är användbart för hjälpmedel och SEO.

### Fältnamn för märkeslogotyp

För närvarande kan du inte välja logotypen för mallöverföringen. I följande exempel visas två metoder som villkorligt återger varumärkeslogotypen. Varje metod verifierar källan, ger en standardbild eller alternativ bild om logotypen inte är tillgänglig och använder en stil:

**Exempel 1**: Använder [!DNL Handlebars] villkor för inbyggda hjälpredor direkt i HTML-attributet `img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Exempel 2**: Använder [!DNL Handlebars] inbyggd villkorssats för att kapsla in HTML `img` -taggen:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

### Manuella fältnamn

Alla andra fältnamn behandlas som manuellt ifyllda fält. Du kanske vill reservera ett avsnitt för sidfotsinnehåll.

Om du vill skapa ett redigerbart avsnitt lägger du till dubbla hakparenteser runt avsnittsnamnet:

```html
<tbody>
    <tr>
        <td>
            <p><span class="s1">{{ footerLegal }}</span></p>
        </td>
    </tr>
</tbody>
```

## Avsnitt eller grupper

_Avsnitt_ informerar GenStudio for Performance Marketing om att fälten i det här avsnittet kräver hög grad av konsekvens. Genom att etablera relationen kan AI generera innehåll som matchar de kreativa elementen i avsnittet.

Använd ett prefix som du väljer i fältnamnet för att ange att ett fält är en del av ett avsnitt eller en grupp. Använd ett fältnamn (`headline`, `body`, `image` eller `cta`) efter understrecket (`_`).

- _Korrigera_ (??): `pod1_body`
- _Felaktigt_ ( ❌): `pod1_link`

Varje avsnitt kan bara använda en av varje fälttyp. Följande fält tillhör till exempel avsnittet `pod1`:

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

På grund av den här regeln kan avsnitten inte kapslas.

Varje malltyp, som e-post eller Meta-annons, har kanalspecifika begränsningar för användning av avsnitt. Se [kanalspecifika riktlinjer](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) i avsnittet _Bästa metoder för att använda mallar_.

En e-postmall kan t.ex. innehålla upp till tre avsnitt. Därför kan du ha tre rubrikavsnitt och innehållsavsnitt:

- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing förstår att `pod1_headline` är närmare relaterat till `pod1_body` än till `pod2_body`.

Se [Strukturerade uppmaningar](/help/user-guide/effective-prompts.md#structured-prompts) om hur du skapar en prompt som genererar varierande innehåll för varje avsnitt i ett e-postmeddelande med flera avsnitt.


## Förhandsgranska mall

När du [överför en mall](use-templates.md#upload-a-template) söker GenStudio for Performance Marketing igenom HTML-filen efter identifierade fält. Använd förhandsgranskningen för att granska dina [mallelement](use-templates.md#template-elements) och bekräfta att du har identifierat dem korrekt med de [igenkända fältnamnen](#recognized-field-names).

Exempel på Förhandsgranska för en e-postmall:

![Förhandsgranskningsfält har identifierats](/help/assets/template-detected-fields.png "Kontrollera identifierade fält"){zoomable="yes"}

Se [Mallkodredigerare](/help/user-guide/content/code-editor.md).

### Förhandsgranska kontroll

Du kan styra visningen av specialinnehåll med hjälp av inbyggda hjälpredor (specialuttryck i mallspråket [!DNL Handlebars] som utför vissa åtgärder). Du kan till exempel lägga till en villkorssats som lägger till spårningsparametrar till länkar i den exporterade mallen samtidigt som förhandsgranskningslänkarna hålls rena.

Värdet `_genStudio.browser` anges när en mall återges och värdet `genStudio.export` anges när en mall exporteras. Du kan välja att ta med visst innehåll högst upp i ett e-postmeddelande med en villkorlig omslutning, till exempel när mallen används för export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ett annat exempel kan vara att förhindra att spårningskoder används när en mall förhandsgranskas i GenStudio for Performance Marketing. I följande exempel visas hur du lägger till spårningsparametrar till länkar i den exporterade mallen, samtidigt som du håller förhandsgranskningslänkarna rena:

```html
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
    <body>{{ pre_header }}
        <div class="container">
            <h1>{{ headline }}</h1>
            <p><a href="{{ link }}">
            <img alt="{{ headline }}"
                    src="{{ image }}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{ body }}</p>
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
    <body>{{ pre_header }}
        <div class="container">
            <h1>{{ headline }}</h1>
            <p>{{ body }}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{ pod1_headline }}</h2>
                <p><img alt="{{ headline }}" src="{{ pod1_image }}" width="200" height="200" border="0"></p>
                <p>{{ pod1_body }}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{ pod2_headline }}</h2>
                <p><img alt="{{ headline }}" src="{{ pod2_image }}" width="200" height="200" border="0"></p>
                <p>{{ pod2_body }}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++Exempel: Meta ad template

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
            <img src="{{ image }}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{ on_image_text }}</div>
        </div>
    </body>
</html>
```

+++
