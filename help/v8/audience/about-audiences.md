---
audience: end-user
title: Kom igång med målgrupper
description: Lär dig hur du använder målgrupper i gränssnittet för Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 3ebe92659916cf2fa4cacb8d28b79d7b6d5359f3
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Kom igång med målgrupper {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


Målgruppen är er leverans: de mottagare som tar emot meddelandena. Vilken typ av målgrupp det är beror på målmappningen som definieras i leveransmallen. Lär dig vad som är en leveransmall [i det här avsnittet](../msg/delivery-template.md).

Om du vill definiera målgruppspopulationen kan du:

* Välj en befintlig målgrupp som skapats som en lista i klientkonsolen. [Läs mer](add-audience.md)
* Välj en Adobe Experience Platform-målgrupp. [Läs mer](aep-audience.md)
* Bygg en ny målgrupp med regelbyggaren genom att definiera och kombinera filtervillkor. [Läs mer](segment-builder.md)
* Använd en målgrupp från en extern fil: det här alternativet är bara tillgängligt för fristående e-postleveranser och kan inte användas i kampanjleveranser. [Läs mer](file-audience.md)

När meddelanden skickas i samband med ett kampanjarbetsflöde definieras målgruppen i en specifik **Läsa målgrupper** arbetsflödesaktivitet. I det här sammanhanget kan du inte läsa in en målgrupp från en fil för en e-postleverans, och målgruppen definieras endast i den här dedikerade aktiviteten. Lär dig definiera målgruppen för leveransen i ett kampanjarbetsflöde [i det här avsnittet](../workflows/orchestrate-activities.md).

Dessutom kan ni definiera kontrollgrupper för att undvika att skicka meddelanden till en del av er målgrupp och mäta effekten av era kampanjer. [Läs mer](control-group.md)

![](assets/about-audience.png)

