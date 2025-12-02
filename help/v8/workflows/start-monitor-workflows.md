---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Starta och övervaka arbetsflödena {#start-monitor}

När du har skapat arbetsflödet och utformat de uppgifter som ska utföras på arbetsytan kan du starta det och övervaka hur det körs.

## Starta arbetsflödet {#start}

Om du vill starta arbetsflödet går du till menyn **[!UICONTROL Workflows]** eller den associerade kampanjen och klickar på knappen **[!UICONTROL Start]** i det övre högra hörnet av arbetsytan.

När arbetsflödet körs körs varje aktivitet på arbetsytan sekventiellt tills arbetsflödets slut nås.

Du kan spåra förloppet för målprofiler i realtid med ett visuellt flöde. På så sätt kan du snabbt identifiera status för varje aktivitet och antalet profiler som övergår mellan dem.

![Visuell representation av arbetsflödeskörning pågår.](assets/workflow-execution.png){zoomable="yes"}

## Arbetsflödesövergångar {#transitions}

I arbetsflöden lagras data som överförs från en aktivitet till en annan via övergångar i en tillfällig arbetstabell. Dessa data kan visas för varje övergång. Om du vill visa data väljer du en övergång för att öppna egenskaperna på skärmens högra sida.

* Klicka på **[!UICONTROL Preview schema]** för att visa arbetstabellens schema.
* Klicka på **[!UICONTROL Preview results]** om du vill visa data som har transporterats i den valda övergången.

![Exempel på övergångsegenskaper och förhandsgranskning av data.](assets/transition.png){zoomable="yes"}

## Körning av övervakningsaktivitet {#activities}

Med visuella indikatorer i det övre högra hörnet av varje aktivitetsruta kan du kontrollera deras körningsstatus:

| Visuell indikator | Beskrivning |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | Aktiviteten körs för närvarande. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | Aktiviteten kräver din uppmärksamhet. Detta kan inbegripa att bekräfta leveransen eller vidta nödvändiga åtgärder. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | Aktiviteten har påträffat ett fel. Du löser problemet genom att öppna arbetsflödesloggarna för mer information. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | Aktiviteten har körts. |

## Övervaka loggar och uppgifter {#logs-tasks}

Övervakning av arbetsflödesloggar och uppgifter är ett viktigt steg för att analysera dina arbetsflöden och säkerställa att de körs som de ska. Loggar och uppgifter är tillgängliga från ikonen **[!UICONTROL Logs]** som är tillgänglig i åtgärdsverktygsfältet och i varje aktivitets egenskapspanel.

Menyn **[!UICONTROL Logs and tasks]** innehåller en historik över arbetsflödeskörningen, där alla användaråtgärder och påträffade fel registreras. Den här historiken sparas så länge som anges i arbetsflödets [körningsalternativ](workflow-settings.md). Under den här tidsperioden sparas alla meddelanden, även efter att arbetsflödet har startats om. Om du inte vill spara meddelanden från en tidigare körning klickar du på knappen **[!UICONTROL Purge history]**.

![Exempel på arbetsflödesloggar och aktivitetsgränssnitt.](assets/workflow-logs.png){zoomable="yes"}

Det finns två typer av information:

* Fliken **[!UICONTROL Log]** innehåller körningshistoriken för alla arbetsflödesaktiviteter. Den indexerar de åtgärder som utförts och körningsfel i kronologisk ordning.
* Fliken **[!UICONTROL Tasks]** innehåller information om körningssekvensen för aktiviteterna.

På båda flikarna kan du välja vilka kolumner som ska visas och i vilken ordning de ska visas, tillämpa filter och använda sökfältet för att snabbt hitta önskad information.

## Kommandon för arbetsflödeskörning {#execution-commands}

Åtgärdsfältet i det övre högra hörnet innehåller kommandon för att hantera arbetsflödets körning. Du kan:

* **[!UICONTROL Start]** / **[!UICONTROL Resume]** körningen av arbetsflödet. Om arbetsflödet pausades återupptas det. Annars startar den och de inledande aktiviteterna aktiveras.
* **[!UICONTROL Pause]** arbetsflödets körning. Arbetsflödet får därefter statusen Pausad. Inga nya aktiviteter aktiveras förrän den återupptas, men pågående åtgärder avbryts inte.
* **[!UICONTROL Stop]** ett arbetsflöde som körs. Arbetsflödet får då statusen Slutförd. Pågående åtgärder avbryts om möjligt. Du kan inte återuppta arbetsflödet från den punkt där det stoppades.