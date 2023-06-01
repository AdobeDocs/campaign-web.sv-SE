---
audience: end-user
title: Använda arbetsflödesaktiviteten AND-join
description: Lär dig hur du använder arbetsflödesaktiviteten OCH-join
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---


# AND-join {#join}

The **Och-join** kan du synkronisera flera körningsgrenar i ett arbetsflöde.

AND-join-aktiviteten utlöser endast sin utgående övergång när alla inkommande övergångar har aktiverats, det vill säga när alla föregående aktiviteter har slutförts.

Följ de här stegen för att konfigurera **AND-join** aktivitet:

1. Lägg till flera aktiviteter som **Kombinera** aktiviteter för att bilda minst två olika utförandegrenar.
1. Lägg till en **AND-join** till någon av grenarna.
1. I **Sammanfogningsalternativ** markerar du alla tidigare aktiviteter du vill delta i.
1. Välj **Primär uppsättning** som ska behållas i den utgående övergången.
