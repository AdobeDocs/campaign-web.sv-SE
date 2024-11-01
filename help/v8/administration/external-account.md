---
title: Externt konto
description: Lär dig konfigurera externa konton
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# Konfigurera externa konton {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Externa konton"
>abstract="Du kan nu ansluta till ytterligare plattformar eller anpassa anslutningarna efter ditt arbetsflöde, och enkelt skapa nya externa konton som uppfyller dina specifika behov och säkerställa smidiga dataöverföringar."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"


>[!AVAILABILITY]
>
> Observera att externa konton för närvarande bara är tillgängliga för studsmeddelanden (POP3) och körningsinstansen, med ytterligare kontotyper som ska läggas till i framtiden.
> Externa konton som inte stöds och som skapats i Adobe Campaign-konsolen visas i webbanvändargränssnittet, men kan inte redigeras eller öppnas.

Adobe Campaign levereras med en uppsättning förkonfigurerade externa konton för enkel integrering med olika system. Om du behöver ansluta till fler plattformar eller anpassa anslutningarna efter ditt arbetsflöde kan du nu enkelt skapa nya externa konton med webbanvändargränssnittet för att uppfylla dina specifika behov och säkerställa smidiga dataöverföringar.

## Skapa ett externt konto {#create-ext-account}

Följ stegen nedan om du vill skapa ett nytt externt konto. Detaljerade inställningar beror på typen av externt konto.

1. Välj **[!UICONTROL External accounts]** under **[!UICONTROL Administration]** på den vänstra panelmenyn.

1. Klicka på **[!UICONTROL Create external account]**.

   ![](assets/external_account_create_1.png)

1. Ange din **[!UICONTROL Label]** och välj ditt externa konto **[!UICONTROL Type]**.

   ![](assets/external_account_create_2.png)

1. Klicka på **[!UICONTROL Create]**.

1. I listrutan **[!UICONTROL Advanced options]** kan du ändra sökvägen **[!UICONTROL Internal name]** eller **[!UICONTROL Folder]** om det behövs.

   ![](assets/external_account_create_3.png)

1. Aktivera **[!UICONTROL Exported automatically]** om du vill att data som hanteras av det här externa kontot automatiskt ska exporteras.

1. Konfigurera åtkomsten till kontot genom att ange autentiseringsuppgifter beroende på vald extern kontotyp.

1. Klicka på **[!UICONTROL Test the connection]** för att kontrollera att konfigurationen är korrekt

1. Duplicera eller ta bort ditt externa konto på menyn **[!UICONTROL More...]**.

   ![](assets/external_account_create_4.png)

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]**.

## Kampanjspecifika externa konton {#campaign-specific}

### Studsa e-post (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 stöds för närvarande inte.

Det externa kontot för studs-e-post anger det externa POP3-konto som används för att ansluta till e-posttjänsten. Alla servrar som konfigurerats för POP3-åtkomst kan ta emot returmeddelanden.

![](assets/external_account_bounce.png)

Så här konfigurerar du det externa kontot **[!UICONTROL Bounce mails (POP3)]**:

* **[!UICONTROL Server]**

  URL för POP3-servern

* **[!UICONTROL Port]**

  POP3-anslutningsportnummer (standardport är 110)

* **[!UICONTROL Account]**

  Användarens namn

* **[!UICONTROL Password]**

  Lösenord för användarkonto

* **[!UICONTROL Encryption]**

  Typ av vald kryptering mellan:

   * Som standard (POP3 om port 110, POP3S om port 995)
   * POP3 som byter till SSL efter att en STARTTLS har skickats
   * POP3 ej skyddad (port 110 som standard)
   * POP3 skyddad över SSL (port 995 som standard)

* **[!UICONTROL Function]**

  Inkommande e-post, när det externa kontot är konfigurerat att ta emot inkommande e-post, eller SOAP router, för att hantera SOAP.

### Körningsinstans{#instance-exec}

Om du har en segmenterad arkitektur måste du identifiera de körningsinstanser som är associerade med kontrollinstansen och skapa anslutningar mellan dem. Transaktionsmeddelandemallar distribueras på körningsinstansen.

![](assets/external_account_exec.png)

Så här konfigurerar du det externa kontot **[!UICONTROL Execution instance]**:

* **[!UICONTROL URL]**

  URL för servern där körningsinstansen är installerad.

* **[!UICONTROL Account]**

  Namnet på kontot måste matcha Message Center Agent enligt operatormappen.

* **[!UICONTROL Password]**

  Lösenord för kontot enligt definitionen i mappen operator.

* **[!UICONTROL Method]**

  Välj mellan webbtjänst eller FDA (Federated Data Access).
Om du har en FDA-metod väljer du ditt FDA-konto. Observera att Campaign-anslutningen till externa system är begränsad till avancerade användare och endast tillgänglig från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Create archiving workflow]**

  För varje körningsinstans som är registrerad i meddelandecentret, oavsett om du har en eller flera instanser, måste du skapa ett separat arkiveringsarbetsflöde för varje externt konto som är associerat med körningsinstansen.
