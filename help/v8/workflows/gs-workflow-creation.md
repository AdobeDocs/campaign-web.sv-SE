---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---


# Viktiga principer för att skapa arbetsflöden {#gs-workflow-creation}

Med Campaign v8 Web kan ni skapa arbetsflöden i en visuell arbetsyta för att utforma flerkanalsprocesser som segmentering, kampanjutförande och filbearbetning.

Arbetsflöden kan skapas antingen som fristående arbetsflöden, från menyn Arbetsflöden eller från en kampanj från menyn Kampanjer.

TBD: Detaljerade detaljer mellan fristående arbetsflöden och kampanjarbetsflöden.

## Vad innehåller ett arbetsflöde?

Arbetsflödesdiagrammet är en representation av vad som ska hända. Det beskriver de olika åtgärder som ska utföras och hur de är sammankopplade.

Varje arbetsflöde innehåller:

* **Verksamhet**: En aktivitet är en uppgift som ska utföras. De olika aktiviteterna visas i diagrammet med ikoner. Varje aktivitet har specifika egenskaper och andra egenskaper som är gemensamma för alla aktiviteter.

   I ett arbetsflödesdiagram kan en viss aktivitet producera flera uppgifter, särskilt när det finns en slinga eller återkommande åtgärder.

* **Övergångar**: Övergångar länkar en källaktivitet till en målaktivitet och definierar deras sekvens.

* **Worktables**: Arbetstabellen innehåller all information som övergången innehåller. Varje arbetsflöde använder flera arbetstabeller. De data som överförs i dessa tabeller kan accelereras och användas under arbetsflödets hela livscykel, så länge som de inte rensas. Det går att tömma tabeller som inte behövs varje gång arbetsflödet är passivat och eventuellt under körningen av de största arbetsflödena för att undvika att servern överbelastas.

## De viktigaste stegen för att skapa ett arbetsflöde

De viktigaste stegen för att skapa arbetsflöden är följande:

TBD: grafik som visar hela processen med förklaring och referens till dokumentsidor

skapa och definiera egenskaper > samordna aktiviteter på arbetsytan > konfigurera inställningar om det behövs > starta körningen och övervaka