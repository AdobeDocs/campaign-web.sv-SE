---
audience: end-user
title: Arbeta med prenumerationstjänster
description: Lär dig hur du får tillgång till, skapar och hanterar prenumerationstjänster på Adobe Campaign Web
badge: label="Begränsad tillgänglighet"
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: d003de806a188b1b5c20a55ee1e308d5af1a19ea
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Skapa och hantera prenumerationstjänster {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Skapa och hantera tjänster"
>abstract="Använd Adobe Campaign för att skapa och övervaka tjänster som nyhetsbrev och för att kontrollera prenumerationer eller avbeställningar av dessa tjänster. Prenumerationer gäller endast för e-post och SMS-leverans."

Använd Adobe Campaign Web för att hantera och skapa t.ex. nyhetsbrev och för att kontrollera prenumerationer eller avbeställningar av dessa tjänster.

>[!NOTE]
>
>Prenumerationer gäller endast för e-post och SMS-leverans.

Flera tjänster kan definieras parallellt, till exempel: nyhetsbrev för specifika produktkategorier, teman eller områden på en webbplats, prenumerationer på olika typer av varningsmeddelanden och meddelanden i realtid.

Mer information om hur du hanterar prenumerationer och avbeställningar finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Få tillgång till prenumerationstjänster {#access-services}

Följ stegen nedan för att få tillgång till prenumerationstjänster som är tillgängliga för din plattform.

1. Gå till **[!UICONTROL Subscription services]** menyn i den vänstra navigeringslisten.

   ![](assets/service-list.png)

1. Listan över alla befintliga prenumerationstjänster visas. Du kan söka efter tjänster och filtrera på kanalen, mappen eller lägga till regler med hjälp av [frågemodellerare](../query/query-modeler-overview.md).

   ![](assets/service-filters.png)

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

Följ stegen nedan för att skapa en prenumerationstjänst.

1. Markera knappen **[!UICONTROL Create subscription service]**.

   ![](assets/service-create-button.png)

1. Välj en kanal: **[!UICONTROL Email]** eller **[!UICONTROL SMS]**.

1. Ange en etikett och definiera **[!UICONTROL Additional options]** som du vill.

   ![](assets/service-create-properties.png)

1. Som standard lagras tjänster i **[!UICONTROL Services and Subscriptions]** mapp. Du kan ändra den genom att bläddra till önskad plats. [Lär dig hur du arbetar med mappar](../get-started/permissions.md#folders)

1. Som standard är prenumerationerna obegränsade. Du kan inaktivera **[!UICONTROL Unlimited validity period]** för att definiera tjänstens giltighetsperiod.

   I exemplet nedan, efter 20 dagar:
   * Inga mottagare kommer att kunna prenumerera på tjänsten längre.
   * Alla prenumeranter på den här tjänsten kommer automatiskt att säga upp prenumerationen efter 20 dagar. [Läs mer](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. När en användare prenumererar på eller avbeställer en tjänst kan du skicka ett bekräftelsemeddelande. Välj de mallar som ska användas för det meddelandet utifrån ditt användningsfall. Dessa mallar måste konfigureras med **[!UICONTROL Subscriptions]** målmappning. [Läs mer](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. Klicka på **[!UICONTROL Save and review]**. Den nya tjänsten läggs till i **[!UICONTROL Subscription services]** lista.

Nu kan du:

* Lägg till prenumeranter i den här tjänsten och avbeställ prenumerationer. [Läs mer](../msg/send-to-subscribers.md)

* Skicka meddelanden till prenumeranterna på tjänsten. [Lär dig mer](../msg/send-to-subscribers.md)

## Skapa ett bekräftelsemeddelande {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Välj leveransmall för prenumerationer"
>abstract="Om du vill skicka bekräftelsemeddelanden till de användare som prenumererar på tjänsten måste du välja en specifik leveransmall baserad på **[!UICONTROL Subscriptions]** målmappning, utan ett definierat mål."


>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Välj leveransmall för avanmälan"
>abstract="Om du vill skicka bekräftelsemeddelanden till de användare som avbeställer tjänsten måste du välja en specifik leveransmall baserad på **[!UICONTROL Subscriptions]** målmappning, utan ett definierat mål."

Om du vill skicka bekräftelsemeddelanden till de användare som prenumererar på eller avbeställer tjänsten måste du skapa en leveransmall med **[!UICONTROL Subscriptions]** målmappning, utan ett definierat mål. Följ stegen nedan för att göra det.

1. Skapa en leveransmall för prenumerationsbekräftelsen. [Lär dig skapa en mall](../msg/delivery-template.md)

1. Välj ingen målgrupp för den här leveransen. I stället kommer du åt leveransen **[!UICONTROL Settings]**, går till [Målgrupp](../advanced-settings/delivery-settings.md#audience) och väljer **[!UICONTROL Subscriptions]** målmappning från listan.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >Om du inte markerar  **[!UICONTROL Subscriptions]** målmappning kommer dina prenumeranter inte att få något bekräftelsemeddelande. Målmappningar definieras i Campaign v8-konsolen. Läs mer i [Adobe Campaign v8-dokumentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

1. Redigera innehållet i leveransmallen, spara och stäng den.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >Läs mer om distributionskanaler och hur du definierar ett leveransinnehåll i [E-postkanal](../email/create-email.md) och [SMS-kanal](../sms/create-sms.md) -avsnitt.

1. Upprepa stegen ovan om du vill skapa en leveransmall för bekräftelsen av oprenumeration.

Nu kan du välja dessa meddelanden när [skapa en prenumerationstjänst](#create-service). Användare som prenumererar på eller avbeställer tjänsten får de valda bekräftelsemeddelandena.

## Övervaka dina prenumerationstjänster {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Totalt antal prenumeranter"
>abstract="Klicka **Beräkna** Hämta det totala antalet prenumeranter för den här tjänsten."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Antal prenumerationer för perioden"
>abstract="Använd listrutan för att ändra tidsintervallet och visa antalet prenumerationer och avbeställningar under den valda perioden."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Generell utveckling av prenumerationer"
>abstract="I det här diagrammet visas fördelningen per period, inklusive prenumerationer, icke-prenumerationer, utvecklingen av siffror och lojalitetsprocenten."

För att mäta hur effektiva era prenumerationstjänster är för SMS- och e-postkanaler har du tillgång till loggarna och rapporterna för en viss tjänst.

1. Välj en befintlig tjänst från **[!UICONTROL Subscription services]** lista. Klicka **[!UICONTROL Calculate]** Hämta det totala antalet prenumeranter.

   ![](assets/service-logs-subscribers-count.png)

1. På tjänstkontrollpanelen väljer du **[!UICONTROL Logs]** om du vill visa en lista över prenumeranter på tjänsten.

   Du kan kontrollera det totala antalet prenumeranter, namn och adress för varje mottagare och när de har prenumererat eller avbrutit prenumerationen. Du kan också filtrera på dem.

   ![](assets/service-logs.png)

1. På tjänstkontrollpanelen väljer du **[!UICONTROL Reports]**. Kontrollera följande indikatorer:

   * The **[!UICONTROL Total numbers of subscribers]** visas.

   * Du kan visa antalet prenumerationer och avbeställningar under en viss period. Använd listrutan för att ändra tidsintervallet.

     ![](assets/service-reports.png)

   * The **[!UICONTROL Overall evolution of subscriptions]** I diagrammet visas fördelningen per period, inklusive prenumerationer, icke-prenumerationer, utvecklingen i antal och lojalitetsprocenten.<!--what is Registered?-->

1. Använd **[!UICONTROL Reload]** för att hämta de senaste värdena från körningen och schemat för spårningsarbetsflödet.
