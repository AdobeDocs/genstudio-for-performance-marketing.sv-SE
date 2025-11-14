---
title: Versionsinformation för Adobe GenStudio for Performance Marketing
description: Läs om de senaste funktionerna och förbättringarna i Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: f6dc843acc6d29b107f5165dfd2ee1d2c9e72f0f
workflow-type: tm+mt
source-wordcount: '4144'
ht-degree: 0%

---

# Versionsinformation för GenStudio for Performance Marketing

Den här versionsinformationen innehåller de senaste uppdateringarna av GenStudio for Performance Marketing-programmet.

## 2025.11.14 {#latest}

### Integrering av Real-Time CDP

* GenStudio for Performance Marketing är nu integrerat med Adobe Real-Time Customer Data Platform (RTCDP) vilket gör att marknadsförarna kan utnyttja målgruppsdefinitioner direkt i arbetsflödet [!DNL Create].
* Genom att välja [!DNL Audience]-parametrar under innehållsgenereringen kan marknadsförarna skapa personaliserade kreativa kopior och e-postkopior utifrån kundens sammanhang, inklusive meddelandeinställningar, köpsegment, kundfaser och beteendedata.

### Innovid Insights for display advertising

* [!DNL Insights] inkluderar nu Innovid (tidigare Flashtalk) som en webbannonskanal, vilket gör att marknadsförarna kan analysera kampanjresultaten tillsammans med Meta, LinkedIn och TikTok på en enhetlig plattform.
* Med daglig datauppdatering och tillgång till viktiga prestandamått, inklusive visningar, klickningar och CTR, kan marknadsförarna fatta snabbare optimeringsbeslut utan att behöva växla mellan verktygen.

### Färdig översättning för betalmedia och e-post

* Översätt snabbt godkända betalda medier och e-postupplevelser till över 40 språk direkt i GenStudio for Performance Marketing.
* Med Azure Open AI Translation Services kan team översätta innehåll till flera målspråk samtidigt.

### PDF export för upplevelser

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

* Marknadsförarna kan nu [exportera upplevelser till PDF-format](/help/user-guide/content/manage-assets.md#export-experiences) för granskning, godkännande och arkivering.

### Egna modeller i Firefly Image Model 4

* GenStudio for Performance Marketing har nu stöd för [anpassade modeller som har utbildats i Adobe Firefly Image Model 4](/help/user-guide/create/generate-assets.md), vilket ger bättre funktioner för generering av bilder på ett varumärke med förbättrad fotorealism och detaljrikedom.

### Aktivera enstaka videoannonser i Meta

* Marknadsförarna kan nu [aktivera Meta-annonser med enstaka videomaterial](/help/user-guide/activation/activate-meta-ad.md) direkt från GenStudio for Performance Marketing till Meta Ads Manager. Detta gör det möjligt för medieköpare, presterande marknadsförare och kreativa team att smidigt publicera videoreklamupplevelser, med samma smidiga arbetsflöde som används för statisk annonsaktivering.
* Användarna kan konfigurera videoannonsinformation, förhandsgranska hur videon kommer att se ut och aktivera videoannonser för Meta-plattformar.

### CPA efter åtgärdstyp för Meta-kampanjer

* Analysera [kostnad per åtgärd (CPA) med flexibel konverteringsspårning](/help/user-guide/insights/ads.md) för Meta-annonskampanjer.
* I stället för ett enda fast mätvärde kan du välja mellan flera åtgärdstyper - t.ex. inköp, tilläggshändelser, leads, videovisningar eller anpassade konverteringar - för att beräkna och visa CPA för kampanjer, annonser, resurser och attribut i [!DNL Insights].

### Korrigeringar och förbättringar

* Ett SDK-tillägg har lagts till som gör det möjligt för kunder att ansluta till sina egna DAM:er i stället för att använda AEM Assets som standard för mediefiler när innehåll genereras.
* Användare kan nu använda [!DNL Brand]-taggar för att gruppera [!DNL Product]- och [!DNL Persona]-poster efter [!DNL Brand].
* Flödet [!DNL Experience Translations] har optimerats tillsammans med den nya översättningsfunktionen för Betald media och E-post.


## Versionsinformation

+++Anmärkningar från 2025.10.16

### Nya GenStudio-pluginer för Photoshop och Figma

* Skapa varumärkesanpassade och personaliserade annonser direkt med de nya designverktygen GenStudio Plugins för Adobe Photoshop och Figma.

### Utökade videofunktioner

* Nu kan marknadsförarna enkelt lägga in- och utgångsklipp i videoreklam med förproducerad reklam.
* Lägg till bild-, text- och logoövertäckningar i hela videon

### Utökade insikter för LinkedIn, Meta och TikTok

* GenStudio Insights innehåller nu LinkedIn Ads prestandarapporter som gör det möjligt för marknadsförare att se och analysera hur kampanjer och annonser fungerar direkt på plattformen för:
   * LinkedIn-annonser
   * Meta Ads
   * TikTok Ads

### Aktivera Amazon Ads

* GenStudio stöder nu aktivering av webbannonser direkt i Amazon Ads Platform.

### FlashTalande aktivering

* GenStudio har nu stöd för aktivering av webbannonser direkt i FlashTalk (Innovid) Ad Serving Platform.
* Användarna måste manuellt konfigurera sin Flashtalk API-token i samordning med Activate Engineering-teamet. Självbetjäningstokenkonfigurationen läggs till i en framtida version.

### Integrering med Adobe Campaign V8

* GenStudio for Performance Marketing är nu integrerat med Adobe Campaign V8, vilket gör att marknadsförarna smidigt kan utnyttja det AI-baserade innehållet tillsammans med Campaigns avancerade orkestreringsfunktioner.

### Autospela video

* Videor spelas nu upp automatiskt över [!DNL Create]-, [!DNL Content]- och [!DNL Insights]-moduler, vilket ger smidiga förgranskningsupplevelser.

### Import av e-postmallar från tredje part

* GenStudio for Performance Marketing har nu stöd för smidig integrering med e-postsystem från tredje part via ett utbyggbart ramverk. Viktiga funktioner:

   * Importera mallar automatiskt från tredjepartssystem för e-postdesign när du skapar innehåll
   * Lägg in mallmetadata tillsammans med importerade mallar
   * Bibehåll en enda källa till sanning genom att ansluta direkt till tredjepartssystem
   * SDK och exempelappar för anpassade integreringar

+++



+++Anmärkningar från 2025.09.11

### Ny generativ utökad AI-funktionalitet för betalmedia

Med den nya funktionen GenExpand kan marknadsförarna dynamiskt anpassa sina kreativa resurser till olika proportioner i betalda mediekanaler som Meta, LinkedIn, Display Ads och Banners. När en bild inte matchar de avsedda proportionerna, till exempel att lägga till en smal bild i en bred layout, kan du använda GenExpandera för att anpassa bilden.

Den här funktionen effektiviserar bildredigeringen och ändrar storlek direkt i GenStudio for Performance Marketing. Mer information finns i [Generative Expandera AI-funktioner](/help/user-guide/create/manage-variants.md#use-generative-expand).

+++

+++Anmärkningar från 2025.08.15

### Insikter om textattribut

Insikter om textattribut i Adobe GenStudio analyserar den känslomässiga tonen, övertalningstekniken och den berättarröst som används i annonstexten. När en kampanj är klar håller GenStudio reda på hur dessa textattribut korrelerar med nyckeltal som CTR, CPA, CPC, intryck och utgifter.

Detta är för närvarande endast tillgängligt för annonser på engelska. Mer information finns i [Textfunktioner](/help/user-guide/insights/text-features.md).

### Förbättringar av Insights-mallar

* Kortet för förhandsgranskning av annonser innehåller nu alternativet &quot;Se mer&quot; för text.
* Nya mallar för annonser i masterkort.

### Generera flerspråkigt innehåll med varumärkesvalidering

Den nya språkväljaren i snabbredigeraren har stöd för att skapa flerspråkigt innehåll, vilket gör att regionala marknadsförare kan utveckla varumärkesinnehåll för sina lokala målgrupper. Den här funktionen har för närvarande stöd för 12 språk.

### Stöd för videomaterial i mallar

* Videor kan läggas till i Meta- och LinkedIn-mallar.

### Aktivera förbättringar av upplevelsen

* Ny funktionalitet för att spara utkast av aktiveringar.
* Ny funktion för att försöka utföra misslyckade aktiveringar igen.

### Använd samma roll i flera textfält

Flera textfält med samma roll stöds nu (till exempel body, cta, on image text osv.) för komplexa kundmallar.

Utforska informationen i [vägledningen för mallkodsredigeraren](/help/user-guide/content/code-editor.md).

### Nya Firefly bildgenereringsmodeller stöds

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Adobe GenStudio for Performance Marketing har nu stöd för den senaste Firefly Image Model 4-sviten, inklusive två kraftfulla varianter:

**Firefly-bild 4**: Optimerad för snabbhet och enkelhet, idealisk för att skapa illustrationer, ikoner, enkla objektfoton och porträtt med ett motiv - som täcker 90 % av de kreativa behoven varje dag.

**Firefly Image 4 Ultra**: Prioriterar fotorealism och precision, och är mycket bra på att återge mänskliga porträtt, medelstora grupper och komplexa scener för avancerade kreativa arbetsuppgifter.

Mer information om hur du använder de här nya bildgenereringsmodellerna finns i [Generera resurser](/help/user-guide/create/generate-assets.md).

### Färdig översättning för e-post

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Adobe GenStudio for Performance Marketing har nu inbyggda funktioner för e-postöversättning som gör att marknadsförarna effektivt kan skala sina e-postkampanjer globalt. Med den här funktionen kan du ta en godkänd e-postupplevelse och översätta den till flera målspråk med Azure Open AI-översättningstjänster.

+++

+++Anmärkningar från 2025.07.25

### Kompatibelt resursfilter

Ett nytt filter i modulen [!DNL Insights] döljer automatiskt [bild- och videomaterial som inte stöds &#x200B;](/help/user-guide/insights/ads.md#ad-formats) från förhandsvisningar av annonser, vilket eliminerar den visuella störningen och brutna rutor. Den här förbättringen säkerställer att användarna endast ser medier som är tillgängliga och färdiga att använda, vilket ger en renare och mer tillförlitlig upplevelse. Filtret fungerar tillsammans med det befintliga filtret Kompatibilitetsannonser.

### Aktivering av flera tillgångar för metadata

Med funktionen för bildaktivering med flera proportioner för Meta Ads kan annonsörer överföra och aktivera flera bildresurser med olika proportioner under en enda annons. Med den här funktionen kan en annons ge rätt kreativ anpassning till olika Meta-montage som Feed, Stories och Reels. Annonsörer kan förhandsvisa hur varje bild återges på olika placeringar och publicera alla versioner på Meta i ett enda API-anrop.

### RTF-formatering i varianter

[Redigera textfält i genererade varianter med formaterad text](/help/user-guide/create/manage-variants.md#manually-edit-text) alternativ som fet, kursiv, understrykning, textjustering, listor, textfärg, textstorlek och länkar. På så sätt kan du förfina text och fraser för publiken och använda formatering för att uppfylla layoutkraven.

### Hjälpmedelsetiketter för bilder och länkar

Lägg till hjälpmedelsetiketter (Aria-labels) till bilder och call-to-action länkar i dina varianter för att ge användarna hjälpmedelsanpassade namn som hjälper dem förstå syftet med interaktiva element. Mer information finns i [Hantera varianter](/help/user-guide/create/manage-variants.md).

### Generering av icke-engelskt innehåll

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Den nya listrutan Språkväljare i snabbredigeringsfacket har stöd för att skapa flerspråkigt innehåll, vilket gör att regionala marknadsförare kan utveckla varumärkesanpassat innehåll för sina lokala målgrupper. Den här funktionen har för närvarande stöd för 12 GA-språk och 5 Beta-språk, med språklistan som ger ett definierat arbetsflöde och ett tydligt språkdirektiv för LLM för enhetligare resultat.

### Mallval är valfritt för Meta ads

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Val av mallar är nu valfritt med Meta-annonser, vilket gör att användare kan skapa annonser utan att behöva text och logotyp överst i mediet. Den här förbättringen möjliggör andra medietyper som animerade GIF-bilder och videor som kanske inte kräver textöverlägg eller logotypplacering.

+++

+++Anmärkningar från 2025.06.15

### Startmallar är tillgängliga

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

[Med startmallar](/help/user-guide/templates/starter-templates.md) kommer du snabbt igång med den kreativa processen. Du kan nu välja från en Meta- eller LinkedIn-startmall.

### Funktioner för generativ utökning av AI

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

I GenStudio for Performance Marketing [!DNL Create] kan du nu använda [&#x200B; Generative Expandera AI-funktioner](/help/user-guide/create/manage-variants.md#use-generative-expand) för att utöka bilddimensionerna och lägga till generativt innehåll för att passa annonsmallarna i betalda medievarianter.

### Lägg till videoklipp i annonser

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Förutom bildinnehåll kan du nu lägga till videofilmer i [LinkedIn](/help/user-guide/create/create-linkedin.md#manage-videos)- och [Meta](/help/user-guide/create/create-meta-ad.md#manage-videos)-annonser. Se hur du kan spela upp videofilmer automatiskt direkt i GenStudio for Performance Marketing när du väljer och lägga till videofilmer till dina varianter.

### Korrigeringar och förbättringar

* Stöd för [publicering av annonsupplevelser](/help/user-guide/activation/activate-linkedin-ad.md) från GenStudio for Performance Marketing har lagts till i LinkedIn Campaign Manager. [!DNL Activate] har stöd för detaljerade förhandsvisningar av LinkedIn-annonser innan de publiceras till LinkedIn Campaign Manager.

* Integreringen av [Workfront Proof](/help/user-guide/approvals/overview.md) ger GenStudio for Performance Marketing tillgång till Korrekturens robusta gransknings- och godkännandefunktioner. Innehåll som granskas i GenStudio for Performance Marketing synkroniseras med Workfront Proof och kommentarer och status bevaras.

* Lagt till möjlighet att [ge tillgängliga namn för bilder och call-to-action-länkar](/help/user-guide/create/manage-variants.md#add-accessibility-labels) i dina varianter genom att lägga till hjälpmedelsetiketter (Aria-labels).

* När du lägger till eller ändrar [Varumärkesriktlinjer](/help/user-guide/guidelines/brands.md) på ett icke-engelskt språk, visar GenStudio for Performance Marketing riktlinjerna på samma språk.

* När du har lagt till en [!DNL Brand] manuellt eller skapat en [!DNL Brand] genom manuell extrahering från ett dokument kan du [ändra eller lägga till miniatyrbilder för varumärket](/help/user-guide/guidelines/add-guidelines.md#change-brand-thumbnail) för att vara säker på att varje varumärke är lätt att urskilja i [!DNL Brands]-listan.

* Du kan nu [använda RTF-redigeringsformatering för text](/help/user-guide/create/manage-variants.md#manually-edit-text) i dina genererade varianter. Experimentera med en mängd formateringsalternativ för olika typer av text, som färg, storlek, listor med mera.

* Du kan nu [skapa en ny annonsuppsättning](/help/user-guide/activation/activate-meta-ad.md#create-a-new-ad-set) under plattformskonfiguration genom att klona en befintlig annonsuppsättning under plattformskonfigurationen. Metaannonser definierar timing, kanalinformation och publik för en viss annons. En Meta-kampanj kan innehålla flera annonsuppsättningar, men en annonsuppsättning är exklusivt kopplad till en kampanj.

* Nu kan du exportera kampanjinformation så att den blir externt åtkomlig som kampanjrapporter i Word eller PDF. Välj en kampanj och klicka sedan på **[!UICONTROL Export]** (övre högra hörnet).

+++

+++Anmärkningar från 2025.05.15

### Korrigeringar och förbättringar

* Aktiverade funktioner för [att lägga till alternativ (alt) text](/help/user-guide/create/manage-variants.md#add-alt-text-for-images) i en bild för en enskild variant.
* Lagt till [nya Meta-proportioner](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) - liggande 1,19:1 (1 080 pixlar bredd).
* Nu kan du välja mer än en upplevelse för export eller hämtning. Se [Exportera upplevelser](/help/user-guide/content/manage-assets.md#export-experiences).
<!-- * Added support for [publishing ad experiences](/help/user-guide/activation/activate-meta-ad.md) directly from _[!DNL Content]_ [into Google Campaign Manager 360 and Meta Ads Manager](/help/user-guide/activation/activate-cm360-ad.md). -->

+++

+++Anmärkningar från 2025.04.15

### Korrigeringar och förbättringar

* Nya filteralternativ för mallar! Nu kan du förfina din _[!UICONTROL Select templates]_-lista i [!DNL Create] och i&#x200B;_[!UICONTROL Content]_ > _[!UICONTROL Templates]_. Se [Sökmallar](/help/user-guide/content/use-templates.md#search-templates). Se till att mallarna är rätt taggade med metadata så att de kan identifieras med dessa filter.
* Aktiverade funktioner för att [visa och markera enskilda lager](/help/user-guide/create/manage-variants.md#view-layers) - redigerbara textfält eller redigerbara bilder - av en upplevelse som framhäver dem för revideringar, som att återskapa innehåll eller beskära bilder.
* Ett [nytt mallfält](/help/user-guide/content/use-templates.md#template-elements), `sub-headline` har lagts till för ytterligare text i upplevelser för att få publiken att lyssna och lyfta fram marknadsföringsmeddelanden.
* Stöd för [publiceringsupplevelser](/help/user-guide/activation/overview.md) från GenStudio for Performance Marketing har lagts till i Google Campaign Manager 360. Aktivera har stöd för detaljerade förhandsvisningar av Google Campaign Manager 360-annonser innan du publicerar till en Campaign Manager 360-annonsörer. Annonser som publiceras via Activate hämtas automatiskt in i insikterna när de väl är publicerade, vilket gör det möjligt för användarna att spåra och rapportera annonsresultaten.

+++

+++Anmärkningar från 2025.03.13

### Aktivera Meta-annonser

Nu kan marknadsförare [publicera annonsupplevelser](/help/user-guide/activation/overview.md) från GenStudio for Performance Marketing i Meta Ads Manager. [!DNL Activate] har stöd för detaljerade förhandsvisningar av Meta-annonser före distributionen. Meta-annonser som publicerats via [!DNL Activate] hämtas automatiskt till [!DNL Insights] en gång i realtid, vilket gör att användare kan spåra och rapportera annonsprestanda.

### Skapa LinkedIn-upplevelser

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Stöd har lagts till för [att skapa LinkedIn-upplevelser](/help/user-guide/create/create-linkedin.md). Se fliken [LinkedIn och](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) i kanalspecifika riktlinjer.

### Skapa banderollupplevelser

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Stöd har lagts till för [att skapa banderollupplevelser](/help/user-guide/create/create-banner-experience.md). Se fliken [Banner](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) i kanalspecifika riktlinjer.

### Regelefterlevnad

Som en del av varumärkesvalideringsprocessen har [efterlevnadsstandarder](/help/user-guide/guidelines/overview.md) introducerats i [innehållskontroller](/help/user-guide/guidelines/brand-validation.md). Dessa kontroller granskar varje variant i en upplevelse utifrån [!DNL Brand] riktlinjer, plattformsriktlinjer (t.ex. för Meta) och ADA-standarder. Denna process ger en omfattande sammanfattning av riktlinjer och standarder som behöver revideras för att bättre uppfylla kraven.

### Utbyggbarhet

Det nya GenStudio for Performance Marketing [utökningsramverket](/help/extensibility/setup.md) innehåller verktyg för organisationer som kan införliva egna efterlevnadsprotokoll i arbetsflödet för innehållsskapande och validering via tillägg eller utökningsbara program.

### Mallar

* **Mallkodredigerare** - Den nya [mallkodsredigeraren](/help/user-guide/content/code-editor.md) hjälper dig att verifiera och förfina mallen för optimal användning när du skapar nya upplevelser med GenStudio for Performance Marketing.

  ![Vyn Kodredigeraren](/help/assets/template-detected-fields.png "Kontrollera identifierade fält"){width="500" zoomable="yes"}

* **Länkar i bild** - Anpassa din e-postmall genom att aktivera bildlänkar. Se [Anpassa en mall: Länk på bild](/help/user-guide/content/customize-template.md#link-on-image).
* **AJO- och Marketo-mallar** - Överför en mall som du har skapat i Adobe Journey Optimizer (AJO) eller Marketo. Se [Arbeta med mallar från AJO och Marketo](/help/user-guide/content/use-templates.md#templates-from-ajo-and-marketo).

### Korrigeringar och förbättringar

* Aktiverade funktioner för [standardkanal](/help/user-guide/guidelines/brands.md#channel-guidelines), [bild](/help/user-guide/guidelines/brands.md#image-guidelines), [logotyp](/help/user-guide/guidelines/brands.md#logos) och [färg](/help/user-guide/guidelines/brands.md#colors) riktlinjer för [[!DNL Brands]](/help/user-guide/guidelines/brands.md).
* Lagt till möjlighet att [lägga till länkar till bilder](/help/user-guide/create/manage-variants.md#add-image-link) inom en variant.
* Funktionerna för [innehållskontroll](/help/user-guide/guidelines/brand-validation.md) och granskning och godkännande har flyttats till det nya högra åtgärdsfältet för att maximera utrymmet på arbetsytan och förbättra användarupplevelsen.
* Förenklade flödet för [överföring eller manuellt tillägg av ett varumärke](/help/user-guide/guidelines/add-guidelines.md#add-brands).
* Introducerade möjligheten att [lägga till eller byta bildresurser i en variant](/help/user-guide/create/manage-variants.md#swap-image) på arbetsytan.
* Förbättrad användarupplevelse och synlighet för kanalkategorierna [på hemsidan Skapa](/help/user-guide/create/overview.md) genom att separera dem till avsnitten Ägt media, Betalat media och Innehåll.
* Förbättrad filtrering i [!DNL Insights] tabell- och gallerivyer.

+++

+++Anmärkningar från 2025.02.13

### Förbättringar av landningssidan för [!DNL Create]

Startsidan [!DNL Create] i GenStudio for Performance Marketing innehåller förbättringar av användargränssnittet som förbättrar användarupplevelsen. Avsnittet _Senaste arbete_ har förfinats och konfigurerats med listvyn som standardvy. Utfyllnad och andra visuella förbättringar effektiviserar utseendet på arbetsytan i [!DNL Create].

### Insikter exporteras till CSV

Du kan nu hämta den visningsbara tabellen från valfri [!DNL Insights]-vy till en CSV-fil. Med den här funktionen kan du exportera och analysera data från olika [!DNL Insights]-vyer, vilket underlättar dataanalys och rapportalternativ.

+++

+++Anmärkningar från 2025.01.16

### Integrering med Adobe Workfront Proof

[!BADGE Beta]{type=Informative tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."}

Integreringsprogrammet GenStudio for Performance Marketing och Adobe Workfront Proof Beta lanseras den här månaden. Workfront Proof snabbar upp framtagning och aktivering av innehåll med mallar för godkännande, arbetsflöden i flera steg och anteckningar. GenStudio for Performance Marketing-användare med Workfront Proof-behörigheter kan använda Proof-funktionens avancerade funktioner i GenStudio for Performance Marketing för att granska och kommentera GenStudio-genererat material.

Med Beta kan man utforma produktutvecklingen och fastställa den allmänna tillgänglighetsberedskapen.

### Generera nya uppmaningar att agera

Nu kan du skapa nya call-to-action-fraser (CTA) när du hanterar varianter. Använd de nya alternativen _Återfras_ och _Lägg till länk_ för att generera nya fraser och redigera länken CTA. Mallen måste vara korrekt konfigurerad för att dessa nya CTA-funktioner ska fungera. Följ riktlinjerna i _Anpassa en mall_: [Anrop till åtgärd](/help/user-guide/content/customize-template.md#calls-to-action). Mer information om hur du hanterar CTA för varianter finns i [Ändra Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action). <!-- GS-6676 -->

### Korrigeringar och förbättringar

* Teckenantal visas nu i alla genererade och manuella fält för visningsannonser. Se _Antal tecken_ i [Meta-upplevelser](/help/user-guide/create/meta-experiences.md#character-counts). <!-- GS-7732 -->

* _Medarbetare_ kan nu visa resurser, men inte skapa, redigera eller ta bort dessa resurser. Medarbetarberättiganden har inte framtvingats på det sätt som förväntades i [!DNL Create]. <!-- GS-7614 -->

* Nu kan redaktörer redigera resurser, upplevelser och mallmetadata. <!-- GS-4905 -->

* Nu finns stöd för anpassade bildstorlekar i Meta annonsmallar. <!-- GS-7512 -->

* Personuppgifter, varumärken och produktval är nu förinlästa under mallgenereringen. <!-- GS-8069 -->

* E-postlänken för call-to-action är inte längre ett obligatoriskt fält. <!-- GS-8103 -->

* Listrutan [!DNL Brand] för väljare fungerar nu som förväntat för mallar. Tidigare gick det inte att läsa in väljaren för vissa mallar. <!-- GS-8908 -->

* Nu kan redaktörer välja högst fyra bilder för e-postmeddelanden med ett enda streck och Meta-annonser. <!-- GS-2631 -->

* Årsvärdet för en godkänd upplevelses `Created by`-fält förblir nu konsekvent som förväntat efter att upplevelsens metadata har redigerats. <!-- GS-8344 -->

* Innehållsredigerare kan nu välja en mall från [!DNL Create]. Tidigare uppstod ett konsolfel i programmet när en redigerare valde en mall.  <!-- GS-8798 -->

* Problem med storleksändring och omgenerering för Meta-annonser har lösts. <!-- GS-8900 -->

* Knappen **[!UICONTROL Back]** returnerar nu användare till antingen föregående sida eller [!DNL Create]-landningssidan som förväntat. <!-- GS-8622 -->

+++

+++Anmärkningar från 2024.12.12

### Nya funktioner

Redigerare kan nu utföra följande metadatarelaterade uppgifter:

* Redigera material, upplevelser och mallmetadata. Se [Resursinformation](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* Visa en tillgångs genererade taggar i vyn _Detaljer_ om du har en upplevelse som använder resursen. Se _Genererade taggar_ i [Resursinformation](/help/user-guide/content/asset-details.md#generated-tags). <!-- GS-3705 -->

Redigerare kan nu ange anpassade värden för följande aspekter av genererade varianter:

* Bredd och höjd för webbanners i mallar för visning och visning. Dessa värden sparas nu som mallmetadata. <!-- GS-6735 -->

* Dimensioner för bilder i displayannonsupplevelser under bildöverföring.<!-- GS-7166 -->

* Se kanalspecifika riktlinjer i [Bästa tillvägagångssätt för mallar](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

Exportalternativen omfattar nu:

* Exportera displayannonser och Meta-annonser som HTML, JPEG eller PNG. Se [Skapa en upplevelse av webbannonsering](/help/user-guide/create/create-display-ad.md) och [Skapa en metaannonsupplevelse](/help/user-guide/create/create-meta-ad.md). <!-- GS-7093 6655 5152-->

Med ytterligare nya funktioner kan redigerare:

* Använd knappen **[!UICONTROL Refresh]** i vyn [!DNL Content] Mallar _Resursinformation_ för att uppdatera den valda mallen. <!-- GS-7102 -->

* Generera om sektioner av displayannonser och e-postvarianter. Se [Skapa en webbannonsupplevelse](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) och [Skapa en e-postupplevelse](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Duplicera befintliga varumärken. Se [Hantera varumärken](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

### Korrigeringar och förbättringar

* Visningsannonsrubrikerna sparas nu på [!DNL Content] som förväntat. <!-- GS-7239 -->

* Knappfacket stängs inte längre när en redigerare klickar utanför den nedrullningsbara menyn. <!-- GS-7275 -->

* Listrutan [!DNL Create] [!DNL Persona]/[!DNL Product] läses nu in som förväntat när ett fel i en URL-tjänst för miniatyrbilder inträffar. <!-- GS-7277 -->

* Visa annonser som innehåller element som överläggsfragment kan nu redigeras. <!-- GS-7186 -->

* Knappen Canvas **[!UICONTROL Brand]** är nu inaktiverad när märkespoäng inte genereras för en upplevelse. <!-- GS-6429 -->

* Arbetsytan visar nu dimensionerade upplevelser i konsekvent ordning. <!-- GS-7123 -->

* Manuell beskärning använder nu bilddimensioner, inte malldimensioner, vid redigering av displayannonser. Tidigare användes malldimensioner, inte bilddimensioner, när en bild var mindre än de dimensioner som angavs i mallen för visning och visning. <!-- GS-7315 -->

* Redigerare kan nu välja upp till fyra bilder när de skapar en visningsannons. <!-- GS-7189 -->

* Webbannonser och Meta-annonsutkast läses nu in som förväntat när storleken ändras i en annan webbläsare. <!-- GS-7204 -->

* Oanvända mallfält visas inte längre i genererat innehåll.  <!-- GS-5670 -->

* Redigerare kan nu klicka på länkar för att redigera som förväntat i genererade varianter. <!-- GS-7423 -->

* [!DNL Create] respekterar nu medarbetarens behörigheter korrekt. <!-- GS-7614 -->

* Knappen Arbetsyta **[!UICONTROL Resize]** är nu inaktiverad när alla storleksalternativ har markerats och renderats. <!-- GS-5940 -->

* Granskare som bara har åtkomst till vyn kan nu zooma in och ut på varianter under granskningar. <!-- GS-7371 -->

* Tangentbordsfokus har bara lagts till för åtgärdbara knappar i vyn [!DNL Create] _Senaste arbete_ . <!-- GS-4060 -->

* Meddelandet **Pågående** som visas under åtgärder för att spara e-postfragment visas nu bara under sparåtgärden. Tidigare visades det här meddelandet i Canvas. <!-- GS-6964 -->

* Redigerare ser nu ett felmeddelande som förväntat när ett utkast inte kan läsas in i området [!DNL Create] _Senaste arbete_.  <!-- GS-8081 -->

* På arbetsytan visas nu storleksändrade Meta-annonser och annonser i rätt ordning.  <!-- GS-7375 -->

* Redigerare kan nu klicka i fält på e-post och visa annonser. <!-- GS-6297 -->

* Funktionen för att redigera fragment för e-post och Meta-annonser aktiveras nu som väntat med ett enda klick. <!-- GS-8081 -->

* Förbättrade prestanda för knappen [!DNL Create] **[!UICONTROL Back]**. <!-- GS-6767 -->

+++

+++Anmärkningar från 2024.11.14

### Nya funktioner

Stöd för att visa statiskt innehåll på externa domäner har lagts till. GenStudio for Performance Marketing validerar innehållskällan som definierats i mallen och bäddar in en kopia för att skapa mallförhandsvisningen. Se [Statiskt innehåll](/help/user-guide/content/customize-template.md#static-content). <!-- GS-6107 -->

### Korrigeringar och förbättringar

* När storleken ändras i en annan webbläsare än den som användes för att generera det ursprungliga innehållet läses utkasten in som förväntat. <!-- GS-7204 -->

* Alla tecken representeras nu korrekt i den exporterade HTML. <!-- GS-7246 -->

* Knapparna på popup-menyn [!DNL Content] _Erfarenheter_ **[!UICONTROL Export]** trunkeras inte längre på vissa språk. <!-- GS-6873 -->

* Visningsannonser som skapats med mallar med storleken 50x50 exporteras nu med den förväntade bildstorleken. Tidigare exporterades PNG-filer med dubbla de förväntade dimensionerna. <!-- GS-7192 -->

* Mallfel som uppstod när visningsannonser storleksändrades har nu åtgärdats. <!-- GS-7322 -->

### Lokalisering

Den här versionen innehåller förbättringar av lokaliseringen i hela användargränssnittet, bland annat:

* Alla strängar i popup-fönstret [!DNL Content] _Överför resurs_ är nu korrekt lokaliserade. <!-- GS-6872 6770 -->
* Alla verktygstips i [!DNL Content] _Assets_-vyfältet **[!UICONTROL Search]** är lokaliserade. <!-- GS-6879 -->
* När du ersätter en befintlig bild i en e-postvariant på arbetsytan [!DNL Create] är vyn _Välj från innehåll_ nu lokaliserad. <!-- GS-6906 -->

+++

+++Anmärkningar från 2024.11.07

### Korrigeringar och förbättringar

* Rotationsrutan _Spara i arbete_ visas inte längre när en användare klickar på **[!UICONTROL Upload New Image]** och sedan avbryter åtgärden innan överföringen har slutförts. <!-- GS-6780 -->

* Upplevelsetitlar skapas nu korrekt vid upplevelsegenerering. <!-- GS-7006 -->

* Problem med flimmer rullningslister vid inläsning av utkast har lösts. <!-- GS-5587 -->

* Länken `View documentation` i popup-fönstret [!DNL Content] _Lägg till den godkända mallen_ fungerar nu som förväntat. <!-- GS-6881 -->

* Om du tar bort en bild från promptlådan under en storleksändring uppstår inte längre något fel. <!-- GS-7115 7009 -->

* Markering av **[!UICONTROL Delete]** från åtgärdsmenyn [!DNL Create] (..) fungerar nu som förväntat. <!-- GS-6871 -->

* Användarna kan nu styra alla interaktiva element i Meta och mallar enbart med tangentbordet. <!-- GS-4066 -->

* Extrahering av bilddimensioner från mallbildfält har lagts till i Visa annonsmallar. Begäran om smart beskärning skickas nu för den faktiska dimensionen av bilden och inte för hela mallen. <!-- GS-6926 -->

* Strängen `Zoom to fit to screen` har lokaliserats i genererade e-post- och Meta-annonser. <!-- GS-5063 -->

* Frågekassen [!DNL Create] stängs nu som förväntat när en användare klickar bort. <!-- GS-5254 -->

* Export av metadataannonser innehåller nu den valda call-to-action-etiketten som förväntat. <!-- GS-6504 -->

* Varumärkespoängen uppdateras nu och behålls som förväntat för återskapade upplevelser. <!-- GS-6535 -->

* HTML export av Meta-annonser och visningsannonser innehåller inte längre wrapper `div`- och `chrome`-element. <!-- GS-7116 -->

* Problem med återgivning av utkast via e-post vid publicering har nu lösts. <!-- GS-6394 -->

* Knappen Canvas **[!UICONTROL Brand]** är nu inaktiverad när ingen varumärkespoäng genereras. <!-- GS-6429 -->

* Växlingen Facebook/Instagram i åtgärdsfältet Arbetsyta uppdaterar nu upplevelserenderingar som förväntat när inställningen för arbetsytan `ReadOnly` är aktiverad. <!-- GS-7039 -->

#### Omgenerering av bilder

* Att ändra storlek på flera Meta-annonsvarianter fungerar nu som väntat. Tidigare visades inte regenererade varianter på arbetsytan, men de förblev tomma. <!-- GS-7010 -->

* Fragmentomgenerering fungerar nu som förväntat för upplevelser med ändrad storlek. <!-- GS-6836 -->

* Återskapande av Meta-annonsbilder efter storleksändring resulterar inte längre i ett fel. Tidigare ändrades kanalens metadata från `meta` till `facebook` när bilder ändrades före omgenerering. <!-- GS-7042 -->

+++

+++Anmärkningar från 2024.10.31

### Nya funktioner

* Sökfiltret **[!DNL Content]** har nu stöd för sökning efter färgtagg. <!-- GS-5501 -->

* Arbetsytan **[!DNL Create]** visar nu teckenantal för e-postfragment. <!-- GS-5819 -->

### Korrigeringar och förbättringar

* Etiketter för skärmläsare som saknas har lagts till i `view`-element för mobiler och datorer. <!-- GS-5624 4729 -->

* Ämnesraden och textområdena före sidhuvudet på **[!DNL Create]**-arbetsytan är nu dynamiska i höjdled. <!-- GS-6258 -->

* Layoutproblem med e-postkanter har lösts. <!-- GS-6631 -->

* Tangentbordsfokus fungerar nu som väntat på knappen **[!DNL Content]** **[!UICONTROL Delete]**. Tidigare kunde användare inte komma åt den här knappen via tangentbordet.  <!-- GS-4065 -->

+++

+++Anmärkningar från 2024.10.14 Allmän tillgänglighet

I den här versionen presenteras Adobe GenStudio for Performance Marketing, en generativ AI-baserad applikation som snabbar upp planering, utveckling och analys av marknadsföringskampanjer. GenStudio for Performance Marketing ger marknadsföringsteamen möjlighet att skapa varumärkesanpassat flerkanalsinnehåll för annonser, e-post och kampanjer samtidigt som ni får realtidsinsikter för att optimera innehållets prestanda.

### Funktioner

Några viktiga funktioner:

I **[!DNL Create]** introduceras arbetsytan, som erbjuder en strukturerad frågeupplevelse som gör det möjligt för innehållsredigerare att snabbt generera innehåll och varianter. Systemansvariga utbildar produkten enligt riktlinjer för varumärken. [!DNL Create] säkerställer att allt AI-genererat innehåll följer varumärkesriktlinjerna - branding, kundprofiler och produktbeskrivningar - och effektiviserar produktionen av slagkraftigt, varumärkesenhetligt marknadsföringsmaterial.

**[!DNL Content]** lagrar förvaltade, varumärkeskompatibla, godkända resurser och upplevelser. GenStudio for Performance Marketing-användare kan enkelt hitta, redigera, återanvända och dela godkända mediefiler, vilket minskar behovet av att återskapa innehåll från grunden för varje kampanj.

**[!DNL Reviews and Approvals]** skapar ett ramverk för intressenter som kan granska och godkänna genererade varianter innan de sparar till **[!DNL Content]** eller exporterar.

**[!DNL Campaigns]** organiserar och hanterar marknadsföringskampanjer och säkerställer smidig körning och spårning. Medarbetarna kan visualisera, planera och spåra kampanjer för att hantera flera initiativ effektivt och säkerställa att de levereras i rätt tid.

**[!DNL Insights]** erbjuder realtidsutvärdering av innehållsprestanda, vilket hjälper marknadsförarna att optimera sina strategier och fatta datadrivna beslut.

GenStudio for Performance Marketing kan integreras med andra Adobe Experience Cloud-produkter som Adobe Express och Adobe AEM Assets.

+++
