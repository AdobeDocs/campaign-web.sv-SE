---
audience: end-user
title: Arbeta med prenumerationstjänster
description: Lär dig hur du skapar och hanterar tjänster på Adobe Campaign Web
badge: label="Beta"
source-git-commit: 307d1e65850fcbdb51ca0016e4f3f30ca74997be
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 1%

---


# Arbeta med prenumerationstjänster {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Skapa och hantera tjänster"
>abstract="Använd Adobe Campaign för att skapa och övervaka tjänster som nyhetsbrev och för att kontrollera prenumerationer/avbeställningar av dessa tjänster. Prenumerationer gäller endast för e-post och SMS-leverans."

Använd Adobe Campaign webben för att hantera och skapa t.ex. nyhetsbrev och för att kontrollera prenumerationer/avbeställningar av dessa tjänster.

>[!NOTE]
>
>Prenumerationer gäller endast för e-post och SMS-leverans.

Flera tjänster kan definieras parallellt, till exempel: nyhetsbrev för specifika produktkategorier, teman eller områden på en webbplats, prenumerationer på olika typer av varningsmeddelanden och meddelanden i realtid.

Mer information om hur du hanterar prenumerationer och avbeställningar finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Åtkomst till prenumerationstjänster {#access-services}

Om du vill få tillgång till prenumerationstjänster för din plattform går du till **[!UICONTROL Subscription services]** menyn i den vänstra navigeringslisten.

![](assets/service-list.png)

Listan över alla befintliga prenumerationstjänster visas. Du kan söka efter tjänster och filtrera på kanalen, mappen eller använda avancerade filter.

![](assets/service-filters.png)

Om du vill redigera en befintlig tjänst klickar du på dess namn.

## Skapa din första prenumerationstjänst {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Definiera dina serviceegenskaper"
>abstract="Ange prenumerationstjänstens etikett och definiera ytterligare alternativ, t.ex. en giltighetsperiod för tjänsten."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Välj ett bekräftelsemeddelande"
>abstract="När en användare prenumererar på eller avbeställer en tjänst kan du skicka ett bekräftelsemeddelande. Välj de mallar som ska användas för det meddelandet."

Så här skapar du en prenumerationstjänst:

1. Markera knappen **[!UICONTROL Create subscription service]**.

   ![](assets/service-create-button.png)

1. Välj en kanal: **[!UICONTROL Email]** eller **[!UICONTROL SMS]**.

1. Ange en etikett och definiera ytterligare alternativ i tjänsteegenskaperna.

   ![](assets/service-create-properties.png)

1. Som standard är prenumerationerna obegränsade. Du kan inaktivera **[!UICONTROL  Unlimited validity period]** för att definiera tjänstens giltighetsperiod. <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. När en användare prenumererar på eller avbeställer en tjänst kan du skicka ett bekräftelsemeddelande. Välj de mallar som ska användas för det meddelandet utifrån ditt användningsfall.

   ![](assets/service-create-confirmation-msg.png)

1. Klicka på **[!UICONTROL Save]**. Den nya tjänsten läggs till i **[!UICONTROL Subscription services]** lista.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


