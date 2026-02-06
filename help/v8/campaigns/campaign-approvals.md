---
audience: end-user
title: Konfigurera och hantera godkännandeprocessen
description: Lär dig hantera godkännanden av marknadsföringskampanjer på Campaign Web
feature: Approvals, Campaigns
exl-id: 8140f904-ec0a-44e1-981f-0e050d3c9cdb
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 1%

---

# Hantera godkännandeprocessen {#campaign-approvals}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn6"
>title="Hantering av kampanjgodkännande"
>abstract="Du kan nu koordinera validering av intressenter innan du skickar leveranser. Kräv godkännanden från marknadschefer, dataanalytiker eller andra team för kvalitetskontroll."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=sv-SE" text="Se versionsinformation"

>[!IMPORTANT]
>
>Godkännanden är bara tillgängliga för leveranser som skapats i en kampanj. Detta gäller inte fristående leveranser eller leveranser som skapats i arbetsflöden utanför ett kampanjsammanhang.

Godkännandeprocessen hjälper till att samordna flera intressenter och säkerställer kvalitetskontroll innan leveranser skickas. Använd godkännanden när organisationen kräver validering från olika team, till exempel marknadschefer som granskar innehåll eller dataanalytiker som validerar målgrupper.

När godkännanden är aktiverade måste du skicka in innehåll eller mål för godkännande. Utvalda granskare får e-postmeddelanden som begär validering och kan godkänna eller avvisa direkt från webbgränssnittet. Det går inte att skicka leveranser förrän alla nödvändiga godkännanden har beviljats. Du kan aktivera

* **Innehållsgodkännande**: validera meddelandeinnehåll, design och personalisering
* **Målgodkännande**: validera målgruppen och målinriktningskriterierna
* **Leveransbekräftelse**: en slutgiltig bekräftelse krävs innan du skickar

## Konfigurera godkännandeinställningar {#configure-approvals}

Godkännandeinställningarna ärvs från kampanjmallen och kan ändras för enskilda kampanjer. Följ de här stegen för att konfigurera inställningar för godkännande:

1. Öppna kampanj- eller kampanjmallen eller skapa en ny på menyn **[!UICONTROL Campaigns]**.

1. Klicka på knappen **[!UICONTROL Settings]** längst upp till höger på kampanjinstrumentpanelen.

1. Konfigurera följande alternativ i avsnittet **[!UICONTROL Approvals]**:

   ![Skärmbild som visar inställningarna för kampanjgodkännande](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Enable content approval]**: När det här alternativet är aktiverat måste leveransinnehållet godkännas innan det skickas. Klicka på mappikonen i fältet **[!UICONTROL Reviewer]** för att välja en operator eller operatorgrupp.

   * **[!UICONTROL Enable target approval]**: När det här alternativet är aktiverat måste målgruppen för leveransen godkännas. Klicka på mappikonen i fältet **[!UICONTROL Reviewer]** för att välja en operator eller operatorgrupp.

   * **[!UICONTROL Confirm the delivery before sending]**: en slutlig manuell bekräftelse krävs innan du skickar, även efter att alla andra godkännanden har slutförts.

>[!NOTE]
>
>* Om ingen granskare har angetts tilldelas kampanjägaren som granskare.
>* Granskarna behöver rätt behörigheter för att godkänna leveranser. Endast användare som identifieras i granskningslistan kan godkänna.

## Skicka för godkännande {#submit-approval}

När du har skapat leveransen följer du de här stegen för att skicka in innehåll och ange målet för godkännande.

>[!NOTE]
>Godkännanden är tillgängliga både för kampanjarbetsflöden och fristående kampanjleveranser.

1. Klicka på knappen **[!UICONTROL Submit content]** på kontrollpanelen för leverans. Utvalda granskare kan godkänna eller avvisa. Se [avsnittet](#approve-reject).

   ![Skärmbild som visar knappen Skicka innehåll](assets/approvals2.png){zoomable="yes"}

   Godkännandestatusen ändras till väntande i avsnittet **[!UICONTROL Properties]** på kontrollpanelen för leverans. Se [avsnittet](#rack-approvals).

1. När innehållet har godkänts klickar du på knappen **[!UICONTROL Prepare]** för att förbereda leveransmålet. Systemet förbereder målgrupps- och målinriktningskriterierna.

1. Klicka på knappen **[!UICONTROL Submit target]**. Utvalda granskare kan sedan godkänna eller avvisa. Se [avsnittet](#approve-reject).

   ![Skärmbild med målknappen Skicka](assets/approvals5.png){zoomable="yes"}

   Godkännandestatusen ändras till väntande. Se [avsnittet](#rack-approvals).

1. När målet har godkänts återupptas beredningen och leveransen kan skickas.

>[!NOTE]
>Om ett godkännande inte godkänns måste leveransägaren göra alla nödvändiga ändringar av innehållet eller målet baserat på granskarens kommentarer och skicka in det på nytt för godkännande.

## Godkänn eller avvisa {#approve-reject}

Utvalda granskare kan godkänna eller avvisa innehåll och målinskickat material. Se [avsnittet](#submit-approval).

>[!NOTE]
>För att e-postmeddelandet ska kunna skickas måste granskarens adress konfigureras i instansen.

1. När du får e-postmeddelandet öppnar du den leverans som kräver godkännande direkt från webbgränssnittet.

1. Granska innehållet eller målinformationen.

1. Klicka på knappen **[!UICONTROL Approve content]** eller **[!UICONTROL Approve target]**.

   ![Skärmbild som visar knappen Godkänn innehåll på kontrollpanelen för leverans](assets/approvals3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Approve]** eller **[!UICONTROL Reject]**.

1. Du kan också lägga till en **[!UICONTROL Comment]** som förklarar ditt beslut.

   ![Skärmbild som visar godkännandedialogrutan med knapparna Godkänn, Avvisa och Kommentar](assets/approvals4.png){zoomable="yes"}

1. Bekräfta ditt beslut. Godkännandestatusen uppdateras omedelbart på kontrollpanelen för leverans. Se [avsnittet](#rack-approvals).

## Spåra godkännandestatus {#track-approvals}

Godkännandestatus visas i avsnittet **[!UICONTROL Properties]** på kontrollpanelen för leverans. Statusen visar vilka godkännanden som väntar och deras aktuella status:

![Skärmbild med godkännandestatus](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL Being edited]**: innehållet eller målet har inte skickats för godkännande än
* **[!UICONTROL Pending approval]**: innehållet eller målet väntar på granskning
* **[!UICONTROL Approved]**: innehållet eller målet har godkänts av granskaren
* **[!UICONTROL Rejected]**: innehållet eller målet har avvisats av granskaren

Godkännandeavsnittet visar alla aktiverade godkännanden och uppdateringar i realtid när granskarna validerar eller avvisar varje steg.

## Relaterade ämnen {#related}

* [Skapa kampanjer](create-campaigns.md)
* [Hantera kampanjer](manage-campaigns.md)
