---
audience: end-user
title: Viktiga principer för att skapa arbetsflöden
description: Lär dig grunderna i arbetsflöden med Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Viktiga principer för att skapa arbetsflöden {#gs-workflow-creation}

Med Adobe Campaign Web kan du skapa arbetsflöden i en visuell arbetsyta för att skapa flerkanalsprocesser som segmentering, kampanjutförande och filbearbetning.

## Vad innehåller ett arbetsflöde? {#gs-workflow-inside}

Arbetsflödesdiagrammet är en representation av vad som ska hända. Det beskriver de olika åtgärder som ska utföras och hur de är sammankopplade.

![](assets/workflow-example.png){zoomable="yes"} {zoomable="yes"}

Varje arbetsflöde innehåller:

* **Aktiviteter**: En aktivitet är en aktivitet som ska utföras. De olika aktiviteterna visas i diagrammet med ikoner. Varje aktivitet har specifika egenskaper och andra egenskaper som är gemensamma för alla aktiviteter.

  I ett arbetsflödesdiagram kan en viss aktivitet producera flera uppgifter, särskilt när det finns en slinga eller återkommande åtgärder.

* **Övergångar**: Övergångar länkar en källaktivitet till en målaktivitet och definierar deras sekvens.

* **Arbetstabeller**: Arbetstabellen innehåller all information som följer med övergången. För varje arbetsflöde används flera arbetstabeller. De data som överförs i dessa tabeller kan användas under hela arbetsflödets livscykel.

## Viktiga steg för att skapa ett arbetsflöde {#gs-workflow-steps}


Det finns två sätt att skapa ett arbetsflöde i kampanjer:

1. Arbetsflöden kan skapas som fristående arbetsflöden på menyn **Arbetsflöden** .

   ![](assets/create-a-standalone-wf.png){zoomable="yes"}

1. Arbetsflöden kan skapas direkt i en kampanj från fliken **Arbetsflöde** i kampanjen. När det ingår i en kampanj körs arbetsflödet tillsammans med alla andra kampanjers arbetsflöden, och alla rapportvärden grupperas på kampanjnivå.

   ![](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

Så här skapar du arbetsflöden:

![](assets/workflow-creation-process.png){zoomable="yes"}

De här stegen beskrivs i följande avsnitt:

1. [Skapa ett arbetsflöde och definiera dess egenskaper](create-workflow.md)
1. [Samordna och konfigurera aktiviteter](orchestrate-activities.md)
1. [Konfigurera avancerade inställningar för ditt arbetsflöde](workflow-settings.md)
1. [Starta arbetsflödet och övervaka dess körning](start-monitor-workflows.md)
