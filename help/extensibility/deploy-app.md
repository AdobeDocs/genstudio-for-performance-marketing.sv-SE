---
title: Distribuera din App Builder-app
description: Driftsätt App Builder-appen eller tillägget för GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Distribuera din app

När du kör din app får du en preliminär ögonblicksbild av din Add-ons beteende innan du distribuerar den. Den här informationen kan underlätta felsökning.

**Så här kör du appen**:

Kör appen i `https://localhost:9080`:

```bash
aio app run
```

**Så här distribuerar du appen**:

1. Navigera till arbetsytan Distribution:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Distribuera appen:

   ```bash
   aio app deploy
   ```

**Så här tvingar du omdistribution**:

Du kan tvinga fram ett bygge och en distribution av ditt program utan att skicka in det igen för godkännande.

>[!NOTE]
>
>Om du framtvingar en programkonstruktion och distribution skrivs din befintliga distribution över. **Testa appen** noggrant i en testmiljö först.

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

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

Om du är nöjd med din add-on kan du distribuera den utan parametern `query`.

Nu kan du [distribuera din app](distribute-app.md).
