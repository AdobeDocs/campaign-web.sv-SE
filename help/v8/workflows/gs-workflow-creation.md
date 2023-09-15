---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 53148300ecb5d52d89875519c44ae979d29a4d76
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---


# Viktiga principer för att skapa arbetsflöden {#gs-workflow-creation}

Med Campaign v8 Web kan ni skapa arbetsflöden i en visuell arbetsyta för att utforma flerkanalsprocesser som segmentering, kampanjutförande och filbearbetning.


## Vad innehåller ett arbetsflöde? {#gs-workflow-inside}

Arbetsflödesdiagrammet är en representation av vad som ska hända. Det beskriver de olika åtgärder som ska utföras och hur de är sammankopplade.

![](assets/workflow-example.png)

Varje arbetsflöde innehåller:

* **Verksamhet**: En aktivitet är en uppgift som ska utföras. De olika aktiviteterna visas i diagrammet med ikoner. Varje aktivitet har specifika egenskaper och andra egenskaper som är gemensamma för alla aktiviteter.

  I ett arbetsflödesdiagram kan en viss aktivitet producera flera uppgifter, särskilt när det finns en slinga eller återkommande åtgärder.

* **Övergångar**: Övergångar länkar en källaktivitet till en målaktivitet och definierar deras sekvens.

* **Worktables**: Arbetstabellen innehåller all information som övergången innehåller. För varje arbetsflöde används flera arbetstabeller. De data som överförs i dessa tabeller kan användas under hela arbetsflödets livscykel.

## Viktiga steg för att skapa ett arbetsflöde {#gs-workflow-steps}


Det finns två sätt att skapa ett arbetsflöde i kampanjer:

1. Arbetsflöden kan skapas som fristående arbetsflöden från **Arbetsflöden** -menyn.

   ![](assets/create-a-standalone-wf.png)

1. Arbetsflöden kan skapas direkt i en kampanj från **Arbetsflöde** -fliken i kampanjen. När det ingår i en kampanj körs arbetsflödet tillsammans med alla andra kampanjers arbetsflöden, och alla rapportvärden grupperas på kampanjnivå.

   ![](assets/create-a-wf-from-a-campaign.png)


Så här skapar du arbetsflöden:

![](assets/workflow-creation-process.png)

De här stegen beskrivs i följande avsnitt:

1. [Skapa ett arbetsflöde och definiera dess egenskaper](create-workflow.md)
1. [Samordna och konfigurera aktiviteter](orchestrate-activities.md)
1. [Konfigurera avancerade inställningar för ditt arbetsflöde](workflow-settings.md)
1. [Starta arbetsflödet och övervaka dess körning](start-monitor-workflows.md)

