---
title: Photoshop Plugin för Adobe GenStudio for Performance Marketing
description: Lär dig hur du installerar, konfigurerar och använder Photoshop-plugin för GenStudio for Performance Marketing.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Photoshop-plugin för GenStudio for Performance Marketing

GenStudio for Performance Marketing Photoshop plugin-programmet lägger till en panel i Adobe Photoshop som gör att du kan generera varumärkesanpassat innehåll.

På den här sidan beskrivs hur du installerar och konfigurerar plugin-programmet och hur du använder det.

Funktioner för det här plugin-programmet:

* Logga in på en GenStudio for Performance Marketing-instans med en Adobe ID
* Mappa GenStudio for Performance Marketing innehållsgenereringsfält till textlager i ett Photoshop-dokument
* Ange ett varumärke, en produkt, en persona och en textfråga för att generera innehåll
* Du kan också lägga till en bild som ska ersätta mallbilden
* Förhandsgranska genererade varianter av varumärkesinnehåll
* Använd genererat innehåll på mappade lager i det aktuella dokumentet
* Skapa innehållsöversättningar på webben
* Exporten har genererats [!DNL Experiences] till GenStudio for Performance Marketing

>[!VIDEO](https://video.tv.adobe.com/v/3478808?learn=on)

## Installera plugin-programmet

Följ dessa anvisningar för att installera plugin-programmet.

### Förutsättningar

* Creative Cloud desktop application
* Photoshop, minimum version 25.6.0

### Installationssteg

1. Hämta och uppdatera plugin-programmet från Creative Cloud Marketplace i Adobe Exchange.
1. Sök efter **GenStudio-plugin för Photoshop** i Adobe Exchange.
1. Installera plugin-programmet genom att följa anvisningarna.

### Avinstallera plugin-programmet

1. Starta Creative Cloud desktop-programmet.
1. Klicka på alternativet **[!UICONTROL Plugins]**.
1. Klicka på ellipsen **[!UICONTROL (...)]** på GenStudio för Creative Cloud-kortet om du vill se alternativ.
1. Välj **Avinstallera**.

## Skapa en mall

För att kunna generera innehåll måste du ha en GenStudio for Performance Marketing-mall som skapats från ditt Photoshop-dokument.

Så här skapar du en GenStudio-färdig mall:

1. Öppna ett dokument i Photoshop.
1. Identifiera ett textlager för genererat innehåll.
1. Byt namn på lagret med fältnamnets standardformat: `{<name_of_generated_field>}`. Exempel: `{body}`, `{headline}`, `{cta}`.
1. Byt namn på lager för alla [fält som krävs för den kanal som är avsedd för malltypen ](../../user-guide/templates/customize-template.md#recognized-field-names).

| Kanal | Obligatoriska fält för generering | Valfria fält för generering |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| Visa | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

Observera att flera lager kan ha samma fältbeteckning, men varje lager kan bara ange ett fält. Om det till exempel finns flera ritytor i dokumentet:

* Du kan ange ett `{headline}`-lager på varje rityta.
* Du kan ange flera `{headline}` lager på en enda rityta.
* Du kan inte ange att ett enskilt lager tar emot både fältnamnen `{headline}` och `{cta}`.

### Krav för mallstorlek

#### Meta-mallar

För Instagram- och Facebook-inlägg:

* Bredd: 1 080 pixlar (fast)
* Höjd: 1 080 px eller 1 350 px

För Instagram- och Facebook-artiklar:

* Bredd: 1 080 pixlar (fast)
* Höjd: 1 920 px

Plugin-programmet bestämmer färgen på den genererade upplevelsen baserat på mallens höjd.

#### Visningsmallar

Det finns inget krav på fast storlek. Visningsmallar har stöd för alla storlekar.

#### LinkedIn-mallar

* Bredd: 1 200 pixlar (fast)
* Höjd: 1 200 px, 628 px, 2 292 px, 1 800 px eller 1 500 px

Dokumentet är nu klart att användas med plugin-programmet.

## Generera nytt innehåll

1. Öppna Photoshop.
1. Öppna ett GenStudio-färdigt malldokument som du har skapat (se instruktionerna ovan) eller använd startmallen för GenStudio for Performance Marketing: `branding-template-acrobat-handlebars.psd`.
1. Öppna plugin-programpanelen på **[!UICONTROL Plugins]** > **[!UICONTROL GenStudio]**.
1. Klicka på knappen **[!UICONTROL Login]**. Om du tillfrågas om behörighet att öppna en URL-adress kan du kontrollera **Kom ihåg mitt val** och sedan klicka på **[!UICONTROL Allow]**.
1. Använd webbläsaren för att logga in med en profil som har åtkomst till GenStudio for Performance Marketing.
1. Markera den kanal (Meta, LinkedIn eller Display) som gäller för mallen som du har öppnat.
   ![Kanalval](./ps-select-channel.png){width="300" zoomable="yes"}
1. Välj kontexten [!DNL Brand], [!DNL Persona] och [!DNL Product] för innehållsgenereringen.
   ![Varumärke, persona och välj produkt](./ps-select-box.png){width="300" zoomable="yes"}
1. Välj antalet variationer som ska produceras.
1. Använd knappen under **[!UICONTROL Select Content]** för att bläddra bland och välja bilder från dina resurser. De 40 senast tillagda resurserna visas först, och du kan söka efter andra resurser. De valda bilderna storleksändras automatiskt så att de passar dina mallar.
1. Ange en textfråga för innehållet i rutan **[!UICONTROL Text Prompt]**.
1. Klicka på knappen **[!UICONTROL Generate]**. Variationer visas på kort på panelen Plugin-program.

Nya dokument läggs till på din Photoshop-arbetsyta med genererat innehåll tillämpat på mallfälten. Dessa dokument namnges med ett numrerat variantsuffix.

## Översätta innehåll

Användare kan översätta innehåll till språk som stöds efter kopieringsgenerering.

1. Klicka på **[!UICONTROL Translate]** när du har genererat en annonskopia med plugin-programmet.
1. Välj ett eller flera språk för översättningen.
1. Klicka på knappen **[!UICONTROL Translate]**.

Nya dokument läggs till på din Photoshop-arbetsyta med genererat innehåll tillämpat på mallfälten. Dessa dokument namnges med ett numrerat variantsuffix.

## Exportera upplevelser till GenStudio

Användarna kan välja export efter att innehållet har genererats eller översatts. Exporterade upplevelser fyller i innehållsavsnittet i GenStudio for Performance Marketing.

![Exporterade resurser som visas i innehållsavsnittet](./content-assets.png){width="90%"}

## Felsökning

Tänk på följande om du inte ersätter text eller bilder i genererade varianter.

### Mappade fält

Om text eller bilder inte ersätts bekräftar du att fält mappas korrekt med klammerparenteser `{}` (inte parenteser `()`).

### Bekräfta att teckensnitt är tillgängliga

Ett teckensnitt i ett textfält måste vara tillgängligt på datorn för att ersättning ska kunna ske under genereringen. Kontrollera att alla teckensnitt som används i filen är tillgängliga på datorn, särskilt om filen har skapats på någon annans dator.

### Undantag för fältmappning

{{$include /help/_includes/field-mapping-exceptions.md}}
