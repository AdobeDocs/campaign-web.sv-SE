---
audience: end-user
title: Använd arbetsflödesaktiviteten Ändra datakälla
description: Lär dig hur du använder arbetsflödesaktiviteten Ändra datakälla
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 2%

---

# Ändra datakälla {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Ändra datakälla"
>abstract="Med aktiviteten **Ändra datakälla** kan du välja en annan datakälla för arbetsflödets arbetstabell."

Aktiviteten **Ändra datakälla** är en **målaktivitet**. Med den här aktiviteten kan du ändra datakällan som används i arbetsflödets arbetsregister. Detta ger större flexibilitet genom att ni kan hantera data över olika databaser och förbättra prestandan.

I arbetsflöden lagras data som transporteras från en aktivitet till en annan via övergångar i en tillfällig **arbetstabell**. Arbetstabeller skapas som standard i samma databas som källan för de bearbetade data. När du till exempel hämtar tabellen &quot;Profiler&quot;, som finns i molndatabasen, skapas en arbetstabell i samma molndatabas.

I vissa fall är antingen data inte tillgängliga i den aktuella databasen eller så är de inte tillräckligt effektiva för att utföra enhetsåtgärder. Du kan därför behöva tvinga arbetsflödet att använda en annan databas för att utföra sådana åtgärder genom att lägga till en **[!UICONTROL Change data source]**-aktivitet.

Detaljerad information om Campaign-arkitekturen finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html).

>[!IMPORTANT]
>
>Observera att aktiviteterna **[!UICONTROL Change Dimension]** och **[!UICONTROL Change Data source]** inte ska läggas till på en rad. Om du behöver använda båda aktiviteterna i följd inkluderar du en **[!UICONTROL Enrichment]**-aktivitet mellan dem. Detta garanterar att programmet körs på rätt sätt och förhindrar eventuella konflikter och fel.

>[!NOTE]
>
>**Source**-aktiviteten Ändra data kan bearbeta högst en miljon poster per körning. Kontakta Adobe om du behöver höja denna gräns.

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Konfigurera aktiviteten Ändra datakälla {#configure}

Följ de här stegen för att konfigurera aktiviteten **Ändra datakälla**:

![Skärmbild som visar hur du lägger till aktiviteten Ändra datakälla i ett arbetsflöde.](../assets/workflow-change-data-source-add.png)

1. Lägg till en **Ändra datakällaktivitet** i arbetsflödet.

1. Definiera datakällan där du vill flytta arbetstabellen:

   * **[!UICONTROL Default Campaign database (PostgreSQL)]**: Använd den lokala standarddatabasen för kampanj.
   * **[!UICONTROL FDA external account]**: Använd externa molndatabaser som är anslutna till Adobe Campaign via funktionen för federerad dataåtkomst.

     >[!AVAILABILITY]
     >
     >Kampanjkonfiguration och anslutning till externa system är begränsade till avancerade användare och är endast tillgängliga från klientkonsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

1. Konfigurera arbetsflödet för att utföra önskade åtgärder med den nya datakällan.

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->