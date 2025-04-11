---
audience: end-user
title: Om skrivskyddade arbetsflöden
description: Lär dig varför arbetsflöden är skrivskyddade
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Om skrivskyddade arbetsflöden {#readonly-workflows}

>[!CONTEXTUALHELP]
>
Vissa arbetsflöden är skrivskyddade. Inbyggda tekniska arbetsflöden är alltid skrivskyddade, men den här begränsningen kan även gälla för andra typer av arbetsflöden.

Kampanjanvändare kan ha begränsad åtkomst till Adobe Campaign-data. En kampanjadministratör kan ge dem behörighet att visa vissa funktioner, men inte att redigera eller ändra dem. Användarbehörigheter för data är nödvändiga för att säkerställa data- och processsäkerhet. Läs mer om behörighetshantering i Campaign i [det här avsnittet](../get-started/permissions.md).

När ett arbetsflöde är skrivskyddat:

* Omnämnandet **[!UICONTROL Read-only]** visas nära knappen **[!UICONTROL Settings]**.
* Åtgärdsknapparna är inte tillgängliga.

![Skrivskyddat arbetsflödesgränssnitt med inställningsknappen och inaktiverade åtgärdsknappar.](assets/readonly-workflow.png){zoomable="yes"}

Användare kan inte redigera något i ett skrivskyddat arbetsflöde. De får inte ändra inställningarna för aktiviteterna.

![Gränssnittet Schemaläggaren i skrivskyddat läge visar inaktiverade inställningsalternativ.](assets/scheduler-readonly.png){zoomable="yes"}

Användare kan inte ta bort arbetsflödet.

![Gränssnitt med begränsade rättigheter för borttagning av arbetsflöden.](assets/readonly-rights.png){zoomable="yes"}

## Typer av skrivskyddade arbetsflöden {#readonly-workflow-types}

Beroende på arbetsflödets typ kan skrivskyddat läge variera.

### Kampanjarbetsflöden {#readonly-campaign-wf}

I ett skrivskyddat kampanjarbetsflöde kan användaren inte komma åt övervakningsknappen.

![Gränssnittet för kampanjarbetsflöde i skrivskyddat läge, med inaktiverade övervakningsalternativ.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Tekniska arbetsflöden {#readonly-tech-wf}

Inbyggda tekniska arbetsflöden är skrivskyddade för alla Campaign-användare, inklusive administratörer. Användarna kan dock **pausa** eller **stoppa** dem vid behov. Detta är de enda tillåtna åtgärderna.

![Tekniskt arbetsflödesgränssnitt i skrivskyddat läge, med alternativ för att pausa eller stoppa arbetsflöden.](assets/readonly-technical-workflow.png){zoomable="yes"}

Läs mer om tekniska arbetsflöden i [det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).