---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha"
exl-id: 8aa76369-c9f3-4c5b-9a51-101b239727e6
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 3%

---

# Starta och övervaka arbetsflödet {#start-monitor}

När du har skapat arbetsflödet och utformat de uppgifter som ska utföras på arbetsytan kan du starta det och övervaka hur det körs.

## Starta arbetsflödet {#start}

Navigera till **[!UICONTROL Workflows]** -menyn eller den associerade kampanjen och klicka på **[!UICONTROL Start]** i det övre högra hörnet av arbetsytan.

När arbetsflödet körs körs varje aktivitet på arbetsytan i sekventiell ordning tills arbetsflödets slut nås.

Du kan spåra förloppet för målprofiler i realtid med ett visuellt flöde. På så sätt kan du snabbt identifiera status för varje aktivitet och antalet profiler som växlar mellan dem.

![](assets/workflow-execution.png)

>[!NOTE]
>
>Du kan inaktivera det visuella flödet med **[!UICONTROL Hide progression]** i det övre åtgärdsfältet på arbetsytan.

## Körning av övervakningsaktivitet {#activities}

Med visuella indikatorer i det övre högra hörnet av varje aktivitetsruta kan du kontrollera deras körning:

| Visuell indikator | Beskrivning |
|-----|------------|
| ![](assets/activity-status-pending.png) | Aktiviteten körs för närvarande. |
| ![](assets/activity-status-orange.png) | Aktiviteten kräver din uppmärksamhet. Detta kan inbegripa att bekräfta leveransen eller vidta nödvändiga åtgärder. |
| ![](assets/activity-status-red.png) | Aktiviteten har påträffat ett fel. Du löser problemet genom att öppna arbetsflödesloggarna för mer information. |
| ![](assets/activity-status-green.png) | Aktiviteten har körts. |

## Övervaka loggar och uppgifter {#logs-tasks}

Övervakning av arbetsflöden, loggar och uppgifter är ett viktigt steg för att analysera dina arbetsflöden och se till att de körs som de ska. De är tillgängliga via **[!UICONTROL Logs]** ikon som är tillgänglig i åtgärdsverktygsfältet och i varje aktivitets egenskapspanel.

The **[!UICONTROL Logs and tasks]** -menyn innehåller en historik över arbetsflödets körning, där alla användaråtgärder och påträffade fel registreras. Den här historiken sparas under den tid som anges i arbetsflödet [körningsalternativ](workflow-settings.md). Under den här tidsperioden sparas alla meddelanden, även efter att arbetsflödet har startats om. Om du inte vill spara meddelandena från en tidigare körning klickar du på knappen **[!UICONTROL Purge history]** -knappen.

![](assets/workflow-logs.png)

Det finns två typer av information:

* The **[!UICONTROL Log]** -fliken innehåller körningshistoriken för alla arbetsflödesaktiviteter. Den indexerar de åtgärder som utförts och körningsfel i kronologisk ordning.
* The **[!UICONTROL Tasks]** -fliken innehåller information om aktiviteternas körningssekvens.

På båda flikarna kan du välja vilka kolumner som ska visas och i vilken ordning de ska visas, tillämpa filter och använda sökfältet för att snabbt hitta önskad information.

## Kommandon för arbetsflödeskörning {#execution-commands}

Åtgärdsfältet i det övre högra hörnet innehåller kommandon som gör att du kan hantera arbetsflödets körning. Du kan:

* **[!UICONTROL Start]** / **[!UICONTROL Resume]** körningen av arbetsflödet, som sedan får statusen Pågår. Om arbetsflödet pausades återupptas det, i annat fall startas det och de inledande aktiviteterna aktiveras sedan.

* **[!UICONTROL Pause]** körningen av arbetsflödet, som sedan får statusen Pausad. Inga nya aktiviteter aktiveras förrän de återupptas, men pågående åtgärder avbryts inte.

* **[!UICONTROL Stop]** ett arbetsflöde som körs och som sedan får statusen Slutfört. De pågående åtgärderna avbryts om möjligt. Du kan inte återuppta arbetsflödet från samma plats som det stoppades.
