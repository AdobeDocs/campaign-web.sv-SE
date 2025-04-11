---
audience: end-user
title: Viktiga principer för att skapa arbetsflöden
description: Lär dig grunderna i arbetsflöden med Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Viktiga principer för att skapa arbetsflöden {#gs-workflow-creation}

Med Adobe Campaign Web kan du skapa arbetsflöden på en visuell arbetsyta för att skapa flerkanalsprocesser som segmentering, kampanjutförande och filbearbetning.

## Vad innehåller ett arbetsflöde? {#gs-workflow-inside}

Arbetsflödesdiagrammet representerar den planerade processen. Det beskriver de olika åtgärder som ska utföras och hur de är sammankopplade.

![Exempeldiagram för arbetsflöde som visar aktiviteter och deras anslutningar](assets/workflow-example.png){zoomable="yes"}

Varje arbetsflöde innehåller:

* **Aktiviteter**: En aktivitet är en aktivitet som ska utföras. Ikonerna i diagrammet representerar de olika aktiviteterna. Varje aktivitet har specifika egenskaper och egenskaper som är gemensamma för alla aktiviteter.

  I ett arbetsflödesdiagram kan en viss aktivitet skapa flera uppgifter, särskilt när det finns en slinga eller återkommande åtgärder.

* **Övergångar**: Övergångar länkar en källaktivitet till en målaktivitet och definierar deras sekvens.

* **Arbetstabeller**: Arbetstabellen innehåller all information som följer med övergången. För varje arbetsflöde används flera arbetstabeller. Data i dessa tabeller kan användas under arbetsflödets hela livscykel.

## Viktiga steg för att skapa ett arbetsflöde {#gs-workflow-steps}

Det finns två sätt att skapa ett arbetsflöde i kampanjer:

1. Arbetsflöden kan skapas som fristående arbetsflöden på menyn **Arbetsflöden** .

   ![Skärmbild av gränssnittet för att skapa ett fristående arbetsflöde](assets/create-a-standalone-wf.png){zoomable="yes"}

1. Arbetsflöden kan skapas direkt i en kampanj från fliken **Arbetsflöde** i kampanjen. När arbetsflödet ingår i en kampanj körs det tillsammans med alla andra kampanjers arbetsflöden, och rapportvärdena grupperas på kampanjnivå.

   ![Skärmbild av gränssnittet för att skapa ett arbetsflöde i en kampanj](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

Så här skapar du arbetsflöden:

![Diagram som visar arbetsflödesskapandet](assets/workflow-creation-process.png){zoomable="yes"}

De här stegen beskrivs i följande avsnitt:

1. [Skapa ett arbetsflöde och definiera dess egenskaper](create-workflow.md)
1. [Samordna och konfigurera aktiviteter](orchestrate-activities.md)
1. [Konfigurera avancerade inställningar för ditt arbetsflöde](workflow-settings.md)
1. [Starta arbetsflödet och övervaka dess körning](start-monitor-workflows.md)