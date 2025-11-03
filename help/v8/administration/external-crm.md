---
title: Hantera externt konto
description: Lär dig hur du konfigurerar externa CRM-konton
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

# Externt CRM-konto {#external-crm}

Använd ett externt CRM-konto för att ansluta Adobe Campaign till en tredjepartsdatabas.

Konfigurationsinställningarna för det här externa kontot beror på vilken databasmotor du ansluter till. Detaljerade installationsanvisningar för varje databas som stöds finns i avsnitten nedan.

## MICROSOFT DYNAMICS CRM

Med det externa Microsoft Dynamics CRM-kontot kan du ansluta Campaign-instansen till den externa Microsoft Dynamics CRM-databasen.

Konfigurera ditt externa Microsoft Dynamics CRM-konto i Adobe Campaign Web User Interface.

1. [Skapa ditt externa konto](external-account.md) och välj **[!UICONTROL External database]** som **[!UICONTROL Type]** och Microsoft Dynamics CRM som **[!UICONTROL Provider type]** för ditt externa konto.

1. Klicka på **[!UICONTROL Create]**.

1. Om du vill konfigurera det externa kontot **[!UICONTROL Microsoft Dynamics CRM]** fyller du i följande fält:

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Microsoft Dynamics CRM.](assets/crm-microsoft-1.png)

   +++ För CRM OAuth-typ: Lösenordsreferenser

   * **[!UICONTROL Server]**: Ange URL-adressen till din Microsoft CRM-server.

     Logga in på ditt Microsoft Dynamics CRM-konto, välj Dynamics 365 och öppna sedan din app för att hitta din Microsoft CRM Server-URL. Serverns URL visas i webbläsarens adressfält, till exempel:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Account]**: Ange vilket konto som ska användas för att logga in på Microsoft CRM.

   * **[!UICONTROL Password]**: Ange lösenordet som är kopplat till det angivna kontot.

   * **[!UICONTROL Client identifier]**: Ange klient-ID:t som finns i Microsoft Azure-hanteringsportalen.

   * **[!UICONTROL CRM version]**: Välj Dynamics CRM 365 CRM-version.

   +++

   </br>

   +++ För CRM O-Auth-typ: Certifikat

   * **[!UICONTROL Server]**: Ange URL-adressen till din Microsoft CRM-server.

     Logga in på ditt Microsoft Dynamics CRM-konto, välj Dynamics 365 och öppna sedan din app för att hitta din Microsoft CRM Server-URL. Serverns URL visas i webbläsarens adressfält, till exempel:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Private Key(Base64 encoded)]**: Ange den privata nyckeln som är kodad i Base64-format.

     Det gör du genom att använda en Base64-kodare eller kommandoraden `base64 -w0 private.key` för Linux.

   * **[!UICONTROL Custom Key identifier]**: Ange den anpassade nyckel-ID som används för certifikatet.

   * **[!UICONTROL Key ID]**: Ange det nyckel-ID som är associerat med ditt certifikat.

   * **[!UICONTROL Client identifier]**: Ange klient-ID:t som finns i Microsoft Azure Management

   * **[!UICONTROL CRM version]**: Välj Dynamics CRM 365 CRM-version.

   +++

1. När du har konfigurerat anslutningen kan du få åtkomst till **[!UICONTROL Microsoft CRM configuration wizard]** för att skapa din Microsoft CRM-tabelllista.

   Klicka på **[!UICONTROL Next]** för att markera de tabeller som krävs.

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Microsoft Dynamics CRM.](assets/crm-microsoft-2.png)

1. Markera de Microsoft CRM-tabeller som ska hämtas, eller lägg till en fjärrtabell genom att ange **[!UICONTROL Table label]** och **[!UICONTROL Table internal name]**, och aktivera sedan växlingsknappen **[!UICONTROL Selected]**.

   Klicka på **[!UICONTROL Next]**.

1. Klicka på **[!UICONTROL Start]** för att börja skapa Microsoft CRM-schemat baserat på de markerade tabellerna.

1. Följ instruktionerna på skärmen för att infoga sidor från Adobe Campaign marknadsföringshistorik och prenumerationshantering direkt i Microsoft Dynamics CRM.

1. Klicka på **[!UICONTROL Display marketing history URLs]** om du vill visa URL:er för integrering av sidor för marknadsföringshistorik eller **[!UICONTROL Display URLs for lead subscriptions]** om du vill visa URL:er för integrering av sidor för prenumerationshantering.

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Microsoft Dynamics CRM.](assets/crm-microsoft-3.png)

1. Klicka på **[!UICONTROL Save]** när ditt externa Microsoft CRM-konto har konfigurerats.

1. När ditt externa konto har skapats kan du nu klicka på **[!UICONTROL Synchronizing enumerations...]** för att synkronisera uppräkningar automatiskt från Microsoft CRM till Adobe Campaign webbanvändargränssnitt.

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Microsoft CRM.](assets/crm-microsoft-4.png)

1. Välj den Adobe Campaign-uppräkning som matchar uppräkningen i Microsoft CRM.

   Aktivera alternativet **[!UICONTROL Replace]** om du vill ersätta Adobe Campaign-värden med Microsoft CRM-värden.

## Salesforce {#salesforce}

Om du vill konfigurera Salesforce externa konto så att det fungerar med Adobe Campaign måste du ange följande information:

1. [Skapa ett externt konto](external-account.md) och välj **[!UICONTROL External database]** som **[!UICONTROL Type]** och Salesforce.com som **[!UICONTROL Provider type]** för ditt externa konto.

   ![Skärmbild som visar konfigurationsfälten för Salesforce externa konton.](assets/crm-salesforce-1.png)

1. Klicka på **[!UICONTROL Create]**.

1. Om du vill konfigurera det externa kontot **[!UICONTROL Salesforce]** fyller du i följande fält:

   * **[!UICONTROL CRM O-Auth type]**: **[!UICONTROL Password credentials]** eller **[!UICONTROL Credentials]**

   * **[!UICONTROL Account]**: Det konto som används för att logga in på Salesforce CRM.

   * **[!UICONTROL Password]**: Ange lösenordet som är kopplat till det angivna kontot.

   * **[!UICONTROL Security token]**: Ange den Salesforce-säkerhetstoken som är associerad med kontot.

   * **[!UICONTROL API version]**: Välj version 49.

   ![Skärmbild som visar konfigurationsfälten för Salesforce externa konton.](assets/crm-salesforce-2.png)

1. Öppna **[!UICONTROL Salesforce CRM configuration wizard]** för att generera din Salesforce CRM-tabelllista och klicka sedan på **[!UICONTROL Next]**.

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Salesforce CRM.](assets/crm-salesforce-3.png)

1. Markera de Salesforce-tabeller som ska hämtas, eller lägg till en fjärrtabell genom att ange **[!UICONTROL Table label]** och **[!UICONTROL Table internal name]** och aktivera sedan växlingsknappen **[!UICONTROL Selected]**.

   Klicka på **[!UICONTROL Next]**.

1. Klicka på **[!UICONTROL Start]** för att börja skapa Salesforce CRM-schemat baserat på de markerade tabellerna.

1. Klicka på **[!UICONTROL Salesforce link creation wizard...]** om du vill generera webblänkarna i Salesforce.

   Klicka sedan på **[!UICONTROL Next]** för att hämta webblänkarna för **Leads** och **Kontakter** från Salesforce.

1. Markera länkarna som ska exporteras till Salesforce webblänkslista.

1. Följ instruktionerna på skärmen för att infoga sidor om **marknadsföringshistorik** och **prenumerationshantering** från Adobe Campaign webbanvändargränssnitt i Salesforce CRM.

1. Klicka på **[!UICONTROL Save]** när ditt externa Salesforce CRM-konto har konfigurerats.

1. När ditt externa konto har skapats kan du nu klicka på **[!UICONTROL Synchronizing enumerations...]** för att synkronisera uppräkningar automatiskt från Salesforce till Adobe Campaign webbanvändargränssnitt.

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Salesforce CRM.](assets/crm-salesforce-4.png)

1. Välj den Adobe Campaign-uppräkning som överensstämmer med uppräkningen i Salesforce.

   Aktivera alternativet **[!UICONTROL Replace]** om du vill ersätta Adobe Campaign-värden med Salesforce-värden.

   ![Skärmbild som visar konfigurationsfälten för det externa kontot i Salesforce CRM.](assets/crm-salesforce-5.png)

