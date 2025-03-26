---
title: Arbeta med mallar
description: Upptäck hur du använder mallar effektivt för att effektivisera din kreativa process i Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 0%

---

# Arbeta med mallar

GenStudio for Performance Marketing gör det möjligt för innehållsskapare att snabbt producera enhetligt marknadsföringsinnehåll med hjälp av _mallar_. En mall minskar tiden och arbetet som krävs för att generera nytt innehåll avsevärt genom att tillhandahålla en startpunkt som inkluderar förkonfigurerade layouter och designelement.

GenStudio for Performance Marketing stöder inte direkt framtagning av mallar i programmet, men du kan enkelt utforma och förbereda mallar med vanliga designverktyg som Adobe InDesign, Illustrator eller Express. När designen är klar kan du anpassa den för användning i GenStudio for Performance Marketing. Börja använda mallar genom att följa de här stegen:

1. **Designa din mall**: Använd det designverktyg du föredrar för att skapa den visuella layouten för din [mall med element](#template-elements) som förrubrik, rubrik, brödtext, CTA, bilder och sidfot.

2. **Koda din mall**: Konvertera din design till HTML och infogad CSS för att säkerställa att den är ren och responsiv på olika enheter. Ta en titt på [hjälpmedelsriktlinjerna](accessibility-for-templates.md) som kan hjälpa dig att nå ut till din avsedda målgrupp.

3. **Förbered för GenStudio for Performance Marketing**: Anpassa din HTML-mall med hjälp av hanteringsfältens mallspråk. Infoga platshållare för att ange var GenStudio for Performance Marketing ska generera innehåll dynamiskt. Se hur du [anpassar en mall](customize-template.md) för GenStudio for Performance Marketing.

Med de här stegen kan du skapa professionella och effektiva mallar som är klara att användas i GenStudio for Performance Marketing, så att du snabbt och effektivt kan producera varumärkesinnehåll.

## Mallelement

En mall är en uppsättning instruktioner som definieras med HTML och infogad CSS som kan användas för att skapa e-postmeddelanden, social annonsering eller webbannonsupplevelser. Mallelement tillhandahåller strukturen för att skapa innehåll.

Nedan följer en lista över element som används i mallar och en del detaljer om deras egenskaper:

| **Element** | **Kanal** | **Beskrivning** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Förrubrik** | E-post | En andra ämnesrad i ett e-postmeddelande, vanligtvis mellan 40 och 50 tecken, som förbättrar ämnesraden. Den visas i inkorgen bredvid motivet innan e-postmeddelandet öppnas. |
| **Sidhuvud** | E-post | Den övre delen av e-postmeddelandet som mottagaren ser när han/hon öppnar e-postmeddelandet anger tonen och anger kontext för det inkluderade innehållet. |
| **Rubrik** | Meta-annons, banner and Display ads, LinkedIn | Det första innehåll som mottagaren ser bör vara intressant att fånga intresset. |
| **Introduktionstext** | LinkedIn | Det primära meddelandet förmedlar huvudmeddelandet, ungefär som brödtexten. Du kan använda upp till 150 tecken, inklusive blanksteg, maximalt fyra känslolägesikoner och skiljetecken. |
| **Brödtext** | E-post, Meta-annons, Banner and Display ads | Huvudtexten i annonsen förmedlar huvudbudskapet. Det bör vara engagerande, informativt och övertygande att uppmuntra målgruppen att vidta de åtgärder som krävs. |
| **CTA** | E-post, Meta-annons, Banner and Display-annonser, LinkedIn | En knapp för att ringa till åtgärd använder en fras och en länk för att uppmuntra mottagaren att vidta en viss åtgärd, till exempel klicka på en länk eller göra ett köp. |
| **Bilder** | E-post, Meta-annons, Banner and Display-annonser, LinkedIn | Förbättra visuell tilltalande, dela upp text och ge stöd åt budskapet. Bilderna ska vara högklassiga och effektfulla. |
| **Sidfot** | E-post | Avsnittet längst ned i e-postmeddelandet innehåller ytterligare innehåll som kontaktinformation, länkar till sociala medier, ansvarsfriskrivningar och alternativ för att avbryta prenumerationen. |
| **Textövertäckning** | Meta ad | Text som placeras på en bild för att stödja och förbättra innehållet i rubriken och brödtexten. |

>[!TIP]
>
>Se de [identifierade fältnamnen](customize-template.md#recognized-field-names) som GenStudio for Performance Marketing stöder för mallar av varje kanaltyp.

## Anpassa mall

Du [anpassar mallen](customize-template.md) för användning i GenStudio for Performance Marketing genom att infoga platshållare för innehåll, eller fält, som den generativa AI-filen använder för att infoga innehåll. GenStudio for Performance Marketing känner igen vissa fält, till exempel fältet `body`, och följer kanalriktlinjerna som konfigurerats för det valda varumärket.

>[!TIP]
>
>Följ [hjälpmedelsriktlinjerna](accessibility-for-templates.md) och [bästa praxis](/help/user-guide/content/best-practices-for-templates.md) så att du kan nå ut till fler av din publik och skapa en optimal upplevelse.

## Hantera mallar

Galleriet _[!DNL Templates]_visar din lista med mallar som är anpassade för att generera upplevelser i GenStudio for Performance Marketing. Du kan filtrera mallar efter kanaltyp, till exempel e-post, visningsannonser, Meta-annonser och LinkedIn-annonser.

![Listan Innehållsmall](/help/assets/content-templates-filter.png "Sök i LinkedIn-mallar"){width="650" zoomable="yes"}

### Lägga till en mall

Innan du överför en mall måste du se till att den är helt förberedd och klar att användas i GenStudio for Performance Marketing genom att följa vägledningen för [Anpassa mallar](customize-template.md) .

**Så här lägger du till en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på **[!UICONTROL Add template]**.

1. I rutan _[!UICONTROL Add your approved template]_bläddrar du efter HTML-mallfilen eller drar HTML-mallfilen till släppområdet. Klicka på&#x200B;**[!UICONTROL Next]**.

1. Granska fälten i rutan _[!UICONTROL Check detected fields]_. Kontrollera att du använder rätt mall och att all information är som förväntat.

   Exempel på Förhandsgranska för en e-postmall:

   ![Förhandsgranskningsfält har identifierats](/help/assets/template-detected-fields.png){width="650" zoomable="yes"}

   >[!TIP]
   >
   >Om mallen inte är korrekt klickar du på **[!UICONTROL Back]** och går tillbaka till föregående steg. Överför den korrigerade mallfilen. Eller använd [mallkodsredigeraren](/help/user-guide/content/code-editor.md) för att göra enkla korrigeringar.

1. Klicka på **[!UICONTROL Next]** när du är nöjd med mallförhandsvisningen.

1. I rutan _[!UICONTROL Provide template details and upload]_ger du mallen ett namn och väljer en **[!UICONTROL Channel]**-typ.

   Mallnamn och kanaltyp krävs. Ytterligare krav kan vara:

   - **Meta**: kräver proportioner
   - **Banner och Display ad**: kräver Dimensions

1. Lägg till så många detaljer du kan för att förbättra identifiering av mallar i sökningar och filtrering.

1. Klicka på **[!UICONTROL Done]**.

### Uppdatera mall

Mallar kan innehålla statiska filer, till exempel ikoner eller logotyper. [Statiskt innehåll](/help/user-guide/content/customize-template.md#static-content) lagras inte när mallförhandsvisningen har skapats. GenStudio for Performance Marketing fortsätter att referera till källlänken som finns i mallen. Använd Uppdatera för att uppdatera mallförhandsvisningen med de senaste versionerna av dessa resurser.

**Så här uppdaterar du mallen**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på en mall för en fullständig vy och en lista med detaljer.

1. Klicka på **[!UICONTROL Refresh]** (cirklingspilar) i det övre högra hörnet för att uppdatera alla resurser som används i mallen.

### Skapa en upplevelse med en mall

Hitta och använd en befintlig mall i GenStudio for Performance Marketing för att skapa fler upplevelser.

**Så här skapar du en upplevelse med en mall**:

1. I _[!DNL Content]_väljer du avsnittet **[!UICONTROL Templates]**.

1. Klicka på en mall för en fullständig vy och en lista med detaljer.

1. Klicka på **[!UICONTROL Create Experience]** (penselverktyget) i det övre högra hörnet om du vill använda mallen.

1. Fortsätt till [Skapa](/help/user-guide/create/overview.md#create-use-cases) en upplevelse.

## Mallar från AJO och Marketo

Du kan överföra en mall som du har skapat i Adobe Journey Optimizer (AJO) eller Marketo. GenStudio for Performance Marketing identifierar programspecifika mönster och ignorerar dem, vilket bevarar originalformuläret för fortsatt användning i AJO eller Marketo. Du behöver inte göra några ändringar i den ursprungliga AJO- eller Marketo-syntaxen.

Kända programmönster är:

- **AJO**: `{{profile.*}}`, `{{context.*}}`
- **Marketo**: `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Förutsättningar**

- Programmet (AJO, Marketo) och GenStudio for Performance Marketing måste tillhöra samma IMS-organisation för integrering
- Användarna måste ha rollen&quot;Medarbetare&quot; (den lägsta nivån) eller högre

>[!ENDSHADEBOX]

Därefter [anpassar du mallen](/help/user-guide/content/customize-template.md) med platshållare för att ange var GenStudio for Performance Marketing ska generera innehåll åt dig. [Lägg till mallen ](#add-a-template) i databasen [!DNL Content] och validera mallen. Gör eventuella mindre korrigeringar med kodredigeraren.
