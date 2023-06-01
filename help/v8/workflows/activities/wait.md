---
audience: end-user
title: Använd aktiviteten Vänta i arbetsflödet
description: Lär dig hur du använder aktiviteten Vänta i arbetsflödet
badge: label="Alpha" type="Positive"
source-git-commit: 9be56c3c9c7a339e1f348ac9c74d425b501c317d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 37%

---


# Vänta {#wait}

The **Vänta** aktiviteten tillfälligt avbryter körningen av en del av ett arbetsflöde. Den aktiverar sin utgående övergång efter en fördröjning som kan variera från några sekunder till flera månader, vilket verkställer de aktiviteter som utförs efteråt.

The **Vänta** aktiviteten används för att en viss tid ska kunna förflyta mellan två aktiviteter som körs. Om du till exempel vill vänta flera dagar efter en aktivitet där e-post levererats så analyserar du de öppningar och klick som genereras under den här perioden innan du utför några uppföljningsåtgärder (påminnelser via e-post, målgruppsgenerering osv.).

## Konfiguration

Följ de här stegen för att konfigurera **Vänta** aktivitet:

1. Lägg till en **Vänta** i arbetsflödet.

1. Ange **Varaktighet** av väntetiden mellan aktiveringen av de inkommande och utgående övergångarna för aktiviteten.

1. Välj tidsenhet **Period**: sekunder, minuter, timmar.

## Exempel

I följande exempel visas **Vänta** i vanliga fall. En e-postinbjudan till ett event skickas.  24 timmar efter att det skickats skickas ett SMS-meddelande till samma population.

![](../assets/workflow-wait-example.png)
