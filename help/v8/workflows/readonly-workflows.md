---
audience: end-user
title: Om skrivskyddade arbetsflöden
description: Lär dig varför arbetsflöden är skrivskyddade
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Om skrivskyddade arbetsflöden {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Arbetsflödet är skrivskyddat"
>abstract="Du kan inte redigera det här arbetsflödet på grund av dina rättigheter eller arbetsflödets typ."

Vissa arbetsflöden kan vara skrivskyddade. Du kan se den med:

- The mention **[!UICONTROL ** Read-only **]** near the **[!UICONTROL Settings]** button
- Åtgärdsknapparna är inte tillgängliga

![](assets/readonly-workflow.png){zoomable="yes"}

Du kan inte redigera något i ett skrivskyddat arbetsflöde. Du får inte ändra inställningarna för aktiviteterna.


![](assets/scheduler-readonly.png){zoomable="yes"}


Du har inte heller behörighet att ta bort arbetsflödet.

![](assets/readonly-rights.png){zoomable="yes"}

## Varför skrivskyddade arbetsflöden

Skrivskyddat läge är avsett för användare som inte har behörighet och behörighet att redigera dessa arbetsflöden. [Läs mer här](../get-started/permissions.md)

En kampanjanvändare kan ha begränsningar i de data han har tillgång till i Adobe Campaign. Administratören kan ge honom möjligheten att se vissa funktioner men inte arbeta med dem.

## Typer av skrivskyddade arbetsflöden

Beroende på arbetsflödets typ kan skrivskyddat läge vara annorlunda.

### Kampanjarbetsflöden

Användaren kan inte komma åt övervakningsknappen om det finns ett skrivskyddat kampanjarbetsflöde.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Tekniska arbetsflöden

Tekniska arbetsflöden är skrivskyddade för kampanjanvändare.
Inbyggda tekniska arbetsflöden är skrivskyddade för alla, även för administratörer. Men användaren kan **pausa** eller **stoppa** vid behov. Det är de enda tillåtna åtgärderna. [Läs mer här](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}
