---
audience: end-user
title: Planer och program
description: Lär dig skapa och konfigurera planer och program i Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Planer och program {#plan-and-programs}

Med Adobe Campaign kan du konfigurera mapphierarkin för marknadsföringsplaner och program.

Adobe rekommenderar följande hierarki för att bättre organisera de här komponenterna: Planera `>` program `>` - kampanjer.

* En **plan** kan innehålla flera program. Det definierar strategiska mål för en viss period.
* Ett **program** kan innehålla andra program samt kampanjer, arbetsflöden och landningssidor.
* En **kampanj** kan innehålla leveranser, arbetsflöden och landningssidor.

## Skapa och konfigurera en plan {#create-plan}

Skapa en mapp med mapptypen **[!UICONTROL Plan]** om du vill skapa en plan. [Läs mer om hur du skapar en mapp](../get-started/work-with-folders.md)

![Skärmbild som visar hur en planmapp skapas](assets/plan_create.png){zoomable="yes"}

Gå till **[!UICONTROL Folder settings]** för din plan för att hantera den.

![Skärmbild som visar mappinställningarna för en plan](assets/plan_settings.png){zoomable="yes"}

Definiera **[!UICONTROL Custom options]** och ange schemaläggningsdatumet för din plan.

![Skärmbild som visar anpassade alternativ för en plan](assets/plan_options.png){zoomable="yes"}

Så här hanterar du **[!UICONTROL Custom options]**:

1. Gå till **[!UICONTROL Schemas]**.
1. Välj **[!UICONTROL Editable]**-scheman i filtren.
1. Klicka på ikonen **[!UICONTROL Edit custom details]**.

![Skärmbild som visar redigering av anpassad information för en plan](assets/plan_edit.png){zoomable="yes"}

Konfigurera anpassade alternativ:

![Skärmbild som visar konfigurationen av anpassade fält för en plan](assets/plan_customfields.png){zoomable="yes"}

## Skapa och konfigurera ett program

Om du vill skapa ett program i din plan ([Läs mer om hur du skapar en plan](#create-plan)) navigerar du till din plan och skapar en mapp med mapptypen **[!UICONTROL Program]**. [Läs mer om hur du skapar en mapp](../get-started/work-with-folders.md).

![Skärmbild som visar hur en programmapp skapas](assets/program_create.png){zoomable="yes"}

Gå till **[!UICONTROL Folder settings]** för ditt program för att hantera det.

![Skärmbild som visar mappinställningarna för ett program](assets/program_settings.png){zoomable="yes"}

Definiera **[!UICONTROL Custom options]** och ange schemaläggningsdatumet för ditt program.

![Skärmbild som visar anpassade alternativ för ett program](assets/program_options.png){zoomable="yes"}

Så här hanterar du **[!UICONTROL Custom options]**:

1. Gå till **[!UICONTROL Schemas]**.
1. Välj **[!UICONTROL Editable]**-scheman i filtren.
1. Klicka på ikonen **[!UICONTROL Edit custom details]**.

![Skärmbild som visar redigering av anpassad information för ett program](assets/program_edit.png){zoomable="yes"}

Konfigurera anpassade alternativ:

![Skärmbild som visar konfigurationen av anpassade fält för ett program](assets/program_customfields.png){zoomable="yes"}

## Länka en kampanj till ett program

Du kan länka en kampanj till ett program på två sätt:

### Sätt 1: Du har redan ett program och vill skapa en länkad kampanj

Om du vill länka en ny kampanj till ditt program skapar du kampanjen direkt i programmet.

![Skärmbild som visar hur en kampanj har skapats i ett program](assets/program_campaign_create.png){zoomable="yes"}

**[!UICONTROL Folder]**-inställningarna fylls automatiskt i med sökvägen till ditt program.

![Skärmbild som visar mappinställningarna för en kampanj som är länkad till ett program](assets/program_campaign_folder.png){zoomable="yes"}

### Way #2: Du har redan en befintlig kampanj och vill länka den till ett befintligt program

Gå till knappen **[!UICONTROL Settings]** för kampanjen som du vill länka till ditt program.

![Skärmbild som visar inställningsknappen för en kampanj](assets/campaign_settings.png){zoomable="yes"}

Klicka på ikonen **[!UICONTROL Folder]** i inställningarna för **[!UICONTROL Folder]** i **[!UICONTROL Properties]** för att välja din **[!UICONTROL Program]**-mapp.

![Skärmbild som visar mappvalet för att länka en kampanj till ett program](assets/campaign_folder.png){zoomable="yes"}

Markera mappen **[!UICONTROL Program]**, klicka på knappen **[!UICONTROL Confirm]** och klicka sedan på knappen **[!UICONTROL Save and Close]** .

![Skärmbild som visar en kampanj länkad till ett program](assets/campaign_linked.png){zoomable="yes"}

Din kampanj visas nu i ditt program.

![Skärmbild som visar en kampanj i ett program](assets/campaign_in_program.png){zoomable="yes"}