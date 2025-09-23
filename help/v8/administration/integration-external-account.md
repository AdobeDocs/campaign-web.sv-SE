---
title: Hantera externt konto
description: Lär dig konfigurera externa konton
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Externa konton för Adobe Solution Integration {#integration-external-account}

Beroende på vilken typ av externt Adobe Solution Integration-konto du har valt följer du stegen nedan för att konfigurera anslutnings- och kontoinställningarna för smidig integrering med Adobe-tjänster.

## Adobe Experience Cloud

Om du vill ansluta till Adobe Campaign-konsolen med en Adobe ID måste du konfigurera det externa Adobe Experience Cloud-kontot (MAC).

![Skärmbild som visar konfigurationsfälten för det externa kontot i Adobe Experience Cloud MAC.](assets/external-MAC.png)

Om du vill konfigurera det externa kontot **[!UICONTROL Adobe Experience Cloud]** fyller du i följande fält:

* **[!UICONTROL IMS server]**

  URL för IMS-servern. Se till att både fas- och produktionsinstanser pekar på samma IMS-produktionsslutpunkt.

* **[!UICONTROL IMS scope]**

  Omfattningar som definieras här måste vara en delmängd av de som tillhandahålls av IMS.

* **[!UICONTROL IMS client identifier]**

  ID för IMS-klienten.

* **[!UICONTROL IMS client secret]**

  Autentiseringsuppgifter för din IMS-klienthemlighet.

* **[!UICONTROL Callback server]**

  Åtkomst-URL för din Adobe Campaign-instans.

* **[!UICONTROL IMS organization ID]**

  ID för din organisation. Information om hur du hittar ditt organisations-ID finns på [den här sidan](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=sv){target=_blank}.

* **[!UICONTROL Association mask]**

  Syntax som gör att konfigurationsnamn i Enterprise Dashboard kan synkroniseras med grupper i Adobe Campaign.

* **[!UICONTROL Server]**

  URL för din Adobe Experience Cloud-instans.

* **[!UICONTROL Tenant]**

  Namn på din Adobe Experience Cloud-klient.
