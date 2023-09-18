---
audience: end-user
title: Använda aktiviteten Spara målgruppsarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten för arbetsflöden
badge: label="Beta"
source-git-commit: d0bfb97c3c06f80a6c429fc0c924b339397447d2
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 7%

---


# Spara målgrupp {#save-audience}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="Save an audience"
>abstract="Use this activity to save the workflow audience."
-->

The **Spara målgrupper** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du uppdatera en befintlig målgrupp eller skapa en ny målgrupp utifrån den population som beräknas uppströms i ett arbetsflöde. De målgrupper som skapas läggs till i listan över programmålgrupper och blir tillgängliga via **Målgrupper** -menyn.

Den här aktiviteten används främst för att behålla populationsgrupper som beräknas i samma arbetsflöde genom att konvertera dem till återanvändbara målgrupper. Koppla det till andra målinriktningsaktiviteter som **Bygg målgrupper** eller en **Kombinera** aktivitet.

## Konfiguration

Följ de här stegen för att konfigurera **Spara målgrupper** aktivitet:

1. Lägg till en **Spara målgrupper** till ditt arbetsflöde.

   ![](../assets/workflow-save-audience.png)

1. I **Läge** väljer du den åtgärd du vill utföra:

   * **Skapa eller uppdatera en befintlig målgrupp**: definiera en **Målgruppsetikett**. Om målgruppen redan finns uppdateras den, annars skapas en ny målgrupp.

   * **Uppdatera en befintlig målgrupp**: välj **Målgrupp** som du vill uppdatera bland de befintliga målgrupperna.

1. Välj **Uppdateringsläge** som ska gälla för befintliga målgrupper:

   * **Ersätt målgruppsinnehåll med nya data**: allt målgruppsinnehåll ersätts. Gammal data går förlorad.  Endast datan från den inkommande övergången av målgruppsaktiviteten för att spara sparas. Med det här alternativet raderas målgruppstypen och målgruppsdimensionen för den uppdaterade målgruppen.

   * **Komplett målgrupp med nya data**: det gamla målgruppsinnehållet behålls och data från den sparade målgruppsaktivitetens inkommande övergång läggs till i det.

1. Kontrollera **Generera en utgående övergång** om du vill lägga till en övergång efter **Spara målgrupper** aktivitet.

Innehållet i den sparade målgruppen är sedan tillgängligt i detaljvyn för målgruppen, som du kommer åt via **Målgrupper** -menyn. Kolumnerna som är tillgängliga från den här vyn motsvarar kolumnerna för den inkommande övergången i arbetsflödets **SAve** aktivitet.


## Exempel


