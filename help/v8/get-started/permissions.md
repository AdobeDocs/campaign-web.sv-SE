---
audience: end-user
title: Behörighetshantering i användargränssnittet för Campaign Web
description: Läs mer om behörigheter i användargränssnittet i Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f352f4e726eff50527d0b9a04d0506600c12b822
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Behörigheter {#permissions}

Varje användare i Adobe Campaign har sina egna behörigheter och begränsningar i programmet. Användaren kan vara en del av operatorgruppen och ärver behörigheterna för gruppen.

Enligt dess behörigheter kan en operator:

* Tillgång till vissa funktioner
* Åtkomst till vissa data
* Åtkomst till vissa åtgärder (skapa, ändra, ta bort)

Detaljerade procedurer för att konfigurera behörigheter i Adobe Campaign finns i [Adobe Campaign v8-dokumentationen (konsolen)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Behörigheter för mappar {#folder-permissions}

Enligt dina rättigheter kan du visa och hantera behörigheter för mappar i **[!UICONTROL Folder settings]**.

Nedan visas ett exempel på en leveransmapp:

![](assets/folder_settings.png){zoomable="yes"}

I avsnittet **[!UICONTROL Security]** i **[!UICONTROL Folder settings]** kan du visa och hantera operatorer eller grupper som kan komma åt mappen.

![](assets/folder_security.png){zoomable="yes"}

Du kan klicka direkt på behörigheterna och ändra dem antingen **[!UICONTROL Allowed]** eller **[!UICONTROL Denied]**.

![](assets/folder_security_denied.png){zoomable="yes"}

Om alternativet **[!UICONTROL Propagate]** är aktiverat tillämpas alla behörigheter som definierats för en mapp på alla dess undermappar. Dessa behörigheter kan överladdas för varje undermapp.

Om alternativet **[!UICONTROL System folder]** är markerat tillåts åtkomst till alla operatorer, oavsett deras behörigheter.

Du kan också [hantera behörigheter för mappar i Adobe Campaign-konsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Alla behörigheter i gränssnittet för Campaign-webben synkroniseras med behörigheterna för Campaign-klientkonsolen.
