---
audience: end-user
title: Använd aktiviteten Vänta i arbetsflödet
description: Lär dig hur du använder aktiviteten Vänta i arbetsflödet
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 40%

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


