---
title: Figma Plugin för Adobe GenStudio for Performance Marketing
description: Lär dig hur du konfigurerar och använder Figma-plugin-programmet för GenStudio for Performance Marketing.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '1129'
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
