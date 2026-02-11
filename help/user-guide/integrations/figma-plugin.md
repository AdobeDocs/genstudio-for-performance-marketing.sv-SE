---
title: Figma Plugin för Adobe GenStudio for Performance Marketing
description: Lär dig hur du konfigurerar och använder Figma-plugin-programmet för GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: c6080555812fa82a7b71eee7e2deb963a881d9f4
workflow-type: tm+mt
source-wordcount: '2001'
ht-degree: 0%

---

# Figma plugin för GenStudio for Performance Marketing

GenStudio for Performance Marketing Figma-pluginen lägger till en ny panel i Figma-programmet som gör att du kan generera varumärkesanpassat innehåll.

På den här sidan beskrivs hur du konfigurerar och använder plugin-programmet.

Funktioner för det här plugin-programmet:

* Mappa Figma-textelement till GenStudio for Performance Marketing-fält, t.ex. `headline`, `body`, `on_image_text`.
* Generera en ny varumärkesanpassad Meta-, LinkedIn- eller Display-annons [!DNL Experiences] baserat på varumärke, persona, produkt och textruta.
* Skapa [!DNL Experiences] direkt i Figma-dokumentet genom att ersätta texten i mappade Figma-element med värden som genererats av GenStudio for Performance Marketing.
* Gör om, förkorta, förlänga eller översätta befintligt innehåll baserat på en uppmaning.
* Översätt genererad [!DNL Experiences] till flera språk.
* Exportera genererade [!DNL Experiences] till en lokal källa som förenklade bilder.
* Exporten genererade [!DNL Experiences] till GenStudio for Performance Marketing.
* Använd plugin-alternativ som anpassar sig till de valda elementen på arbetsytan i Figma.

>[!VIDEO](https://video.tv.adobe.com/v/3478813?captions=swe&learn=on)

## Skapa en mall

Plugin-programmet kräver att de två första nivåerna i Figma-dokumentet följer den här konventionen:

* **Avsnitt** - Detta representerar det överordnade projektet, som kan innehålla flera mallar.
* **Ram** - Detta representerar en mall i ett projekt. Mallen kan fyllas med text, bilder, komponenter och andra element.

### Meta-mallar

Dessa mallstorlekar stöds:

För Instagram- och Facebook-inlägg:

* Bredd: 1 080 pixlar (fast)
* Höjd: 1 080 px eller 1 350 px

För Instagram- och Facebook-artiklar:

* Bredd: 1 080 pixlar (fast)
* Höjd: 1 920 px

Plugin-programmet bestämmer färgen på den genererade upplevelsen baserat på mallens höjd.

### Visningsmallar

Det finns inget krav på fast storlek. Visningsmallar har stöd för alla storlekar.

### LinkedIn-mallar

* Bredd: 1 200 pixlar (fast)
* Höjd: 1 200 px, 628 px, 2 292 px, 1 800 px eller 1 500 px

### Fältrollsmappning

Plugin-programmet måste förstå mallens olika element, t.ex. rubrik, brödtext eller bild.

Så här tilldelar du elementroller:

1. Markera ett element i mallen (text, bild osv.).
1. Använd listrutan för att tilldela en roll.

Plugin-programmet kommer ihåg dessa mappningar som används för genererat innehåll. En fältroll kan mappas till flera mallelement.

![Fältrollsmappning](./field-role-mapping.png){width="600"}

### Undantag för fältmappning

{{$include /help/_includes/field-mapping-exceptions.md}}

## Generera nytt innehåll

Använd GenStudio for Performance Marketing AI för att generera eller göra variationer av element i Figma-mallar.

1. Om du använder GenStudio Plugin Playground eller redan förberedda mallar väljer du den avsnittsnod som innehåller dina annonsmallar. Du kan göra detta på panelen **Lager** eller genom att klicka direkt på avsnittet på arbetsytan.
   ![Avsnittsmarkering eller variationer](./plugin-playground.png){width="500" zoomable="yes"}
1. I plugin-fönstret anger du ett projektnamn för variationerna, väljer en plattform för innehållet och fyller i övrig nödvändig information. Klicka sedan på knappen **[!UICONTROL Finish Setup]**.
   ![Konfigurera projektfönster](./setup-project.png){width="300" zoomable="yes"}
1. Välj [!DNL Brand], [!DNL Persona] och [!DNL Product] som ska användas för innehållsgenerering.
1. Välj antalet variationer som ska produceras (upp till åtta).
1. Använd knappen under **[!UICONTROL Select Content]** för att bläddra bland och välja bilder från dina resurser. De 40 senast tillagda resurserna visas först, och du kan söka efter andra resurser. De valda bilderna storleksändras automatiskt så att de passar dina mallar.
1. Skriv en textfråga. Varje fält i listan **[!UICONTROL Fields]** har alternativet **[!UICONTROL Action]** inställt på **[!UICONTROL Generate]** för nytt innehåll.
1. Mappa alla fältroller. Se [Fältrollsmappning](#field-role-mapping).
1. Klicka på knappen **[!UICONTROL Generate]**.

## Översätt eller generera reklamvarianter från befintligt innehåll

Använd GenStudio for Performance Marketing AI för att generera reklamvarianter eller översätta Figma-mallar.

1. Markera den avsnittsnod som innehåller annonsmallarna. Du kan göra detta på panelen **Lager** eller genom att klicka direkt på avsnittet på arbetsytan.
   ![Avsnittsmarkering eller variationer](./plugin-playground.png){width="500" zoomable="yes"}
1. I plugin-fönstret anger du ett projektnamn för variationerna och väljer en plattform för innehållet.
1. I **[!UICONTROL What is the goal?]** väljer du **[!UICONTROL Generate Variations]** eller **[!UICONTROL Translate]** och klickar sedan på knappen **[!UICONTROL Finish Setup]**.
   ![Konfigurera projektfönster](./setup-project.png){width="300" zoomable="yes"}
1. Välj [!DNL Brand], [!DNL Persona] och [!DNL Product] som ska användas för innehållsgenerering.
1. Välj antalet variationer som ska produceras.
1. Använd knappen under **[!UICONTROL Select Content]** för att bläddra bland och välja bilder från dina resurser. De 40 senast tillagda resurserna visas först, och du kan söka efter andra resurser. De valda bilderna storleksändras automatiskt så att de passar dina mallar.
1. Skriv en textfråga. Varje fält i listan **[!UICONTROL Fields]** har alternativet **[!UICONTROL Action]** inställt på **[!UICONTROL Generate]** för nytt innehåll.
1. Mappa alla fältroller. Se [Fältrollsmappning](#field-role-mapping).
1. Markera varje fälttyp om du vill generera variationer eller översätta i panelen till vänster om plugin-programmet och klistra in det ursprungliga innehållet i varje **[!UICONTROL Initial Content]**-ruta.
   ![Exempeltext i rutan Ursprungligt innehåll](./initial-content-box.png){width="60%" zoomable="yes"}
1. Klicka på knappen **[!UICONTROL Generate]**.

## Översätt innehåll efter generering

1. Välj en generation som du vill översätta.
   ![Välj generering](./select-generation.png){width="200" zoomable="yes"}
1. Välj **[!UICONTROL Translation]** och klicka sedan på **[!UICONTROL Translate]**.
1. Välj målspråk.
1. Klicka på **[!UICONTROL Select]**.

Översättningsresultaten är:

* En ny sida visas med översatt innehåll.
* Varje översättning visar målspråket eller språkområdet.
* Originalinnehållet ändras inte på originalsidan.

![Översättningsresultat](./translation-results.png){width="60%" zoomable="yes"}

## Andra åtgärder för innehållsfält efter generering

När du redigerar befintligt innehåll i ett fält visas användbara alternativ på plugin-panelen.

![Alternativ för insticksåtgärder](./figma-other-actions.png){width="300" zoomable="yes"}

Alternativen är:

* Ändra **[!UICONTROL Value]** så att texten ändras direkt. Om du ändrar det här innehållet gäller det automatiskt alla valda varianter.
* AI kan utföra många **[!UICONTROL Action]** alternativ, bland annat:

| Åtgärd | Beskrivning |
| --- | --- |
| **[!UICONTROL Generate]** | Generera en ny textvariant. |
| **[!UICONTROL Rephrase]** | Generera en ny textvariant. |
| **[!UICONTROL Shorten]** | Generera en kortare variant av texten. |
| **[!UICONTROL Lengthen]** | Generera en längre textvariant. |

När du har valt ett **[!UICONTROL Action]**-alternativ kan du återskapa innehåll med knappen **[!UICONTROL Regenerate]**.

## Generera en bild

Generera bilder som du kan använda i mallar med hjälp av en textruta.

1. Välj **[!UICONTROL Generate Image]**.
1. Välj en modell i listrutan. Du kan också välja egna modeller som du har skapat.
1. Välj inställningsikonen för att justera genereringsinställningarna.
1. Valfritt: Välj en proportion.
1. Valfritt: Justera bildens stil genom att göra något av följande:
   * Överför en referensbild från din enhet eller AEM genom att välja **[!UICONTROL Upload image]**.
   * Välj en av Adobe Stock-bilder genom att välja **[!UICONTROL Browse Gallery]**.
   * Välj ett styrkevärde med reglaget. Styrka justerar hur strikt Firefly följer det format du anger.
1. Markera knappen **&lt;**.
1. Skriv en uppmaning.
1. Välj ikonen Generera. Bilder visas på panelen Plugin-program.
1. Lägg in bilder på arbetsytan på något av följande sätt:
   * Dra och släpp en bild på arbetsytan.
   * Markera en bildruta på bildarbetsytan och markera en bild i plugin-fönstret som du vill infoga i bildrutan.
   * Välj ikonen för att överföra en bild till arbetsytan.
   * Välj 3 punkter och **[!UICONTROL Download all to Figma]**.
1. Valfritt: Välj de tre punkterna för att utföra ytterligare åtgärder:
   * Välj **[!UICONTROL Generate more]** om du vill köra uppmaningen igen.
   * Välj **[!UICONTROL Copy prompt]** om du vill kopiera uppmaningen.
1. Valfritt: Välj pennikonen om du vill använda Generativ fyllning och Generera liknande åtgärder på en enda bild.

## Generera liknande bilder

Skapa en uppsättning liknande bilder.

1. Välj **[!UICONTROL Generate Similar]**-kortet.
1. Välj en bild som referens på något av följande sätt:
   * Markera en bild på bildarbetsytan.
   * Välj **[!UICONTROL Upload image]** att överföra från din enhet.
   * Välj **[!UICONTROL Browse AEM assets]** att överföra från AEM.
1. Välj ikonen Generera. Variationer visas på plugin-programpanelen.
1. Lägg in bilder på arbetsytan på något av följande sätt:
   * Dra och släpp en bild på arbetsytan.
   * Markera en bildruta på bildarbetsytan och markera en bild i plugin-fönstret som du vill infoga i bildrutan.
   * Välj ikonen för att överföra en bild till arbetsytan.
   * Välj 3 punkter och **[!UICONTROL Download all to Figma]**.
1. Valfritt: Välj de tre punkterna för att utföra ytterligare åtgärder:
   * Välj **[!UICONTROL Generate more]** om du vill köra uppmaningen igen.
1. Valfritt: Välj pennikonen om du vill använda Generativ fyllning och Generera liknande åtgärder på en enda bild.

## Ta bort bakgrund

Ta bort bakgrunden i en bild.

1. Välj **[!UICONTROL Remove Background]**-kortet.
1. Välj en bild som referens på något av följande sätt:
   * Markera en bild på bildarbetsytan.
   * Välj **[!UICONTROL Upload image]** att överföra från din enhet.
   * Välj **[!UICONTROL Browse AEM assets]** att överföra från AEM.
1. Välj **[!UICONTROL Remove]**. Om bilden har valts från arbetsytan ersätts bilden på bildarbetsytan. Om bilden har valts från en enhet eller AEM kan du dra och släppa den på arbetsytan eller välja **[!UICONTROL Insert Image]** för att placera bilden på arbetsytan.

## Generativ fyllning

Använd generativa fyllningar för ett område i en bild.

1. Välj **[!UICONTROL Generative Fill]**-kortet.
1. Välj en bild som referens på något av följande sätt:
   * Markera en bild på bildarbetsytan.
   * Välj **[!UICONTROL Upload image]** att överföra från din enhet.
   * Välj **[!UICONTROL Browse AEM assets]** att överföra från AEM.
1. Välj penselverktyget och skapa en mask.
1. Valfritt: Välj cirkumflex och justera penselstorleken.
1. Markera återställningsknappen för att ta bort masken.
1. Du kan också markera ikonen Ta bort bakgrund för att ta bort bakgrunden.
1. Ange en uppmaning om att vägleda genereringen av den markerade masken och välj knappen **[!UICONTROL Generate]**.
1. Lägg in bilder på arbetsytan på något av följande sätt:
   * Dra och släpp en bild på arbetsytan.
   * Markera en bildruta på bildarbetsytan och markera en bild i plugin-fönstret som du vill infoga i bildrutan.
   * Välj ikonen för att överföra en bild till arbetsytan.
   * Välj 3 punkter och **[!UICONTROL Download all to Figma]**.
1. Valfritt: Välj de tre punkterna för att utföra ytterligare åtgärder:
   * Välj **[!UICONTROL Copy prompt]** om du vill kopiera uppmaningen.
1. Valfritt: Välj pennikonen om du vill använda Generativ fyllning och Generera liknande åtgärder på en enda bild.

## Uppmana att redigera

Redigera innehållet i en bild med en textruta.

1. Välj **[!UICONTROL Prompt to Edit]**-kortet.
1. Välj en bild som referens på något av följande sätt:
   * Markera en bild på bildarbetsytan.
   * Välj **[!UICONTROL Upload image]** att överföra från din enhet.
   * Välj **[!UICONTROL Browse AEM assets]** att överföra från AEM.
1. Välj inställningsikonen för att justera genereringsinställningarna.
1. Valfritt: Välj en proportion och välj knappen **&lt;**.
1. Ange en uppmaning som guidar genereringen och välj knappen **[!UICONTROL Generate]**.
1. Lägg in bilder på arbetsytan på något av följande sätt:
   * Dra och släpp en bild på arbetsytan.
   * Markera en bildruta på bildarbetsytan och markera en bild i plugin-fönstret som du vill infoga i bildrutan.
   * Välj ikonen för att överföra en bild till arbetsytan.
   * Välj 3 punkter och **[!UICONTROL Download all to Figma]**.
1. Valfritt: Välj de tre punkterna för att utföra ytterligare åtgärder:
   * Välj **[!UICONTROL Generate more]** om du vill köra uppmaningen igen.
   * Välj **[!UICONTROL Copy prompt]** om du vill kopiera uppmaningen.
1. Valfritt: Välj pennikonen om du vill använda Generativ fyllning och Generera liknande åtgärder på en enda bild.

## Generativ utökning

Utvidga bilderna och lägg till generativt innehåll med Generative Expandera. Generativ utökning gör att du kan omvandla fyllningsbilder till de lämpligaste proportionerna för banners, Meta-annonser, LinkedIn-annonser eller mallar för visningsannonser.

1. Välj **[!UICONTROL Generative Expand]**-kortet.
1. Markera en bild på arbetsytan.
1. Ändra storlek på bildrutan Utöka temporärt ritstift till önskade nya mått.
1. Valfritt: Flytta bilden var som helst inuti ramen.
1. Ange en uppmaning som guidar genereringen och välj knappen **[!UICONTROL Generate]**.
1. Välj en bild på arbetsytan som du vill ersätta den ursprungliga bilden med det genererade resultatet.

## Exportera upplevelser

Variationer kan exporteras från Figma som GenStudio for Performance Marketing [!DNL Experiences].

1. Välj det innehåll som ska exporteras på arbetsytan i Figma genom att göra något av följande:
   * Markera genereringsavsnittet på arbetsytan och klicka sedan på **[!UICONTROL Mark all for Export]** på plugin-panelen.
     ![Val av genereringsavsnitt](./select-generation-section.png){width="200" zoomable="yes"}
   * Välj en enskild generation på arbetsytan och klicka sedan på **[!UICONTROL Mark for Export]** på plugin-panelen.
     ![Individuellt genererat urval](./select-generation.png){width="200" zoomable="yes"}
1. Välj Exportera objekt på sidofältsmenyn.
   ![Knappen Markera för export visas för en Meta-annons](./mark-for-export.png){width="60%" zoomable="yes"}
1. Välj ett mål.
1. Klicka på **[!UICONTROL Export]** om du vill exportera innehållet.

En ZIP-fil skapas på plugin-panelen eller så visas en länk till **[!UICONTROL Open in GenStudio]**. Använd ZIP-länken för att välja var filen ska sparas, eller välj **[!UICONTROL Open in GenStudio]**.

## Genereringshistorik

Plugin-programmet har en ändringshistorik för varje fält. På mallsidan väljer du **[!UICONTROL Generation history]** i sidofältet för plugin-programmet.

![Alternativet Genereringshistorik visas för en Meta-annons](./generation-history.png){width="80%" zoomable="yes"}

## Felsökning

Tänk på följande om du inte ersätter text eller bilder i genererade varianter.

### Mappade fält

Om text eller bilder inte ersätts kontrollerar du att fält har mappats till GenStudio fältroller i plugin-programmets användargränssnitt. Se [Fältrollsmappning](#field-role-mapping).

### Bekräfta att teckensnitt är tillgängliga

Ett teckensnitt i ett textfält måste vara tillgängligt på datorn för att ersättning ska kunna ske under genereringen. Kontrollera att alla teckensnitt som används i filen är tillgängliga på datorn, särskilt om filen har skapats på någon annans dator.

### Överväg stöd för fältroll

Vissa kanaler har bara stöd för ersättning i vissa fält. Observera undantag för [fältrollsmappning](#field-role-mapping).
