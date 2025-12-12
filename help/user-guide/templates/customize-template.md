---
title: Anpassa en mall
description: Lär dig hur du anpassar din HTML-mall med hjälp av platshållare för innehåll som känns igen av Adobe GenStudio for Performance Marketing generativa AI.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 4f3d8558f37656ccfc67b592e0bb9e90c30a7963
workflow-type: tm+mt
source-wordcount: '1630'
ht-degree: 0%

---

# Anpassa en mall

Du kan anpassa en mall för användning i GenStudio for Performance Marketing genom att infoga platshållare för innehåll, eller fält, som används av den generativa AI-filen för att infoga innehåll.

I de följande avsnitten beskrivs hur du anpassar dina HTML-mallar för GenStudio for Performance Marketing med hjälp av mallspråket _[!DNL Handlebars]_. Syntaxen [!DNL Handlebars] använder vanlig text med dubbla klammerparenteser som innehållsplatshållare. Se [Vad är  [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) i_ Handlebars språkguide _om du vill lära dig hur du förbereder mallen.

När mallen är klar kan du [överföra den till GenStudio for Performance Marketing](use-templates.md#upload-a-template) och börja generera anpassade e-postmeddelanden baserat på din anpassade mall.

Följ [hjälpmedelsriktlinjerna](accessibility-for-templates.md) och [bästa praxis](/help/user-guide/templates/best-practices-for-templates.md) så att du kan nå ut till fler av din publik och skapa en optimal upplevelse.

## Platshållare för innehåll

>[!TIP]
>
>Platshållare för innehåll är **inte** samma som platshållartext i innehåll som ska fyllas i senare av en användare. Se mer om [att använda platshållartext i mallar](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates).

GenStudio for Performance Marketing känner igen vissa typer av innehåll eller [element](use-templates.md#template-elements) i en mall, men bara om du identifierar dem med ett [igenkänt fältnamn](#recognized-field-names).

I en HTML-malls huvud eller brödtext kan du använda syntaxen [!DNL Handlebars] för att infoga en innehållsplatshållare där du kräver att GenStudio for Performance Marketing ska fylla i mallen med faktiskt innehåll. GenStudio for Performance Marketing känner igen och tolkar dessa platshållare baserat på det [identifierade _fältnamnet_](#recognized-field-names). Varje fältnamn är kopplat till särskilda regler och beteenden som bestämmer hur innehåll skapas och infogas i mallen.

Du kan till exempel använda `{{headline}}` med syntaxen [!DNL Handlebars] för att ange var rubriken i e-postmeddelandet ska placeras. GenStudio känner igen det här fältet, genererar en rubrik baserad på dina riktlinjer och frågekriterier och infogar rubriken här:

```handlebars
<div>{{headline}}</div>
```

### Identifierade fältnamn

I följande tabell visas de fältnamn som GenStudio for Performance Marketing känner igen för att lägga till en platshållare i en mall. Varje fält följer specifika riktlinjer för kanaler, instruktioner för programmet för livslångt lärande och rollbaserade regler. Lägg till de här fältnamnen med syntaxen [!DNL Handlebars] i mallen där du behöver GenStudio for Performance Marketing för att generera en viss typ av innehåll.

| Fält | Roll | Kanalmall |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Förrubrik | e-post |
| `{{headline}}` | Headline | e-post <br>Meta och <br>Banner och Display och <br>LinkedIn |
| `{{sub_headline}}` | Underrubrik | e-post<br>Banderoll och visningsannons |
| `{{introductory_text}}` | Introduktionstext | LinkedIn och |
| `{{body}}` | Body copy | e-post <br>Meta och <br>Banner och Display ad |
| `{{cta}}` | Call to action<br>Se [Anrop till åtgärd](#calls-to-action) | e-post <br>Meta och <br>Banner och Display och <br>LinkedIn |
| `{{image}}` | Bild - välj från [!DNL Content] | e-post <br>Meta och <br>Banner och Display och <br>LinkedIn |
| `{{on_image_text}}` | På bildtext <br>Se [Om bildtext](#on-image-text). | Meta och <br>LinkedIn |
| `{{link}}` | Call to action på bild<br>Se [Länk på bild](#link-on-image). | e-post |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing genererar automatiskt vissa fält i följande mallar:

- **E-postmallen** behöver inte identifiera fältet `subject`
- **Meta annonsmall** kräver inte att du identifierar fälten `headline`, `body` och `CTA`
- **Banner och Display ad template** kräver inte att du identifierar fältet `CTA`
- **LinkedIn och-mallen** kräver inte att du identifierar fälten `headline`, `introductory_text` och `CTA`

>[!WARNING]
>
>För Instagram-annonser visas den genererade rubriken inte i den slutliga versionen.

Det finns en gräns på 20 fält när en mall överförs till GenStudio for Performance Marketing. Eftersom fältet `subject` genereras automatiskt i ett e-postmeddelande räknas det som ett fält. Det innebär att 19 fält tillåts i en e-postmall.

>[!TIP]
>
>Du kan verifiera mallen med [mallförhandsgranskning](#template-preview) i GenStudio for Performance Marketing.

### Utmaningar

En Call to action (CTA) innehåller en fras och en länk. För att funktionerna _[!UICONTROL Rephrase]_&#x200B;och&#x200B;_[!UICONTROL Add link]_ ska fungera korrekt under genereringsprocessen för varianter måste du ta med platshållare för länken och frasen i mallen.

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

GenStudio for Performance Marketing kan även tillhandahålla olika uppmaningar att vidta åtgärder. Se [Granska Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Länka till bild

Du kan anpassa din e-postmall så att andra kan lägga till en länk till en bild. På samma sätt som för länken CTA använder du följande vägledning för att tillämpa en `link`-platshållare för en bildtagg:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

I detta exempel:

- `{{link}}` är en platshållare för den faktiska URL:en.
- `src="image-source.jpg"` ska ersättas med den faktiska URL-adressen för bildkällan.
- `{{imageDescription}}` är ett användardefinierat fältnamn som ger en platshållare för bildens alternativa text, vilket är användbart för hjälpmedel och SEO.

### Alternativ text

Använd ett användardefinierat fältnamn som platshållare för att generera en alternativ textbeskrivning (HTML `alt="text"`-attribut) för en bild. Följande `{{imageDescription}}`-platshållare används med fältet `{{image}}` i samma `<img>` -tagg, vilket säkerställer att relationen mellan bilden och beskrivningen kvarstår.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

I detta exempel:

- `{{image}}` är platshållare för bildkällans URL.
- `{{imageDescription}}` är platshållare för alt-texten, som innehåller en beskrivning av bilden för hjälpmedel och SEO.

### Hjälpmedelsetikett

Attributet `aria-label` används för att definiera ett tillgängligt namn för element som inte har synliga etiketter. Det här attributet är särskilt användbart i mallar där det är viktigt att ange kontext för interaktiva element, t.ex. en CTA-knapp.

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

### På bildtext

Platshållaren `{{on_image_text}}` används för att ange en textövertäckning med korta, effektfulla meddelanden som placeras direkt i bilden.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Manuella fältnamn

Alla andra fältnamn är användardefinierade och behandlas som manuellt ifyllda fält. Du kanske vill reservera ett avsnitt för sidfotsinnehåll.

Om du vill skapa ett redigerbart avsnitt lägger du till dubbla hakparenteser runt avsnittsnamnet:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

### Redigera avancerad text

Förbättra ditt kreativa innehåll under [!DNL Create]-processen med avancerad textredigering. Arbetsytan avgör möjligheten till formaterad text baserat på platsen för innehållsplatshållaren. RTF-funktioner är bara tillgängliga när du använder platshållare för innehåll som fristående element eller inom HTML-taggar på blocknivå, som `<p>`, `<div>` eller `<span>`.

RTF-redigering är tillgängligt för fristående innehåll i ett stycke:

```html
<p>{{body}}</p>
```

Om du använder en innehållsplatshållare inuti ett HTML-attribut (till exempel `alt`, `href` eller `src`) stöds inte RTF-redigering för det fältet.

RTF-redigering är **inte** tillgängligt för `alt`-innehåll:

```html
<img src="image.jpg" alt="{{image_description}}">
```

Om ett fält visas mer än en gång bestäms RTF-funktionen utifrån om det används som ett HTML-attribut i någon av förekomsterna. Om du t.ex. använder rubriken som rubrik och alternativ text för en bild har taggen `alt` företräde.

RTF-redigering är **inte** tillgängligt för `headline` eftersom den används som `alt`-innehåll:

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

RTF-redigering kan vara tillgängligt för vissa fält i specifika kanaler, som `on_image_text` i sociala kanaler (Meta, LinkedIn).

## Avsnitt eller grupper

Om din e-postmall kräver flera innehållsområden, t.ex. flera erbjudanden eller artiklar, kan du ordna dessa med hjälp av avsnitt eller grupper. _Avsnitt_ informerar GenStudio for Performance Marketing om att fälten i det här avsnittet kräver hög grad av konsekvens. Genom att etablera relationen kan AI generera innehåll som matchar de kreativa elementen i avsnittet.

Använd ett valfritt gruppnamn som prefix för att ange att ett fält är en del av ett avsnitt eller en grupp. Använd ett fältnamn (till exempel `headline`, `body`, `image` eller `cta`) efter understrecket (`_`).

Syntax: `groupname_fieldname`

- _Korrigera_ (👍): `pod1_body`
- _Felaktigt_ (❌): `pod1body`

Varje avsnitt kan bara använda en av varje fälttyp. Följande fält tillhör till exempel avsnittet `pod1`:

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

På grund av den här regeln kan avsnitten inte kapslas.

Varje malltyp, som e-post eller Meta-annons, har kanalspecifika begränsningar för användning av avsnitt. Se [kanalspecifika riktlinjer](/help/user-guide/templates/best-practices-for-templates.md) i avsnittet _Bästa metoder för att använda mallar_.

En e-postmall kan t.ex. innehålla upp till tre avsnitt. Därför kan du ha tre rubrikavsnitt och innehållsavsnitt:

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

GenStudio for Performance Marketing förstår att `pod1_headline` är närmare relaterat till `pod1_body` än till `pod2_body`.

>[!TIP]
>
>Se [Strukturerade uppmaningar](/help/user-guide/effective-prompts.md#structured-prompts) om hur du skapar en prompt som genererar varierande innehåll för varje avsnitt i ett e-postmeddelande med flera avsnitt.

## Förhandsgranska mall

När du [överför en mall](use-templates.md#upload-a-template) söker GenStudio for Performance Marketing igenom HTML-filen efter identifierade fält. Använd förhandsgranskningen för att granska dina [mallelement](use-templates.md#template-elements) och bekräfta att du har identifierat dem korrekt med de [igenkända fältnamnen](#recognized-field-names).

Exempel på Förhandsgranska för en e-postmall:

![Förhandsgranskningsfält har identifierats](/help/assets/template-detected-fields.png "Kontrollera identifierade fält"){zoomable="yes"}

Se [Mallkodredigerare](/help/user-guide/templates/code-editor.md).

### Förhandsgranska kontroll

Du kan styra visningen av specialinnehåll med hjälp av inbyggda hjälpredor (specialuttryck i mallspråket [!DNL Handlebars] som utför vissa åtgärder). Du kan till exempel lägga till en villkorssats som lägger till spårningsparametrar till länkar i den exporterade mallen samtidigt som förhandsgranskningslänkarna hålls rena.

Värdet `_genStudio.canvas` anges när en mall återges och värdet `genStudio.export` anges när en mall exporteras. Du kan välja att ta med visst innehåll högst upp i ett e-postmeddelande med en villkorlig omslutning, till exempel när mallen används för export:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Ett annat exempel kan vara att förhindra att spårningskoder används när en mall förhandsgranskas i GenStudio for Performance Marketing. I följande exempel visas hur du lägger till spårningsparametrar till länkar i den exporterade mallen, samtidigt som du håller förhandsgranskningslänkarna rena:

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Statiskt innehåll

E-post- och Meta-mallar länkar ofta till bilder och CSS-filer på andra domäner. När GenStudio for Performance Marketing genererar miniatyrbilder för mallförhandsvisningar eller de upplevelser som härletts från dem, valideras innehållskällan och en kopia bäddas in för förhandsgranskning.

Externa filer bäddas bara in tillfälligt i syfte att skapa mallförhandsvisningen, vilket gör att förhandsvisningen korrekt återger innehållet så som det ser ut när du skapar mallen. Dessa externa filer lagras **inte** permanent i GenStudio for Performance Marketing. När mallförhandsgranskningen har skapats fortsätter GenStudio for Performance Marketing att referera till den ursprungliga källlänken som finns i mallen.

### Uppdatera innehåll

Om källan ändras efter att den inledande förhandsgranskningen har skapats använder du funktionen [Uppdatera](/help/user-guide/templates/use-templates.md#refresh-template) för att uppdatera mallförhandsvisningen med den senaste versionen av innehållet från de externa källorna.
