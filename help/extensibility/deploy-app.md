---
title: Distribuera din App Builder-app
description: Driftsätt App Builder-appen eller tillägget för GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 6fef5933421a56cf9f77c19bc198f017ee6c117e
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Distribuera din app

När du kör ditt program får du en preliminär ögonblicksbild av ditt Add-on-beteende innan du distribuerar det. Den här informationen kan underlätta felsökning. Du kan tvinga fram bygge och driftsättning av ett distribuerat program utan att skicka in det på nytt för godkännande.

**Så här kör du appen**:

Kör appen i `https://localhost:9080`:

```bash
aio app run
```

**Så här distribuerar du appen**:

1. Navigera till arbetsytan Distribution. Om du till exempel vill navigera till arbetsytan Produktion:

   ```bash
   aio app use -w Production
   ```

1. Distribuera appen:

   ```bash
   aio app deploy
   ```

**Så här tvingar du omdistribution**:

>[!NOTE]
>
>Om du framtvingar bygge och distribution skrivs din befintliga distribution över. Testa appen noggrant i en testmiljö först.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**Så här skapar och distribuerar du samtidigt**:

```bash
aio app deploy --force-build --force-deploy
```

**Så här visar du appen**:

Efter distributionen kan du visa appen i GenStudio for Performance Marketing genom att lägga till en `query`-parameter i GenStudio for Performance Marketing URL:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Om du är nöjd med din add-on kan du distribuera den utan parametern `query`.

Du kan nu [distribuera din app](distribute-app.md).
