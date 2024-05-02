---
audience: end-user
title: Använd extern signalaktivitet
description: Lär dig hur du använder arbetsflödesaktiviteten för externa signaturer
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Extern signal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Extern signal"
>abstract="The **Extern signal** Med -aktivitet kan du utlösa ett arbetsflöde från ett annat arbetsflöde eller ett API-anrop."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Externa signalparametrar"
>abstract="Externa signalparametrar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Slututlösare"
>abstract="Slututlösare"

The **Extern signal** aktiviteten är en **Flödeskontroll** aktivitet. Det gör att du kan utlösa körningen av ett arbetsflöde från ett annat arbetsflöde eller från ett API-anrop.

>[!NOTE]
>
>Den här sidan innehåller de viktigaste stegen för att konfigurera **[!UICONTROL External Signal]** i Campaign Web User Interface och utlösa det från ett annat arbetsflöde eller ett API-anrop. Detaljerad information om hur du utlöser ett arbetsflöde och dess bästa metoder samt hur du arbetar med Campaign-API:er finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Följ de här stegen för att konfigurera **Extern signal** och utlösa dess körning:

1. Lägg till en **Extern signal** i arbetsflödet.

1. Slutför konfigurationen av arbetsflödet och starta körningen. The **[!UICONTROL External Signal]** aktiviteten visas som &quot;Väntande&quot;, väntar på att utlösas.

   ![](../assets/external-signal-pending.png)

1. Hämta informationen nedan:

   * The **arbetsflödets interna namn**, som visas bredvid etiketten.

     +++Exempel på vy

     ![](../assets/external-signal-workflow-name.png)

+++

   * The **Namn på extern signalaktivitet** som visas i arbetsflödets **[!UICONTROL Execution options]**.

     +++Exempel på vy

     ![](../assets/external-signal-name.png)

+++

1. För att starta arbetsflödet måste du köra `PostEvent` JavaScript-funktion. Med den här funktionen kan du skicka variabler med valfria värden och använda dem i det utlösta arbetsflödet.

   The `PostEvent` kan köras antingen från ett annat arbetsflöde eller från ett API-anrop.

   * Så här utlöser du en **[!UICONTROL External signal]** från ett arbetsflöde, köra PostEvent-funktionen från **[!UICONTROL Initialization script]** som är tillgänglig från aktivitetens **[!UICONTROL Execution options]**. För **[!UICONTROL JavaScript code]** kör du funktionen från aktivitetens skript.

     Syntaxen är följande:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Exempel på vy

   I det här exemplet utlöser vi den externa signalaktiviteten &quot;signal1&quot; som har lagts till i arbetsflödet vars interna namn är &quot;WKF12345&quot;. Vi skickar också en variabel som heter &quot;customID&quot;, med värdet &quot;123456&quot;.

   ![](../assets/external-signal-sample.png)

+++

   * Så här utlöser du en **[!UICONTROL External signal]** -aktivitet från ett API-anrop, följ stegen som beskrivs i dokumentationen för Campaign API. [Lär dig använda den statiska `PostEvent` method](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
