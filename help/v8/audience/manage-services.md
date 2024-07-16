---
audience: end-user
title: Arbeta med prenumerationstjänster
description: Lär dig hur du får tillgång till, skapar och hanterar prenumerationstjänster på Adobe Campaign Web
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: 943ed7ce9245a3fd0fd7111f285fdf409968c78b
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 1%

---

# Skapa och hantera prenumerationstjänster {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Skapa och hantera tjänster"
>abstract="Använd Adobe Campaign för att skapa och övervaka tjänster som nyhetsbrev och för att kontrollera prenumerationer eller avbeställningar av dessa tjänster. Prenumerationer gäller endast för e-post och SMS-leverans."

Använd Adobe Campaign Web för att hantera och skapa t.ex. nyhetsbrev och för att kontrollera prenumerationer eller avbeställningar av dessa tjänster.

Flera tjänster kan definieras parallellt, till exempel: nyhetsbrev för specifika produktkategorier, teman eller områden på en webbplats, prenumerationer på olika typer av varningsmeddelanden och meddelanden i realtid.

>[!NOTE]
>
>Prenumerationer gäller endast för e-post och SMS-leverans.

## Få tillgång till prenumerationstjänster {#access-services}

Följ stegen nedan för att få tillgång till prenumerationstjänster som är tillgängliga för din plattform.

1. Bläddra till menyn **[!UICONTROL Subscription services]** i den vänstra navigeringslisten.

   ![](assets/service-list.png){zoomable="yes"}

1. Listan över alla befintliga prenumerationstjänster visas. Du kan söka efter tjänster och filtrera på kanalen, mappen eller lägga till regler med [frågemodelleraren](../query/query-modeler-overview.md).

   ![](assets/service-filters.png){zoomable="yes"}

1. Om du vill redigera en befintlig tjänst klickar du på dess namn.

1. Du kan ta bort eller duplicera en tjänst med hjälp av ikonen med tre punkter bredvid tjänstnamnet.<!--so all subscribers are unsubscribed - need to mention?-->

## Skapa din första prenumerationstjänst {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Definiera tjänstegenskaperna"
>abstract="Ange prenumerationstjänstens etikett och definiera ytterligare alternativ, t.ex. en giltighetsperiod för tjänsten."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Välj ett bekräftelsemeddelande"
>abstract="När en användare prenumererar på eller avbeställer en tjänst kan du skicka ett bekräftelsemeddelande. Välj de mallar som ska användas för det meddelandet."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Standardstartsida"
>abstract="Välj de standardlandningssidor som är associerade med den här tjänsten."

Följ stegen nedan för att skapa en prenumerationstjänst.

1. Markera knappen **[!UICONTROL Create subscription service]**.

   ![](assets/service-create-button.png){zoomable="yes"}

1. Välj en kanal: **[!UICONTROL Email]** eller **[!UICONTROL SMS]**.

1. Ange en etikett i tjänsteegenskaperna och definiera **[!UICONTROL Additional options]** efter behov.

   ![](assets/service-create-properties.png){zoomable="yes"}

1. Som standard lagras tjänster i mappen **[!UICONTROL Services and Subscriptions]**. Du kan ändra den genom att bläddra till önskad plats. [Lär dig arbeta med mappar](../get-started/permissions.md#folders)

1. Som standard är prenumerationerna obegränsade.

   Du kan inaktivera alternativet **[!UICONTROL Unlimited validity period]** för att definiera en giltighetslängd för tjänsten. När giltighetsperioden är slut:
   * Ingen profil kan längre prenumerera på tjänsten
   * Alla prenumeranter på tjänsten avbryts automatiskt

   ![](assets/service-create-validity-period.png){zoomable="yes"}

1. När en användare prenumererar på eller avbeställer en tjänst kan du skicka ett bekräftelsemeddelande. Välj de mallar som ska användas för det meddelandet utifrån ditt användningsfall. Dessa mallar måste konfigureras med målmappningen **[!UICONTROL Subscriptions]**. [Läs mer](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Save and review]**. Den nya tjänsten läggs till i listan **[!UICONTROL Subscription services]**.

1. Du kan också välja standardstartsidor för prenumeration och avprenumeration som är kopplade till den här tjänsten.

   >[!AVAILABILITY]
   >
   >Den här funktionen är begränsad tillgänglighet (LA). Den är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

   ![](assets/service-create-default-lp.png){zoomable="yes"}

   När du är klar väljer du **[!UICONTROL Subscription link]** eller **[!UICONTROL Unsubscription link]** när du [infogar en länk](../email/message-tracking.md) i ett e-postmeddelande. När du klickar på länken dirigeras användarna till den prenumerations- eller avprenumerationssida som tjänsten hänvisar till. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

   ![](assets/service-create-default-lp-link.png){zoomable="yes"}

1. Spara och granska ändringarna.

Nu kan du:

* Lägg till prenumeranter manuellt i den här tjänsten och avbeställ profiler. [Läs mer](../audience/manage-subscribers.md)

* Bjud in kunderna att prenumerera på den här tjänsten via en landningssida. [Läs mer](../landing-pages/lp-use-cases.md#lp-subscription)

* Skicka meddelanden till prenumeranterna på tjänsten. [Lär dig hur](../msg/send-to-subscribers.md)

## Skapa ett bekräftelsemeddelande {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Välj leveransmall för prenumerationer"
>abstract="Om du vill skicka bekräftelsemeddelanden till de användare som prenumererar på tjänsten måste du välja en specifik leveransmall baserad på målmappningen **[!UICONTROL Subscriptions]**, utan något definierat mål."


>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Välj leveransmall för avanmälan"
>abstract="Om du vill skicka bekräftelsemeddelanden till de användare som avbeställer tjänsten måste du välja en specifik leveransmall baserad på målmappningen **[!UICONTROL Subscriptions]**, utan något definierat mål."

Om du vill skicka bekräftelsemeddelanden till de användare som prenumererar på eller avslutar prenumerationen på tjänsten måste du skapa en leveransmall med målmappningen **[!UICONTROL Subscriptions]**, utan något definierat mål. För att göra detta, följ nedanstående steg:

1. Skapa en leveransmall för prenumerationsbekräftelsen. [Lär dig skapa en mall](../msg/delivery-template.md)

1. Välj ingen målgrupp för den här leveransen. Öppna i stället leveransen **[!UICONTROL Settings]**, gå till fliken [Målgrupp](../advanced-settings/delivery-settings.md#audience) och välj målmappningen **[!UICONTROL Subscriptions]** i listan.

   ![](assets/service-confirmation-template-mapping.png){zoomable="yes"}

   >[!NOTE]
   >
   >Om du inte väljer målmappningen **[!UICONTROL Subscriptions]** får prenumeranterna inte något bekräftelsemeddelande. Läs mer om målmappningar i [det här avsnittet](../audience/targeting-dimensions.md).

1. Redigera innehållet i leveransmallen, spara och stäng den.

   ![](assets/service-confirmation-template.png){zoomable="yes"}

   >[!NOTE]
   >
   >Läs mer om leveranskanaler och hur du definierar ett leveransinnehåll i avsnitten [E-postkanal](../email/create-email.md) och [SMS-kanal](../sms/create-sms.md).

1. Upprepa stegen ovan om du vill skapa en leveransmall för bekräftelsen av oprenumeration.

Du kan nu välja dessa meddelanden när du [skapar en prenumerationstjänst](#create-service). Användare som prenumererar på eller avbeställer tjänsten får de valda bekräftelsemeddelandena.

## Övervaka dina prenumerationstjänster {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Antal prenumeranter"
>abstract="Klicka på **Beräkna** om du vill hämta det totala antalet prenumeranter för den här tjänsten."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="Totalt antal prenumeranter"
>abstract="KPI (Key Performance Indicator) ger en heltäckande bild av prenumerationsbasen och visar det totala antalet personer som har prenumererat på den här tjänsten."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Antal prenumerationer för perioden"
>abstract="Använd listrutan för att ändra tidsintervallet och visa antalet prenumerationer och avbeställningar under den valda perioden."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Generell utveckling av prenumerationer"
>abstract="I det här diagrammet visas fördelningen per period, inklusive prenumerationer, icke-prenumerationer, utvecklingen av siffror och lojalitetsprocenten."

För att mäta hur effektiva era prenumerationstjänster är för SMS- och e-postkanaler har du tillgång till loggarna och rapporterna för en viss tjänst.

1. Välj en befintlig tjänst i listan **[!UICONTROL Subscription services]**. Klicka på **[!UICONTROL Calculate]** för att hämta det totala antalet prenumeranter.

   ![](assets/service-logs-subscribers-count.png){zoomable="yes"}

1. Välj **[!UICONTROL Logs]** på tjänstinstrumentpanelen för att visa listan över prenumeranter på den här tjänsten.

   Du kan kontrollera det totala antalet prenumeranter, namn och adress för varje mottagare och när de har prenumererat eller avbrutit prenumerationen. Du kan också filtrera på dem.

   ![](assets/service-logs.png){zoomable="yes"}

1. Välj **[!UICONTROL Reports]** på tjänstinstrumentpanelen. Kontrollera följande indikatorer:

   * **[!UICONTROL Total numbers of subscribers]** visas.

   * Du kan visa antalet prenumerationer och avbeställningar under en viss period. Använd listrutan för att ändra tidsintervallet.

     ![](assets/service-reports.png){zoomable="yes"}

   * Diagrammet **[!UICONTROL Overall evolution of subscriptions]** visar fördelningen per period, inklusive prenumerationer, icke-prenumerationer, nummerutvecklingen och lojalitetsprocenten.<!--what is Registered?-->

1. Använd knappen **[!UICONTROL Reload]** för att hämta de senaste värdena från körningen och schemat för spårningsarbetsflödet.

<!--## Best practices {#best-practices}

It is recommended to send a confirmation message to the new subscribers of a service. To do so, create a delivery template and select it when creating a subscription service. [Learn more](#create-confirmation-message).

Send communications targeting your subscribers only. [Learn how](../msg/send-to-subscribers.md)

Always provide your subscribers the capability to unsubscribe from your services. [Learn how](consent.md#email-opt-out)

* When creating a confirmation message:

    * Do not select an audience for this delivery.

    * Select the **[!UICONTROL Subscriptions]** target mapping. Otherwise, your subscribers will not receive the confirmation message.
-->