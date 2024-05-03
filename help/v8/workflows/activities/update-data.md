---
audience: end-user
title: Använd aktiviteten Uppdatera arbetsflöde för data
description: Lär dig hur du använder arbetsflödesaktiviteten Uppdatera data
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 11%

---

# Uppdatera data {#update-data}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Uppdatera dataaktivitet"
>abstract="Aktiviteten Uppdatera data är nu tillgänglig för användning i arbetsflöden. Använd aktiviteten Uppdatera data för att utföra en massuppdatering av fält i databasen. Flera alternativ föreslås för att anpassa uppdateringstypen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"



The **Uppdatera data** aktiviteten är en **Datahantering** aktivitet. Det gör att du kan utföra en massuppdatering på fält i databasen. Flera alternativ gör att du kan anpassa datauppdateringen.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## Konfigurera aktiviteten Uppdatera data{#update-data-configuration}

Konfigurera **Uppdatera data** börjar du med att lägga till aktiviteten i arbetsflödet och definierar en etikett.

![](../assets/workflow-update-data.png)

### Åtgärdstyp

The **Åtgärdstyp** kan du välja vilken process som ska utföras på data i databasen:

* **Infoga eller uppdatera**: infoga data eller uppdatera dem om posterna redan finns i databasen.
* **Infoga**: endast infoga data. Posterna som redan finns uppdateras inte. Om avstämningskriterier definieras läggs endast icke avstämda poster till.
* **Uppdatera**: Uppdatera data för de poster som redan finns i databasen.
* **Ta bort**: delete data.

The **Batchstorlek** I kan du välja hur många inkommande övergångselement som ska uppdateras. Om du till exempel anger 500 uppdateras de första 500 posterna som behandlas.

### Registrerings-ID

I det här avsnittet kan du ange hur posterna i databasen ska identifieras:

* Om datainmatningarna relaterar till en befintlig måldimension väljer du **Använda målgruppsdimensionen** och välj det i **Måldimension att uppdatera** fält.
* Du kan också välja **Använda anpassade länkar** och ange en eller flera länkar som gör det möjligt att identifiera data i databasen
* Om den valda åtgärdstypen kräver en uppdatering måste du använda **Använda avstämningsregler** alternativ.

### Fält som ska uppdateras

I **Fält som ska uppdateras** lägger du till de fält som uppdateringen ska tillämpas på och, om det behövs, lägger till villkor så att uppdateringen utförs. Använd **Beaktas om** fält. Villkoren tillämpas i en efter en beroende på listordningen. Använd pilarna till höger för att ändra uppdateringsordningen. Du kan använda samma målfält flera gånger.

Du kan länka fält automatiskt med **Automatisk mappning** -knappen. Automatisk länkning identifierar fält med samma namn.

Under en **Infoga eller uppdatera** åtgärdstyp kan du välja en åtgärd som ska användas för varje fält. Om du vill göra det väljer du det värde du vill ha i dialogrutan **Åtgärdstyp** fält.

### Avancerade alternativ

The **Avancerade alternativ** Med kan du ange ytterligare alternativ för att hantera både uppdatering och dubbletter.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

De två sista alternativen gör att du kan utföra specifika åtgärder:

* **Generera en utgående övergång**: skapar en utgående övergång som aktiveras i slutet av körningen. Uppdatering signalerar vanligtvis slutet på ett målarbetsflöde och alternativet är därför inte aktiverat som standard.

* **Generera en utgående övergång för projekten**: skapar en utgående övergång som innehåller poster som inte har bearbetats korrekt efter uppdateringen (till exempel om det finns en dubblett). Uppdateringen markerar vanligtvis slutet av ett målarbetsflöde och därför är alternativet inte aktiverat som standard.
