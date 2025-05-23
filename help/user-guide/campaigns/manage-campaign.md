---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Läs om hur du hanterar kampanjer och kampanjinnehåll
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Den här funktionen finns för närvarande i Beta, så vissa funktioner kan vara begränsade eller kunna ändras."
source-git-commit: 689a3f9c1860237d82774850f5b07145c6d3f562
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Hantera kampanjer

Standardvyn för kontrollpanelen [!DNL Campaigns] visar kampanjer efter **[!UICONTROL Start Date]**, med början från den senaste. Raderna innehåller huvudattributen för varje kampanj. Du kan växla mellan standardlistvyn, kortvyn och tidslinjevyn för alla kampanjer. Klicka på ikonen som motsvarar den vy du vill använda längst upp till höger i tabellen.

* **Listvy** - Den här standardvyn visar en delmängd av den definieringsinformation som anges när kampanjer skapas. Listvyn innehåller beskrivning, kanaler, regioner, start- och slutdatum samt status.
* **Kortvy** - Den här gallerivyn representerar varje kampanj med ett kort.
* **Tidslinjevy** - Den här Gantt-liknande representationen visar varje kampanj som ett vågrätt fält som representerar dess varaktighet och förlopp. Staplarna ordnas kronologiskt från vänster till höger så att ni snabbt kan utvärdera kampanjens förlopp, hitta överlappande milstolpar och förstå hur kampanjer justeras över tiden.

Varje vy har följande funktioner:

* Sök efter en kampanj efter namn eller nyckelord
* Växla för att ändra vyer
* Skapa kampanj

## Kampanjinformation

Om du vill visa information om en viss kampanj klickar du på kampanjnamnet i listan eller kortvyn. Vyn _Kampanjinformation_ öppnas. Dessa kampanjdetaljer är de attribut som tilldelas när kampanjer skapas.

{{$include /help/_includes/campaign-details.md}}

**Så här visar du innehåll som är associerat med kampanjen**:

1. Klicka på **[!UICONTROL Content]** precis nedanför kampanjnamnet. En _filterkampanjinnehåll_-vy öppnas.

1. Växlingsknappar i området **[!UICONTROL Filter by]** för att identifiera kampanjinnehåll med _Assets_, _Experience_ och _Templates_.
I den här vyn visas länkade resurser, upplevelser och mallar. Dubbelklicka på en tillgångs kort för att se information.

## Uppdatera kampanjinnehåll

När en kampanj har startats kan [!DNL Insights] hjälpa dig att spåra komponenternas prestanda. Ni kan utvärdera hur effektiva olika resurser och upplevelser är. Med den här prestandainformationen kan du fatta välgrundade beslut om vilka komponenter som ska ersättas, markeras eller revideras.

### Lägga till och ta bort kampanjinnehåll

Du kan hantera resurser i en kampanj genom att lägga till eller ta bort kampanjetiketten från resursen eller upplevelsen.

1. Välj en upplevelse eller resurs i galleriet [!DNL Content] _Erfarenheter_ eller _Assets_.

1. Lägg till eller ta bort kampanjetiketten från vyn _Detaljer_ .

Mer information om hur du skapar resurser och upplevelser som ska ingå i kampanjen finns i [!DNL Create].

## Uppdatera kampanjattribut

Efterhand som kampanjer pågår kan målgrupper och tidsplaner behöva justeras. Du kan lägga till eller ta bort distributionskanaler, profiler, regioner och produkter från en aktiv kampanj.

## Lägga till eller ta bort en kanal

Kampanjens vy _Detaljer_ innehåller de kanaler, målprofiler, regioner och produkter som är länkade till den här kampanjen.

1. Klicka på **[!UICONTROL Connect records]** till höger om etiketten _Kanaler_, _Områden_, _Personas_ eller _Produkter_.

   Popup-fönstret _Anslut poster_ öppnas.

1. Välj den inställning som du vill lägga till eller ta bort.

   Klicka på **[!UICONTROL Select all]** om du vill se fler alternativ. Popup-fönstret _Anslut objekt_ öppnas.

## Ta bort en kampanj

Om du tar bort en kampanj tas den bort från kampanjobjektet och alla definierade kampanjattribut från [!DNL Content]. Det tar bort kampanjetiketten från alla resurser och upplevelser utan att ta bort själva upplevelsen eller resursen.

**Så här tar du bort en kampanj**:

1. I _Kampanjer_ klickar du på åtgärdsmenyn (...) bredvid namnet på kampanjen som du vill ta bort.

1. Välj **[!UICONTROL Delete]**.

   Du kan också ta bort en kampanj från åtgärdsmenyn (..) bredvid kampanjnamnet i vyn _Detaljer_ .
