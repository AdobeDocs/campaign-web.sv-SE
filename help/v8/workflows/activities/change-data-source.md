---
audience: end-user
title: Använd arbetsflödesaktiviteten Ändra datakälla
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra datakälla
source-git-commit: f4919f9955e098630e596cf68e2b51088fde68dc
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# Ändra datakälla {#change-data-source}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Ändra datakälla i arbetsflöden"
>abstract="Med aktiviteten Ändra mål för datakälla kan du ändra datakällan som används i arbetsflödets arbetsregister. Den här aktiviteten ger större flexibilitet genom att du kan hantera data i olika databaser och förbättra prestandan."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="Se versionsinformation"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Ändra datakälla"
>abstract="The **Ändra datakälla** kan du välja en annan datakälla för arbetsflödets arbetstabell."

The **Ändra datakälla** aktiviteten är en **målinriktning** aktivitet. Med den här aktiviteten kan du ändra datakällan som används i arbetsflödets arbetsregister. Detta ger större flexibilitet genom att ni kan hantera data över olika databaser och förbättra prestandan.

I arbetsflöden lagras data som överförs från en aktivitet till en annan via övergångar i en temporär **Arbetsregister**. Arbetstabeller skapas som standard i samma databas som källan för de bearbetade data. När du till exempel hämtar tabellen &quot;Profiler&quot;, som finns i molndatabasen, skapas en arbetstabell i samma molndatabas.

I vissa fall är antingen data inte tillgängliga i den aktuella databasen eller så är de inte tillräckligt effektiva för att utföra enhetsåtgärder. Du kan därför behöva tvinga arbetsflödet att använda en annan databas för att utföra sådana åtgärder genom att lägga till en **[!UICONTROL Change data source]** aktivitet.

Detaljerad information om Campaign-arkitekturen finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Konfigurera aktiviteten Ändra datakälla {#configure}

Följ de här stegen för att konfigurera **Ändra dimension** aktivitet:

![](../assets/workflow-change-data-source-add.png)

1. Lägg till en **Ändra datakälla** till ditt arbetsflöde.

1. Definiera datakällan där du vill flytta arbetstabellen:

   * **[!UICONTROL Default Campaign database (PostgreSQL)]**: Använd standarddatabasen för Campaign.
   * **[!UICONTROL FDA external account]**: Använd externa Cloud-databaser som är anslutna till Adobe Campaign via Federated Data Access-funktioner.

     >[!AVAILABILITY]
     >
     >Kampanjkonfiguration och anslutning till externa system är begränsade till avancerade användare och är endast tillgängliga från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

1. Konfigurera arbetsflödet för att utföra önskade åtgärder med den nya datakällan.

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
