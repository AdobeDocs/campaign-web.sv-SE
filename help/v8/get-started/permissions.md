---
audience: end-user
title: Behörighetshantering i användargränssnittet för Campaign Web
description: Läs mer om behörigheter i användargränssnittet i Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Behörigheter {#permissions}

Varje användare i Adobe Campaign har sina egna behörigheter och begränsningar i programmet.

Användaren kan vara en del av operatorgruppen och ärver behörigheterna för gruppen.

Enligt dess behörigheter kan en operator:

* Tillgång till vissa funktioner
* Åtkomst till vissa data
* Åtkomst till vissa åtgärder (skapa, ändra, ta bort)

## Behörigheter för mappar {#folder-permissions}

Enligt dina rättigheter kan du visa och hantera behörigheter för mappar i **[!UICONTROL Folder settings]**.
Nedan finns ett exempel på en leveransmapp.

![](assets/folder_settings.png){zoomable="yes"}

I avsnittet **[!UICONTROL Security]** i **[!UICONTROL Folder settings]** kan du visa och hantera operatorer eller grupper som kan komma åt mappen.

![](assets/folder_security.png){zoomable="yes"}

Du kan klicka direkt på behörigheterna och ändra dem antingen **[!UICONTROL Allowed]** eller **[!UICONTROL Denied]**.

![](assets/folder_security_denied.png){zoomable="yes"}

Om alternativet **[!UICONTROL Propagate]** är aktiverat tillämpas alla behörigheter som definierats för en mapp på alla dess undermappar. Dessa behörigheter kan överladdas för varje undermapp.

Om alternativet **[!UICONTROL System folder]** är markerat tillåts åtkomst till alla operatorer, oavsett deras behörigheter.

Du kan också [hantera behörigheter för mappar i Adobe Campaign-konsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions).
Alla behörigheter i gränssnittet för Campaign-webben synkroniseras med behörigheterna för Campaign-klientkonsolen.
