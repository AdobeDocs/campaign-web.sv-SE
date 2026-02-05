---
title: Hantera externt konto
description: Lär dig konfigurera externa konton
exl-id: 52b4ec99-4f55-4e0b-8a54-b25058d97b02
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 2%

---

# Skapa ett externt konto {#create-external-account}

Följ stegen nedan om du vill skapa ett nytt externt konto. De specifika konfigurationsinställningarna beror på vilken typ av externt konto du skapar.

1. Välj **[!UICONTROL External accounts]** under **[!UICONTROL Administration]** på den vänstra panelmenyn.

1. Klicka på **[!UICONTROL Create external account]**.

   ![Skärmbild som visar alternativet att skapa ett externt konto i webbanvändargränssnittet.](assets/external_account_create_1.png)

1. Ange din **[!UICONTROL Label]** och välj det externa kontot **[!UICONTROL Type]**.

   * [Kampanjspecifika typer](external-account.md)
   * [Adobe Solution Integration](integration-external-account.md)
   * [Överför data](transfer-external-account.md)
   * [Extern databas](external-account-database.md)

   ![Skärmbild med fält för att ange etiketten och välja extern kontotyp.](assets/external_account_create_2.png)

1. Klicka på **[!UICONTROL Create]**.

1. Ändra sökvägen **[!UICONTROL Additional options]** eller **[!UICONTROL Internal name]** i listrutan **[!UICONTROL Folder]** om det behövs.

   ![Skärmbild med ytterligare alternativ för konfiguration av internt namn och mappsökväg.](assets/external_account_create_3.png)

1. Aktivera alternativet **[!UICONTROL Exported automatically in packages]** för att automatiskt exportera data som hanteras av det här externa kontot. <!--Exported where??-->

   ![Skärmbild som visar alternativet att aktivera automatisk export i paket.](assets/external_account_create_exported.png)

1. Konfigurera åtkomst till kontot i avsnittet **[!UICONTROL Details]** genom att ange autentiseringsuppgifter baserat på den valda externa kontotypen. [Läs mer](#bounce)

1. Klicka på **[!UICONTROL Test connection]** för att verifiera att konfigurationen är korrekt.

1. Duplicera eller ta bort ditt externa konto på menyn **[!UICONTROL More...]**.

   ![Skärmbild som visar menyn Mer med alternativ för att duplicera eller ta bort det externa kontot.](assets/external_account_create_4.png)

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]**.
