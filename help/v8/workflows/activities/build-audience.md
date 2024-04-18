---
audience: end-user
title: Använda aktiviteten Skapa målgruppsarbetsflöde
description: Lär dig använda aktiviteten Bygg målgruppsarbetsflöde
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: a98203e983fec6e55f8c60e254f965f20ffe7dea
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# Bygg målgrupper {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Bygg målgruppsaktivitet"
>abstract="The **Bygg målgrupper** kan du definiera målgruppen som ska delta i arbetsflödet. När du skickar meddelanden i ett arbetsflödes sammanhang definieras inte meddelandemålgruppen i kanalaktiviteten, utan i **Bygg målgrupper** aktivitet."

The **Bygg målgrupper** aktiviteten är en **Målinriktning** aktivitet. Med den här aktiviteten kan du definiera målgruppen som ska delta i arbetsflödet. När du skickar meddelanden i ett arbetsflödes sammanhang definieras inte meddelandemålgruppen i kanalaktiviteten, utan i **Bygg målgrupper** aktivitet.

Om du vill definiera målgruppspopulationen kan du:

* Välj en befintlig målgrupp som skapats som en lista i klientkonsolen.
* Välj en Adobe Experience Platform-målgrupp.
* Bygg en ny målgrupp med frågemodelleraren genom att definiera och kombinera filtervillkor.

>[!NOTE]
>
>Målgrupper som läses in från en fil kan inte anges som mål med en Build-målgruppsaktivitet. För att göra detta måste du använda en **Läs in fil** aktivitet följt av **Avstämning** aktivitet. [Läs mer](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Konfigurera aktiviteten Skapa målgrupp{#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_audienceselector"
>title="Målgrupp"
>abstract="Målgrupp"

Följ de här stegen för att konfigurera **Bygg målgrupper** aktivitet:

![](../assets/workflow-audience.png)

1. Lägg till en **Bygg målgrupper** aktivitet.
1. Definiera en etikett.
1. Definiera målgruppstyp: **Skapa en egen** eller **Läsa målgrupper**.
1. Konfigurera målgruppen genom att följa stegen som beskrivs på flikarna nedan.

>[!BEGINTABS]

>[!TAB Skapa en egen (fråga)]

Så här skapar du en egen fråga:

1. Välj **Skapa en egen (fråga)**.
1. Välj **Måldimension**. Med målinriktningsdimensionen kan du definiera målgruppen för operationen: mottagare, mottagare, operatör, prenumeranter osv. Som standard är målet markerat bland mottagarna. [Läs mer om målinriktning](../../audience/about-recipients.md#targeting-dimensions)
1. Klicka **Fortsätt**.
1. Använd frågemodelleraren för att definiera frågan, på samma sätt som du skapar en målgrupp när du utformar ett nytt e-postmeddelande. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

>[!TAB Läs målgrupp]

Så här väljer du en befintlig målgrupp:

1. Välj **Läsa målgrupper**.
1. Klicka **Fortsätt**.
1. Välj målgrupp på samma sätt som du använder en målgrupp när du designar en ny leverans. Se detta [section](../../audience/add-audience.md).

>[!ENDTABS]

## Exempel{#build-audience-examples}

Här är ett exempel på ett arbetsflöde med två **Bygg målgrupper** verksamhet. Det första riktar sig till pokerspelarna, följt av ett mejlerbjudande. Det andra riktar sig till VIP kunder, följt av en SMS-leverans.

![](../assets/workflow-audience-example.png)
