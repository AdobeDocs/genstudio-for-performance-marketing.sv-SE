---
title: Tillhandahåll Adobe GenStudio for Performance Marketing
description: Läs om hur du distribuerar GenStudio for Performance Marketing-produkten.
level: Beginner
feature: Generative AI
role: Admin
exl-id: 7a9f8de1-79e7-455c-ae0f-e7646febc483
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Tillhandahåll Adobe GenStudio for Performance Marketing

En Adobe-systemadministratör utför initiala provisioneringsåtgärder i [Adobe Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html#Overview). Från Admin Console har en Adobe-systemadministratör åtkomst till GenStudio produktprofil och kan tilldela användare tillgängliga produktlicenser.

>[!NOTE]
>
>Endast Adobe systemadministratörer kan implementera aktiveringsuppgifter som kräver åtkomst från Adobe Admin Console.

>[!IMPORTANT]
>
>Lägg inte till nya, eller redigera eller ta bort, befintliga produktprofiler. Om du ändrar standardproduktprofilerna kan det allvarligt störa driftsättningen av GenStudio for Performance Marketing.

## Steg 1: Gå till produktprofilen i Adobe Admin Console

Inom Admin Console definierar produktprofilen regler och användarprofiler som är unika för varumärken och kampanjskapande och -hantering inom GenStudio for Performance Marketing.

**Så här kommer du åt GenStudio produktprofil**

1. Klicka på länken **Kom igång** i ditt välkomstmeddelande för att navigera till [Adobe Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html#Overview).

1. Logga in på Admin Console med din Adobe ID.

   När inloggningen är klar visas fliken _Översikt_ i Adobe Admin Console.

1. Gå till fliken _Produkter_. På den här fliken visas alla Adobe-produkter som din organisation har köpt.

1. Välj **[!UICONTROL GenStudio]** i listan över produkter. På konsolen visas GenStudio produktprofil, som visar viktig information om de produktlicenser din organisation har köpt. Här finns även alternativ för att hantera dessa licenser.

Du kan nu tilldela licenser till (provisionera) användare till GenStudio for Performance Marketing. Om du har loggat in i fel organisation växlar du till rätt organisation innan du försöker tilldela behörigheter till användare. Om du vill ändra din organisation klickar du på organisationsnamnet i det övre högra hörnet och väljer **GenStudio** -organisationen.

## Steg 2: Tillhandahåll användare

Att tilldela användare i Admin Console är processen att tilldela produktlicenser till användare. Dessa användare måste tillhöra den IMS-organisation som anges i produktprofilen. Du kan tilldela användare till din GenStudio for Performance Marketing-organisation på samma sätt som du distribuerar användare till andra Adobe-produkter. Du kan lägga till användare manuellt eller importera flera användare samtidigt.

>[!TIP]
>
>Tilldela dig själv behörighet som systemadministratör för GenStudio för att utföra systemhanteringsuppgifter i GenStudio for Performance Marketing.

**Förutsättningar**:

Förbered dig för etablering genom att först identifiera grundläggande information:

* Förnamn och efternamn
* Företagets e-postadress
* Typ av berättiganden att tilldela användare

Mer information om hur du tilldelar GenStudio for Performance Marketing-användarroller finns i [Användarroller och behörigheter](user-roles.md).

Du kan lägga till användare individuellt eller importera kontoinformation för flera användare:

* [Hantera användare individuellt](https://helpx.adobe.com/se/enterprise/using/manage-users-individually.html#add-users)

* [Hantera flera användare/massöverföring av CSV](https://helpx.adobe.com/se/enterprise/using/bulk-upload-users.html)

När du har anslutit användare till din organisations GenStudio for Performance Marketing kan en GenStudio-systemadministratör [konfigurera din organisations varumärke- och medieriktlinjer](get-started.md).
