---
audience: end-user
title: Använda aktiviteten Skapa målgruppsarbetsflöde
description: Lär dig använda aktiviteten Bygg målgruppsarbetsflöde
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# Bygg målgrupper {#build-audience}

Med den här aktiviteten kan du definiera en målgrupp. Du kan antingen välja en befintlig Campaign-förekomst eller använda regelbyggaren för att definiera en egen fråga.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

Följ de här stegen för att konfigurera **Bygg målgrupper** aktivitet:

1. Lägg till en Build-målgruppsaktivitet.
1. Definiera en etikett.
1. Definiera målgruppstyp: **Skapa en egen** eller **Läsa målgrupper**.

Så här skapar du en egen fråga:

1. Välj **Skapa en egen (fråga)**.
1. Välj **Måldimension**. Med måldimensionen kan du definiera målgruppen för åtgärden: mottagare, mottagare, mottagare, operatör, abonnenter osv. Som standard är målet markerat bland mottagarna. Se [v8-dokumentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Klicka **Fortsätt**.
1. Använd regelbyggaren för att definiera frågan, på samma sätt som du skapar en målgrupp när du utformar ett nytt e-postmeddelande. Se detta [section](../../audience/segment-builder.md).

Så här väljer du en befintlig målgrupp:

1. Välj **Läsa målgrupper**.
1. Klicka **Fortsätt**.
1. Välj målgrupp på samma sätt som du använder en målgrupp när du utformar ett nytt e-postmeddelande. Se detta [section](../../audience/add-audience.md).
