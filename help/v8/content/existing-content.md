---
audience: end-user
title: Importera e-postinnehåll
description: Lär dig hur du importerar e-postinnehåll
exl-id: ef9c8e6f-f422-404e-9ebb-a89d1bd45e7f
badge: label="Beta"
source-git-commit: ed12d289c1180fe8705d2c143bd9dce4ed96e313
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Importera e-postinnehåll {#existing-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_import_content"
>title="Använd befintligt e-postinnehåll"
>abstract="Med e-postdesignern kan du importera befintligt HTML-innehåll. Innehållet kan vara en HTML-fil med en infogad formatmall eller en ZIP-mapp med HTML-filen, formatmallen (.css) och bilder."

Du kan importera befintligt HTML-innehåll i e-postdesignern. Innehållet kan vara:

* An **HTML-fil** med en infogad formatmall,
* A **ZIP-mapp** med HTML-filen, formatmallen (.css) och bilderna.

  >[!NOTE]
  >
  >ZIP-filstrukturen har inga begränsningar. Referenserna måste dock vara relativa och passa i trädstrukturen i ZIP-mappen.

Om du vill importera en fil som innehåller HTML-innehåll följer du stegen nedan:

1. På [E-postdesigner](get-started-email-designer.md) startsida, välja **[!UICONTROL Import HTML]**.

   ![](assets/html-import.png)

1. Dra och släpp HTML- eller ZIP-filen med HTML och klicka på **[!UICONTROL Import]**.

1. När HTML-innehållet har överförts är ditt innehåll **[!UICONTROL Compatibility mode]**.

   I det här läget kan du bara anpassa texten, lägga till länkar eller inkludera resurser i innehållet.

   ![](assets/html-imported.png)

1. Om du vill kunna utnyttja e-postdesignerns innehållskomponenter ska du gå till **[!UICONTROL HTML converter]** och klicka **[!UICONTROL Convert]**.

   ![](assets/html-imported-2.png)

   >[!NOTE]
   >
   > Använda `<table>` taggen som det första lagret i en HTML-fil kan orsaka formatförlust, inklusive inställningar för bakgrund och bredd i den översta lagertaggen.

1. Du kan nu anpassa den importerade filen efter behov med e-postdesignerfunktionerna [Läs mer](content-components.md).

