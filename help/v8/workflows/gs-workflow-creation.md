---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Viktiga principer för att skapa arbetsflöden {#gs-workflow-creation}

Med Campaign v8 Web kan ni skapa arbetsflöden i en visuell arbetsyta för att utforma flerkanalsprocesser som segmentering, kampanjutförande och filbearbetning.

Arbetsflöden kan skapas antingen som fristående arbetsflöden, från menyn Arbetsflöden eller direkt i en kampanj. I så fall länkas arbetsflödet till kampanjen och körs tillsammans med alla andra kampanjers arbetsflöden.

## Vad innehåller ett arbetsflöde?

Arbetsflödesdiagrammet är en representation av vad som ska hända. Det beskriver de olika åtgärder som ska utföras och hur de är sammankopplade.

![](assets/workflow-example.png)

Varje arbetsflöde innehåller:

* **Verksamhet**: En aktivitet är en uppgift som ska utföras. De olika aktiviteterna visas i diagrammet med ikoner. Varje aktivitet har specifika egenskaper och andra egenskaper som är gemensamma för alla aktiviteter.

   I ett arbetsflödesdiagram kan en viss aktivitet producera flera uppgifter, särskilt när det finns en slinga eller återkommande åtgärder.

* **Övergångar**: Övergångar länkar en källaktivitet till en målaktivitet och definierar deras sekvens.

* **Worktables**: Arbetstabellen innehåller all information som övergången innehåller. Varje arbetsflöde använder flera arbetstabeller. De data som överförs i dessa tabeller kan användas under hela arbetsflödets livscykel.

## De viktigaste stegen för att skapa ett arbetsflöde

De viktigaste stegen för att skapa arbetsflöden är följande:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="Lead" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>Skapa arbetsflödet</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="Sällan" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>Organisera aktiviteter</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="Validering" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>Konfigurera avancerade inställningar (valfritt)</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="starta och övervaka arbetsflöden" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>Starta och övervaka arbetsflödets körning</strong></a>
</div>
<p>
</td>
</tr></table>