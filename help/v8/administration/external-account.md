---
title: Hantera externt konto
description: Lär dig konfigurera externa konton
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 1%

---

# Kampanjspecifika externa konton {#external-account}

Följ stegen nedan för att konfigurera kontoinställningarna baserat på den typ av externt konto som du har valt.

## Studsa e-post (POP3) {#bounce}

Det externa kontot för studsmeddelanden anger det externa POP3-kontot som används för att ansluta till e-posttjänsten. Alla servrar som konfigurerats för POP3-åtkomst kan ta emot returmeddelanden.

![Skärmbild som visar konfigurationsfälten för det externa kontot, Bounce mails (POP3).](assets/external_account_bounce.png)

Om du vill konfigurera det externa kontot **[!UICONTROL Bounce mails (POP3)]** fyller du i följande fält:

* **[!UICONTROL Server]** - URL för POP3-servern.

* **[!UICONTROL Port]** - portnummer för POP3-anslutning (standardport är 110).

* **[!UICONTROL Account]** - Användarens namn.

* **[!UICONTROL Password]** - Lösenord för användarkonto.

* **[!UICONTROL Encryption]** - Typ av vald kryptering, inklusive:
   * Som standard (POP3 om port 110, POP3S om port 995).
   * POP3 som byter till SSL efter att ha skickat STARTTLS.
   * POP3 ej skyddad (port 110 som standard).
   * POP3-skyddad över SSL (port 995 som standard).

* **[!UICONTROL Function]** - Välj **[!UICONTROL Inbound email]** om du vill konfigurera kontot för att ta emot inkommande e-post eller **[!UICONTROL SOAP router]** om du vill hantera SOAP-begäranden.

>[!IMPORTANT]
>
>Innan du konfigurerar ditt POP3-externa konto med Microsoft OAuth 2.0 måste du först registrera programmet i Azure-portalen. Mer information finns på [den här sidan](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}.

Om du vill konfigurera en POP3-extern med Microsoft OAuth 2.0 markerar du alternativet Microsoft OAuth 2.0 och fyller i följande fält:

* **[!UICONTROL Azure Tenant]**

  Azure ID (eller klientorganisations-ID) finns i listrutan Grundläggande i programöversikten på Azure-portalen.

* **[!UICONTROL Azure Client ID]**

  Klient-ID (eller program-ID (klient)) finns i listrutan Grundläggande i programöversikten på Azure-portalen.

* **[!UICONTROL Azure Client Secret]**

  Klienthemligt ID finns i kolumnen Klienthemligheter på menyn Certifikat och hemligheter för ditt program i Azure-portalen.

* **[!UICONTROL Azure Redirect URL]**

  Omdirigerings-URL:en finns på autentiseringsmenyn för ditt program i Azure-portalen. Det ska sluta med följande syntax: nl/jsp/oauth.jsp, t.ex. `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

Internetåtkomst krävs för installation och för att använda knappen Testa anslutning i klientkonsolen. Efter installationen kan inMail-processen kommunicera med Microsoft-servrar utan Internet.

När du har angett de olika inloggningsuppgifterna kan du klicka på Konfigurera anslutningen för att slutföra konfigurationen av det externa kontot.

## Routning {#routing}

Följ stegen nedan för att konfigurera ett specifikt externt konto för externa leveranser.

1. Skapa ett externt konto. [Läs mer](create-external-account.md)

1. Välj typen **[!UICONTROL Routing]**.

   ![Skärmbild som visar val av extern kontotyp för routning.](assets/external-account-routing.png){zoomable="yes"}

1. Markera kanalen och klicka på **[!UICONTROL Create]**.

1. I avsnittet för det externa kontot **[!UICONTROL Details]** markeras **[!UICONTROL External]** som standard som **[!UICONTROL Delivery mode]**.

   ![Skärmbild som visar konfigurationen för leveransläge för routning av externa konton.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >För närvarande är **[!UICONTROL External]** det enda tillgängliga läget.

1. Om du vill hantera processen efter leveranskörningen kan du göra det externt till ett arbetsflöde för efterbearbetning. Skapa ett arbetsflöde med en [extern signal](../workflows/activities/external-signal.md)-aktivitet och välj den i fältet **[!UICONTROL Post-processing]**.

   ![Skärmbild som visar postbearbetningsfältets konfiguration för routning av externa konton.](assets/external-account-post-processing.png){zoomable="yes"}

1. I fältet **[!UICONTROL Activity]** redigerar du namnet på arbetsflödesaktiviteten för efterbearbetning som visas i loggarna. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Körningsinstans {#instance-exec}

Om du har en segmenterad arkitektur ska du identifiera de körningsinstanser som är associerade med kontrollinstansen och upprätta anslutningar mellan dem. Transaktionsmeddelandemallar distribueras på körningsinstansen.

![Skärmbild som visar konfigurationsfälten för det externa kontot i körningsinstansen.](assets/external_account_exec.png)

Så här konfigurerar du det externa kontot **[!UICONTROL Execution instance]**:

* **[!UICONTROL URL]** - URL för servern där körningsinstansen är installerad.

* **[!UICONTROL Account]** - Namnet på kontot, matchar Message Center Agent enligt operatormappen.

* **[!UICONTROL Password]** - Lösenord för kontot enligt definitionen i operatormappen.

* **[!UICONTROL Method]** - Välj mellan webbtjänsten eller FDA (Federated Data Access).

  Välj FDA-konto för FDA. Observera att Campaign-anslutningen till externa system är begränsad till avancerade användare och endast tillgänglig från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Create archiving workflow]** - För varje körningsinstans som är registrerad i meddelandecentret, oavsett om du har en eller flera instanser, skapar du ett separat arkiveringsarbetsflöde för varje externt konto som är associerat med körningsinstansen.
