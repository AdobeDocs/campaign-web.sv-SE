---
audience: end-user
title: Skapa flerspråkiga e-postmeddelanden med Adobe Experience Manager
description: Lär dig hur du skapar flerspråkiga e-postleveranser med Adobe Experience Manager språkkopior på Campaign Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
exl-id: 6fc6ff43-ac7f-46c7-aa1a-9489ffc45423
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# Skapa flerspråkiga e-postmeddelanden med Adobe Experience Manager {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Manager live- och språkversioner"
>abstract="Nu kan du komma åt Adobe Experience Manager språk och live-kopior direkt i Campaign. Uppdatering av innehåll i realtid eliminerar manuell synkronisering för smidiga flerspråkiga arbetsflöden."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=sv-SE" text="Se versionsinformation"

Tack vare integreringen med Adobe Experience Manager kan du skapa flerspråkiga e-postleveranser med Adobe Experience Manager språkversioner. På så sätt kan ni hantera innehållsvarianter på olika språk och leverera personaliserade e-postmeddelanden baserat på mottagarnas språkinställningar.

## Förhandskrav {#prerequisites}

Innan du skapar en flerspråkig e-postleverans måste du se till att:

* Åtkomst till en Adobe Experience Manager-instans som konfigurerats för integrering av Adobe Campaign webbgränssnitt.
* Adobe Experience Manager-innehåll med språkversioner som redan skapats och godkänts. Läs mer om guiden för språkkopiering i [Adobe Experience Manager-dokumentationen](https://experienceleague.adobe.com/sv/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Mall för e-postleverans konfigurerad för att ta emot Adobe Experience Manager-innehåll. Se stegen som beskrivs i avsnittet [Aktivera flerspråkigt läge](#enable-multilingual).

## Skapa flerspråkig leverans

Om du vill skapa en flerspråkig e-postleverans måste du först aktivera det flerspråkiga alternativet i leveransinställningarna. Systemet identifierar automatiskt tillgängliga språkkopior och låter dig välja vilka som ska läggas till.

### Aktivera flerspråkigt läge {#enable-multilingual}

Skapa en ny leverans och aktivera alternativet för flera språk i de avancerade inställningarna.

1. Klicka på **[!UICONTROL Deliveries]** på menyn **[!UICONTROL Create delivery]**.

   ![](assets/lg-copy-1.png)

1. Välj mallen **[!UICONTROL Email delivery with AEM content]** och klicka på **[!UICONTROL Create delivery]**.

   ![](assets/lg-copy-2.png)

1. Ange en etikett för leveransen och konfigurera målgruppen. [Läs mer](../email/create-email.md)

1. Få åtkomst till leveransen **[!UICONTROL Settings]** och navigera sedan till avsnittet **[!UICONTROL Advanced]**.

1. Aktivera alternativet **[!UICONTROL Enable AEM multilingual]**.

   ![](assets/lg-copy-3.png)

1. Se till att:

   * **[!UICONTROL Content editing mode]** är inställt på **[!UICONTROL AEM]**.
   * Rätt Adobe Experience Manager **[!UICONTROL External account]** har valts.

1. Klicka på **[!UICONTROL Save and close]**.

### Skapa innehållsvarianter {#create-variants}

Välj ditt Adobe Experience Manager-innehåll och välj vilka språkvarianter som ska inkluderas i leveransen.

1. Klicka på **[!UICONTROL Edit content]**.

1. Välj **[!UICONTROL Create content variant]**.

   ![](assets/lg-copy-4.png)

1. Markera ditt Adobe Experience Manager-innehåll i listan.

   ![](assets/lg-copy-5.png)

1. Alla språkversioner som är associerade med det valda innehållet (överordnad-underordnad relation) identifieras, t.ex. om ditt Adobe Experience Manager-innehåll har varianter på franska, tyska och italienska, är alla varianter tillgängliga för val.

   Välj de språkvarianter som du vill ta med i leveransen.

   ![](assets/lg-copy-6.png)

1. Klicka på **[!UICONTROL Save]**.

1. Granska dina språkvarianter i innehållsredigeraren. Du kan nu [hantera varje variant individuellt](#manage-variants) eller fortsätta med att [skicka leveransen](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Hantera språkvarianter {#manage-variants}

När du har skapat innehållsvarianter kan du hantera dem direkt i leveransen:

1. Om du vill ange ett standardspråk öppnar du den avancerade menyn för den valda varianten och väljer **[!UICONTROL Set as default]**. Standardspråket används när en profils språkinställning inte har angetts eller inte matchar någon tillgänglig variant.

   Klicka på **[!UICONTROL Delete]** om du vill ta bort en variant från leveransen.

   ![](assets/lg-copy-8.png)

1. Klicka på **[!UICONTROL Manage locales]** på den avancerade menyn Innehållsvarianter för att lägga till andra språk i leveransen.

   ![](assets/lg-copy-9.png)

1. Välj ytterligare språkkopior om du vill ta med fler varianter och klicka på **[!UICONTROL Save]**.

   ![](assets/lg-copy-11.png)

1. Om innehåll uppdateras i Adobe Experience Manager klickar du på **[!UICONTROL Refresh AEM content]** för att synkronisera alla varianter med den senaste versionen.

   ![](assets/lg-copy-10.png)

1. Klicka på **[!UICONTROL Unlink AEM content]** om du vill redigera innehåll direkt i Campaign eller bryta länken med Adobe Experience Manager.

   >[!CAUTION]
   >
   >När du har brytt länken kan du inte uppdatera innehåll från Adobe Experience Manager eller skapa nya varianter. Innehållet blir självständigt från Adobe Experience Manager.
