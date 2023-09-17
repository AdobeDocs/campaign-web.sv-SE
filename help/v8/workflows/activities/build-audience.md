---
audience: end-user
title: Använda aktiviteten Skapa målgruppsarbetsflöde
description: Lär dig använda aktiviteten Bygg målgruppsarbetsflöde
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---


# Bygg målgrupper {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Bygg målgrupper"
>abstract="The **Bygg målgrupper** kan du definiera målgruppen som ska delta i arbetsflödet. När du skickar meddelanden i ett arbetsflödes sammanhang definieras inte meddelandemålgruppen i kanalaktiviteten, utan i **Bygg målgrupper** aktivitet."


The **Bygg målgrupper** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du definiera målgruppen som ska delta i arbetsflödet. När du skickar meddelanden i ett arbetsflödes sammanhang definieras inte meddelandemålgruppen i kanalaktiviteten, utan i **Bygg målgrupper** aktivitet.

Om du vill definiera målgruppspopulationen kan du:

* Välj en befintlig målgrupp som skapats som en lista i klientkonsolen.
* Välj en Adobe Experience Platform-målgrupp.
* Bygg en ny målgrupp med regelbyggaren genom att definiera och kombinera filtervillkor.

>[!NOTE]
>
>I det här sammanhanget kan du inte läsa in en målgrupp från en fil. Därför måste du skapa en fristående e-postleverans. [Läs mer](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Konfigurera aktiviteten Skapa målgrupp

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Välj måldimension"
>abstract="Med målinriktningsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter osv. Som standard är målet markerat bland mottagarna."


Följ de här stegen för att konfigurera **Bygg målgrupper** aktivitet:

1. Lägg till en **Bygg målgrupper** aktivitet.
1. Definiera en etikett.
1. Definiera målgruppstyp: **Skapa en egen** eller **Läsa målgrupper**.

Så här skapar du en egen fråga:

1. Välj **Skapa en egen (fråga)**.
1. Välj **Måldimension**. Med målinriktningsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter osv. Som standard är målet markerat bland mottagarna. Se [v8-dokumentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Klicka **Fortsätt**.
1. Använd regelbyggaren för att definiera frågan, på samma sätt som du skapar en målgrupp när du utformar ett nytt e-postmeddelande. Se detta [section](../../audience/segment-builder.md).

Så här väljer du en befintlig målgrupp:

1. Välj **Läsa målgrupper**.
1. Klicka **Fortsätt**.
1. Välj målgrupp på samma sätt som du använder en målgrupp när du utformar ett nytt e-postmeddelande. Se detta [section](../../audience/add-audience.md).

## Exempel

Här är ett exempel på ett arbetsflöde med två **Bygg målgrupper** verksamhet. Det första riktar sig till pokerspelarna, följt av ett mejlerbjudande. Det andra riktar sig till VIP kunder, följt av en SMS-leverans.

![](../assets/workflow-audience-example.png)