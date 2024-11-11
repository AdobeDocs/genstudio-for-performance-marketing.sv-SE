---
title: Tilldela [!DNL Brand] behörigheter
description: Lär dig hur du tilldelar berättiganden för skapare och redigerare av GenStudio for Performance Marketing [!DNL Brand] .
level: Intermediate
feature: Brands Service, Generative AI
source-git-commit: 3c391753ebd0d19ad7dcb17870915eeccc55cc05
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# Tilldela [!DNL Brand] behörigheter

Som standard kan GenStudio systemhanterare skapa och redigera [!DNL Brands]. Rollerna som innehållsredigerare och medarbetare har behörighet att redigera och skapa, men behöver inte ha några systemhanteringsrättigheter. Om du vill ge innehållsredigerare och medarbetare dessa [!DNL Brand]-relaterade berättiganden måste en Adobe-systemadministratör utföra ytterligare konfigurationsuppgifter i Adobe Admin Console. Se [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) i _Administrationshandboken för Enterprise och Teams_.

Att lägga till användare och användargrupper är grundläggande uppgifter som är gemensamma för alla Adobe-produkter med berättiganden som hanteras via Admin Console. Se [Adobe Admin Console-användare](https://helpx.adobe.com/enterprise/using/users.html) i _Administrationshandboken för Enterprise och Teams_ för en översikt över användarhantering och procedurer för att lägga till användare och användargrupper.

## Steg 1: Skapa en användargrupp

**Så här skapar du en användargrupp**:

1. Logga in på Admin Console och gå till **[!UICONTROL Users]** > **[!UICONTROL Users Groups]**.

1. Klicka på **[!UICONTROL New User Group]**. Popup-fönstret _Skapa en ny användargrupp_ öppnas.

1. Lägg till ett informativt användargruppnamn i fältet **[!UICONTROL User group name]** för att identifiera den nya gruppens syfte. Exempel:&quot;Varumärkeshanterare&quot;.

1. Du kan också lägga till en beskrivning av gruppen och dess syfte.

1. Klicka på **[!UICONTROL Save]**. Admin Console öppnar popup-fönstret _Ny grupp_ med namnet på den nyligen skapade gruppen.

Se [Hantera användargrupper](https://helpx.adobe.com/enterprise/using/user-groups.html) i _Administrationshandboken för Enterprise och Teams_.

## Steg 2: Tilldela en GenStudio-systemhanterarprofil till användargruppen

När du har skapat en ny användargrupp och lagt till användare kan du tilldela den här gruppen **Adobe GenStudions systemhanterarprofil**. De berättiganden som är kopplade till den tilldelade profilen ger alla användare i den här gruppen GenStudio [!DNL Brands] behörigheter (skapa, uppdatera och ta bort varumärken).

**Så här tilldelar du en profil till användargruppen**:

1. Navigera till den nya användargruppen och klicka på fliken _Tilldelade produktprofiler_.

1. Klicka på **[!UICONTROL Assign profile]** på fliken _Tilldelade produktprofiler_. Popup-fönstret _Tilldela produkter och profiler_ öppnas.

1. Välj `Adobe GenStudio` i listan _Välj produkter_.

1. Klicka på **[!UICONTROL Apply]**. Popup-fönstret _Välj produktprofiler_ öppnas och visar de produktprofiler som är associerade med Adobe GenStudio.

1. Välj `Adobe GenStudio system manager`.

1. Klicka på **[!UICONTROL Apply]**. Popup-fönstret _Tilldela produkter och profiler_ öppnas och visar produktprofilen för den nya användargruppen.

1. Klicka på **[!UICONTROL Save]**.

Se [Tilldela produktprofiler till användargrupper](https://helpx.adobe.com/enterprise/using/user-groups.html) i _Administrationshandboken för Enterprise och Teams_.

## Steg 3: Skapa ett [!DNL Brands]-projekt

Ett _projekt_ tillhandahåller en lagringsplats där utvalda användare kan spara resurser, i det här fallet [!DNL Brands] resurser.

**Så här skapar du ett [!DNL Brands]-projekt från fliken _Lagring_**:

1. Gå till fliken _Lagring_ i Admin Console.

1. Klicka på **[!UICONTROL Projects]** i sidnavigeringen. Fliken _Projekt_ öppnas.

1. Klicka på **[!UICONTROL Create Project]**. Popup-fönstret _Nytt projekt_ öppnas.

1. Ange `Adobe GenStudio Brands` i projektnamnsfältet. Ange projektnamnet exakt så som det visas här. Ta inte med extra blanksteg eller ändra skiftläget.

1. Klicka på **[!UICONTROL Create]**. Popup-fönstret _Bjud in till projekt_ öppnas.

Se [Hantera projekt](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) i _Administrationshandboken för företag och team_.

## Steg 4: Bjud in användargrupp till projekt

Du kan nu lägga till användargruppen som du nyss skapade i `Adobe GenStudio [!DNL Brands]`-projektet.

**Så här bjuder du in användargruppen till det nyskapade projektet**:

1. Lägg till användargruppen som du nyss skapade i det här projektet från popup-menyn _Bjud in till projekt_ .

1. Välj behörighetsalternativet **Kan redigera**.

1. Klicka på **[!UICONTROL Invite]**.

## Steg 5: Lägg till användare i användargruppen

Om du vill tilldela användare behörighet att skapa, redigera och publicera [!DNL Brands] lägger du till dem i den nya användargruppen.

**Så här lägger du till användare i användargruppen**:

1. Navigera från _Admin Console_ till **[!UICONTROL Users]** > **[!UICONTROL User Groups]**.

1. Markera namnet på användargruppen som du skapade tidigare. Popup-fönstret _Lägg till användare i den här användargruppen_ öppnas.

1. Lägg till en ny eller befintlig användare med antingen användarnamn eller e-postadress. Läs om hur du hanterar användargrupper i [Hantera användargrupper](https://helpx.adobe.com/enterprise/using/user-groups.html) i _Administrationsguiden för Enterprise och team_.

Användare får behörighet att skapa, redigera och publicera [!DNL Brand] för Adobe GenStudio-systemhanterare när de läggs till i gruppen. Användarna får även en automatisk e-postinbjudan om att redigera Adobe GenStudio for Performance Marketing [!DNL Brands]-projektet.
