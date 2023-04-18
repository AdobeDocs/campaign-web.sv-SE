---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 9a4ca68d475cfbbcccb7a5b0d84f841589824288
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Viktiga principer för att skapa arbetsflöden {#gs-workflow-creation}

Ett arbetsflöde är en processdefinition: arbetsflödesdiagrammet, som är en representation av vad som ska hända. Ett arbetsflöde är också en instans av den här processen: en arbetsflödesinstans, vilket är en representation av vad som faktiskt händer.

Arbetsflödesmallen beskriver de olika uppgifter som ska utföras och hur de länkas samman. Uppgiftsmallarna kallas aktiviteter och representeras av ikoner. De länkas ihop av övergångar.

skärmbild TBD

## Vad innehåller ett arbetsflöde?

Varje arbetsflöde innehåller:

* **Verksamhet**: En aktivitet beskriver en uppgiftsmall. De olika aktiviteterna som är tillgängliga visas i diagrammet med ikoner. Varje typ har gemensamma egenskaper och specifika egenskaper.

   I ett arbetsflödesdiagram kan en viss aktivitet producera flera uppgifter, särskilt när det finns en slinga eller återkommande åtgärder.

* **Övergångar**: Med övergångar kan du länka aktiviteter och definiera deras sekvens. En övergång länkar en källaktivitet till en målaktivitet.

* **Worktables**: Arbetstabellen innehåller all information som övergången innehåller. Varje arbetsflöde använder flera arbetstabeller. De data som överförs i dessa tabeller kan accelereras och användas under arbetsflödets hela livscykel, så länge som de inte rensas. Det går att tömma tabeller som inte behövs varje gång arbetsflödet är passivat och eventuellt under körningen av de största arbetsflödena för att undvika att servern överbelastas.

## Fristående arbetsflöden och kampanjarbetsflöden

Arbetsflöden kan skapas antingen som fristående arbetsflöden eller inifrån en kampanj.

TBD: Detaljerade detaljer mellan fristående arbetsflöden och kampanjarbetsflöden.

## De viktigaste stegen för att skapa ett arbetsflöde

De viktigaste stegen för att skapa arbetsflöden är följande:

TBD: grafik som visar hela processen med förklaring och referens till dokumentsidor