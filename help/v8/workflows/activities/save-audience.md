---
audience: end-user
title: Använda aktiviteten Spara målgruppsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 5%

---


# Spara målgrupp {#save-audience}

>[!CONTEXTUALHELP]
>id="???"
>title="Spara målgruppsaktivitet"
>abstract="Med aktiviteten Spara målgrupp kan du ..."

Mode Audience label Adobe Campaign kommer att matcha den här etiketten mot befintliga målgrupper. Om den hittar en matchning kommer den att uppdatera den målgruppen, annars kommer den att skapa en ny målgrupp.
Uppdateringsmetod

Ersätt målgruppen med nya data

Fullständig målgrupp med nya datamapplistor (/Profiler och mål/listor/)

Generera en utgående övergång


The **Spara målgrupper** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du uppdatera en befintlig målgrupp eller skapa en ny målgrupp utifrån den population som beräknas uppströms i ett arbetsflöde. De målgrupper som skapas läggs till i listan över programmålgrupper och blir tillgängliga via **Målgrupper** -menyn.

Den här aktiviteten används främst för att behålla populationsgrupper som beräknas i samma arbetsflöde genom att konvertera dem till återanvändbara målgrupper. Koppla det till andra målinriktningsaktiviteter som **Bygg målgrupper** eller en **Kombinera** aktivitet.

## Konfiguration

Följ de här stegen för att konfigurera **Spara målgrupper** aktivitet:

1. Lägg till en **Spara målgrupper** till ditt arbetsflöde.

   <!--![](../assets/workflow-save-audience.png)-->

1. I **Läge** väljer du den åtgärd du vill utföra:

   * **Skapa eller uppdatera en befintlig målgrupp**: definiera en **Målgruppsetikett**. Om målgruppen redan finns uppdateras den, annars skapas en ny målgrupp.

   * **Uppdatera en befintlig målgrupp**: välj **Målgrupp** som du vill uppdatera bland de befintliga målgrupperna.

1. Välj **Uppdateringsläge** som ska gälla för befintliga målgrupper:

   * **Ersätt målgruppsinnehåll med nya data**: allt målgruppsinnehåll ersätts. Gammal data går förlorad.  Endast datan från den inkommande övergången av målgruppsaktiviteten för att spara sparas. Med det här alternativet raderas målgruppstypen och målgruppsdimensionen för den uppdaterade målgruppen.

   * **Komplett målgrupp med nya data**: det gamla målgruppsinnehållet behålls och data från den sparade målgruppsaktivitetens inkommande övergång läggs till i det.

1. Kontrollera **Generera komplement** om du vill utnyttja den återstående populationen. Därefter läggs ytterligare en övergång till aktiviteten.

Innehållet i den sparade målgruppen är sedan tillgängligt i detaljvyn för målgruppen, som du kommer åt via **Målgrupper** -menyn. Kolumnerna som är tillgängliga från den här vyn motsvarar kolumnerna för den inkommande övergången i arbetsflödets **SAve** aktivitet.


## Exempel



