---
audience: end-user
title: Övervaka leveransloggar
description: Lär dig övervaka leveransloggar
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
badge: label="Alpha"
source-git-commit: f7ffa5daaff1ad57bba365bc09ed24fa08a277f0
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 25%

---

# Övervaka leveransloggar {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Leveransloggar"
>abstract="Leveransloggarna visar information om sändningen. De visar detaljerna för utskicket, vilket eller vilka mål som har uteslutits och varför de har uteslutits. De visar även spårningsinformation som exempelvis öppningar och klick."

När leveransen är klar och du klickade på **Skicka** bläddra till leveransloggarna för att kontrollera varningar, fel, status, undantag och spårningsdata. Loggarna kan nås direkt från meddelandekontrollpanelen. De visar detaljerna för utskicket, vilket eller vilka mål som har uteslutits och varför de har uteslutits. De visar även spårningsinformation som exempelvis öppningar och klick.

Om du vill visa loggarna öppnar du kontrollpanelen för leverans och klickar på **Loggar** -knappen.

Följande flikar är tillgängliga:

* [Loggar](#logs-tab)
* [Leveranser](#deliveries-tab)
* [Undantag](#exclusion-tab)
* [Uteslutningsorsaker](#exclusion-causes)
* [Spårade URL:er](#tracked-urls)
* [Spåra](#tracking)

## Loggar {#logs-tab}

The **Loggar** -fliken innehåller alla meddelanden som rör leveransen och korrekturet. Med specifika ikoner kan du identifiera fel eller varningar.    

Alla valideringssteg, varningar och fel visas. Färgade ikoner visar meddelandetypen:

* Den grå ikonen visar ett informativt meddelande.
* Den gula ikonen indikerar ett icke-kritiskt bearbetningsfel.
* Den röda ikonen anger ett kritiskt fel som förhindrar leverans. Allvarliga fel måste åtgärdas för att leveransen ska kunna skickas.

![](assets/logs.png)


## Leveranser {#deliveries-tab}

The **Skicka loggar** På -fliken finns en historik över alla förekomster av leveransen. Listan med skickade meddelanden och deras status lagras här.        Du kan visa leveransstatus för varje mottagare.

![](assets/logs2.png)

## Undantag {#exclusion-tab}

The **Uteslutningsloggar** På -fliken visas alla meddelanden som har uteslutits från målet och orsaken till sändningsfelet anges.

![](assets/logs3.png)

## Uteslutningsorsaker {#exclusion-causes-tab}

The **Uteslutningsorsaker** för varje möjlig orsak visas antalet meddelanden som har uteslutits från målet.

![](assets/logs4.png)

## Spårade URL:er {#tracked-urls-tab}

The **Spårade URL:er** På fliken grupperas URL:erna i skickade meddelanden, inklusive deras URL-typ och deras käll-URL.

![](assets/logs5.png)

## Spåra {#tracking-tab}

The **Spårning** På -fliken visas spårningshistoriken för leveransen. På den här fliken visas spårningsdata för skickade meddelanden, d.v.s. alla URL:er som spåras av Adobe Campaign.


![](assets/logs6.png)

>[!NOTE]
>
>Om spårning inte är aktiverat för en leverans visas inte den här fliken.