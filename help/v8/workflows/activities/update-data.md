---
audience: end-user
title: Använd aktiviteten Uppdatera arbetsflöde för data
description: Lär dig hur du använder arbetsflödesaktiviteten Uppdatera data
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 9%

---

# Uppdatera data {#update-data}

Aktiviteten **Uppdatera data** är en **datahanteringsaktivitet**. Det gör att du kan utföra en massuppdatering av fält i databasen. Med flera alternativ kan du anpassa datauppdateringen.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update it if it has already been added. You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely.

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or directly use reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section lets you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.
-->

## Konfigurera aktiviteten Uppdatera data {#update-data-configuration}

Om du vill konfigurera aktiviteten **Uppdatera data** lägger du till aktiviteten i arbetsflödet och definierar en etikett.

![Dataaktivitet för uppdatering av arbetsflöde](../assets/workflow-update-data.png)

### Åtgärdstyp

I fältet **Åtgärdstyp** kan du välja vilken process som ska utföras på data i databasen:

* **Infoga eller uppdatera**: Infoga data eller uppdatera dem om posterna redan finns i databasen.
* **Infoga**: Infoga endast data. Poster som redan finns uppdateras inte. Om avstämningskriterier definieras läggs endast icke avstämda poster till.
* **Uppdatera**: Uppdatera data för de poster som redan finns i databasen.
* **Ta bort**: Ta bort data.

I fältet **Batchstorlek** kan du välja antalet inkommande övergångselement som ska uppdateras. Om du till exempel anger 500 uppdateras de första 500 posterna som bearbetas.

### Registrerings-ID

I det här avsnittet kan du ange hur posterna i databasen ska identifieras:

* Om dataposter relaterar till en befintlig måldimension markerar du alternativet **Använda måldimensionen** och väljer det i fältet **Måldimension att uppdatera**.
* Du kan också välja **Använda anpassade länkar** och ange en eller flera länkar som gör att data i databasen kan identifieras.
* Om den valda åtgärdstypen kräver en uppdatering använder du alternativet **Använda avstämningsregler**.

### Fält som ska uppdateras

I avsnittet **Fält som ska uppdateras** lägger du till de fält som uppdateringen ska tillämpas på. Om det behövs lägger du till villkor så att uppdateringen genomförs. Använd fältet **Om** har tagits med i beräkningen för att definiera villkor. Villkoren tillämpas sekventiellt i listordningen. Använd pilarna till höger för att ändra uppdateringsordningen. Du kan använda samma målfält flera gånger.

Länka fält automatiskt med knappen **Automatisk mappning**. Automatisk länkning identifierar fält med samma namn.

Under en **Infoga eller uppdatera**-åtgärdstyp väljer du den åtgärd som ska användas för varje fält separat. Använd fältet **Åtgärdstyp** för att ange önskat värde.

### Avancerade alternativ

I avsnittet **Avancerade alternativ** kan du ange ytterligare alternativ för att hantera dataraderingsuppdateringar och dubbletter.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

De två sista alternativen gör att du kan utföra specifika åtgärder:

* **Generera en utgående övergång**: Skapar en utgående övergång som aktiveras i slutet av körningen. Uppdatering signalerar vanligtvis slutet på ett målarbetsflöde och alternativet är därför inte aktiverat som standard.

* **Generera en utgående övergång för avslagen**: Skapar en utgående övergång som innehåller poster som inte har bearbetats korrekt efter uppdateringen (till exempel om det finns en dubblett). Uppdateringen markerar vanligtvis slutet av ett målarbetsflöde och alternativet är inte aktiverat som standard.