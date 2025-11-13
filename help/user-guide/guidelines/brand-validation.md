---
title: Varumärkesvalidering i Adobe GenStudio for Performance Marketing
description: Läs om hur det inbyggda varumärkesvalideringssystemet fungerar i GenStudio for Performance Marketing.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 436e2d7c02cef91eee7f4180f049b71b42ec76d5
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Varumärkesvalidering

I GenStudio for Performance Marketing är varumärkesvalidering en viktig komponent som fungerar i samarbete med de generativa AI-funktionerna och -riktlinjerna -[[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) och [[!DNL Personas]](/help/user-guide/guidelines/personas.md). Det ser till att allt innehåll är anpassat till varumärkesidentiteten, ADA-standarder och vägledning för olika kanalplattformar.

GenStudio for Performance Marketing genomför varumärkesvalidering och andra innehållskontroller av olika aspekter, bland annat:

* [!DNL Brand]-riktlinjer har definierats eller är standard
* Riktlinjer för plattformen
* American with Disabilities Act (ADA)-standarder
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->


## Sammanfattning av innehållskontroll

En sammanfattning av varumärkesvalidering och annan information om innehållskontroll för varje objekt med genererat innehåll kan nås via sammanfattningsikonen _Innehållskontroll_ för varje variant på arbetsytan.

Sammanfattningen av _innehållskontrollen_ visar följande:

* Procentandel kompatibilitet med din [[!DNL Brand]](brands.md), beräknat som antalet [riktlinjer](overview.md) som godkänts i valideringen jämfört med antalet riktlinjer som testats
* `Pass` eller `Fail` resultat för plattformsriktlinjer, som Meta eller LinkedIn
* `Pass` eller `Fail` resultat för ADA-tillgänglighetsstandarder

![Sammanfattning av innehållskontroll](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Klicka på procentandelen för att se hur kompatibel varianten är. Poängen uppdateras automatiskt när du redigerar varianterna eller annat innehåll. Du kan klicka på _Visa och åtgärda problem_ för att säkerställa ytterligare kompatibilitet.

Se [Förbättra varumärkesjusteringen](#improve-brand-alignment).

## Panelen Innehållskontroll

Panelen _Innehållskontroll_ öppnas till höger om arbetsytan när du klickar på den i det högra åtgärdsfältet _eller_ från sammanfattningsikonen [_Innehållskontroll_](#content-check-summary) . Panelen innehåller detaljerad varumärkesvalidering, riktlinjer för plattformen och information om tillgänglighetsstandarder och visar på möjligheter till förbättringar.

![Panelen Innehållskontroll](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

På panelen _Innehållskontroll_ visas validering och [kompatibilitetsinformation](/help/user-guide/guidelines/overview.md#compliance) för bilder och variantavsnitt:

* Representation av sammanfattningsinformation för _innehållskontrollen_ för [!DNL Brand], plattformsriktlinjer och tillgänglighetsstandarder
* _Behöver granskas_ och visar antalet felaktiga riktlinjer och detaljerad information om varje riktlinje som behöver revideras
* _Godkänt_-avsnitt som visar antalet skickade riktlinjer och detaljerad information om varje stödlinje

Se [Förbättra varumärkesjusteringen](#improve-brand-alignment) om du vill veta mer om hur du kan förbättra poängen för panelen _Innehållskontroll_.

### Innehållstyp

På panelen _Innehållskontroll_ kan du växla vilka stödlinje- och tillgänglighetsstandarder som ska kontrolleras. Klicka på ikonen _Innehållstyp_ (nivåikon) längst upp på panelen för att aktivera eller inaktivera:

* **[!DNL Brand]** - Utför de kontroller som är kopplade till riktlinjerna för [!DNL Brand]
* **Riktlinjer för plattformen** - Utför de kontroller som är kopplade till den kanalspecifika plattformen, till exempel Meta
* **Tillgänglighet** - Utför de kontroller som är kopplade till ADA-tillgänglighetsstandarder

Om du vill **ange innehållstypen** för de kontroller du vill utföra klickar du för att inaktivera eller på de tillgängliga typerna och klickar på **Använd**.

## Förbättra varumärkesanpassningen

Om du vill maximera effekten av genererat innehåll och behålla en konsekvent varumärkesidentitet använder du [_innehållskontrollen_ sammanfattning](#content-check-summary) och [_innehållskontrollpanelen_](#content-check-panel). Du kan ändra specifika avsnitt manuellt för att anpassa dem till dina [[!DNL Brand] riktlinjer](brands.md), kontroller av plattformens riktlinjer och kontroller av tillgänglighetsstandarder.

**Så här förbättrar du varumärkesjusteringen för genererade varianter**:

1. Klicka på panelikonen _Innehållskontroll_ i det högra åtgärdsfältet för att visa validering och tillgänglighetsinformation.

   Du kan se en sammanfattning av kontrollerna _Behöver granskas_ och _Godkänd_ för att se vad som behöver förbättras.

   >[!NOTE]
   >
   > Riktlinjen _Varumärkesröst_ som beskrivs på panelen _Innehållskontroll_ gäller för hela varianten, inte för ett enskilt avsnitt. Hela innehållsvarianten markeras för föreslagna förbättringar.

1. Klicka för att korrigera riktlinjer som för närvarande inte är kompatibla.
1. Klicka för att expandera och inspektera varje kontroll som behöver granskas i tillgängliga avsnitt som _Headline_, _Color_ och _Brand voice_.

   Använd de argument som ges för varje kontroll för att hjälpa dig att ändra bilder och varianter.

1. När du har gjort nödvändiga ändringar klickar du på **[!UICONTROL Recheck score]** för att kontrollera och validera dina ändringar och se till att de är mer i linje med din varumärkesidentitet, riktlinjer för plattformen och tillgänglighetsstandarder.

   Processen för innehållskontroll körs igen. Om de ändrade objekten godkänns i valideringen visas en grön banderoll längst ned på arbetsytan som bekräftar att poängen uppdaterades. Om det inte skett någon förändring efter en ny kontroll bekräftar banderollen att det inte skett någon ändring av poängen. Procentandelen i sammanfattningsikonen för _innehållskontroll_ för den ändrade varianten visar också förloppet.

1. Fortsätt att granska avsnitt för att säkerställa att hela varianten klarar validerings- och tillgänglighetskontroller. Navigera genom varje variant med pilarna bredvid en enskild variant på arbetsytan.
