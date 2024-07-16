---
audience: end-user
title: Använd extern signalaktivitet
description: Lär dig hur du använder arbetsflödesaktiviteten för externa signaturer
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Extern signal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Extern signal"
>abstract="Med aktiviteten **Extern signal** kan du utlösa körningen av ett arbetsflöde från ett annat arbetsflöde eller ett API-anrop."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Externa signalparametrar"
>abstract="Externa signalparametrar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Slututlösare"
>abstract="Slututlösare"

Aktiviteten **Extern signal** är en **Flödeskontroll**-aktivitet. Det gör att du kan utlösa körningen av ett arbetsflöde från ett annat arbetsflöde eller från ett API-anrop.

>[!NOTE]
>
>Den här sidan innehåller de viktigaste stegen för att konfigurera en **[!UICONTROL External Signal]**-aktivitet i webbgränssnittet för Campaign och utlösa den från ett annat arbetsflöde eller ett API-anrop. Detaljerad information om hur du utlöser ett arbetsflöde och dess bästa metoder samt hur du arbetar med Campaign-API:er finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Följ de här stegen för att konfigurera aktiviteten **Extern signal** och utlösa dess körning:

1. Lägg till en **extern signalaktivitet** i arbetsflödet.

1. Slutför konfigurationen av arbetsflödet och starta körningen. Aktiviteten **[!UICONTROL External Signal]** visas som Väntande, väntar på att utlösas.

   ![](../assets/external-signal-pending.png)

1. Hämta informationen nedan:

   * **Arbetsflödets interna namn**, som visas bredvid dess etikett.

     +++Exempel på vy

     ![](../assets/external-signal-workflow-name.png)

+++

   * **Den externa signalaktivitetens namn**, som visas i arbetsflödets **[!UICONTROL Execution options]**.

     +++Exempel på vy

     ![](../assets/external-signal-name.png)

+++

1. Om du vill utlösa arbetsflödet måste du köra JavaScript-funktionen `PostEvent`. Med den här funktionen kan du skicka variabler med valfria värden och använda dem i det utlösta arbetsflödet.

   Funktionen `PostEvent` kan köras antingen från ett annat arbetsflöde eller från ett API-anrop.

   * Om du vill utlösa en **[!UICONTROL External signal]**-aktivitet från ett arbetsflöde kör du PostEvent-funktionen från rutan **[!UICONTROL Initialization script]** som är tillgänglig från aktivitetens **[!UICONTROL Execution options]**. Kör funktionen från aktivitetens skript för aktiviteten **[!UICONTROL JavaScript code]**.

     Syntaxen är följande:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Exempel på vy

   I det här exemplet utlöser vi den externa signalaktiviteten &quot;signal1&quot; som har lagts till i arbetsflödet vars interna namn är &quot;WKF12345&quot;. Vi skickar också en variabel som heter &quot;customID&quot;, med värdet &quot;123456&quot;.

   ![](../assets/external-signal-sample.png)

+++

   * Om du vill utlösa en **[!UICONTROL External signal]**-aktivitet från ett API-anrop följer du stegen som beskrivs i dokumentationen för Campaign API. [Lär dig använda den statiska `PostEvent`-metoden ](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
