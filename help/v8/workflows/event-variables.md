---
audience: end-user
title: Händelsevariabler för arbetsflöde
description: Lär dig hur du utnyttjar händelsevariabler i dina arbetsflöden.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: c3f04d3828f22207bd5e9a0e8c334e8f7a57b2c1
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Händelsevariabler för arbetsflöde {#event-variables}

I vissa arbetsflödesaktiviteter kan du redigera skript i uttrycksredigeraren för att utföra specifika åtgärder som att hämta data från tidigare aktiviteter, skapa villkor eller beräkna filnamn baserat på händelsevariabler.

## Vad är händelsevariabler? {#scripting}

Skript som körs i samband med ett arbetsflöde får tillgång till en serie ytterligare globala **objekt** som själva arbetsflödet som körs (`ìnstance`), dess olika uppgifter (`task`), eller händelserna som aktiverade en viss uppgift (`event`).

Till varje typ av **object** är associerad med en kategori av **variabler** som kan användas i uttrycksredigeraren när skript redigeras i aktiviteter som **[!UICONTROL JavaScript code]** eller **[!UICONTROL Test]**.

* **Förekomstvariabler** (`instance.vars.xxx`) kan jämföras med globala variabler. De delas av alla aktiviteter.
* **Uppgiftsvariabler** (`task.vars.xxx`) kan jämföras med lokala variabler. De används bara av den aktuella uppgiften. Variablerna används av beständiga aktiviteter för att lagra data och används ibland för att utbyta data mellan olika skript för samma aktivitet.
* **Händelsevariabler** (`vars.xxx`) möjliggör datautbyte mellan de grundläggande uppgifterna i en arbetsflödesprocess. Dessa variabler skickas av aktiviteten som aktiverade den pågående uppgiften. De överförs sedan till följande aktiviteter. **Händelsevariabler** är de vanligaste variablerna och de bör användas i stället för förekomstvariabler.

>[!NOTE]
>
>Ytterligare information om skript och exponerade objekt och variabler i Adobe Campaign finns i dokumentationen för Campaign v8 (klientkonsolen) i [det här avsnittet](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Observera att även om den här resursen ger värdefulla insikter kan det finnas avvikelser eftersom den specifikt gäller klientkonsolen i stället för webbgränssnittet för Campaign.

## Utnyttja händelsevariabler i uttrycksredigeraren {#expression-editor}

Fördefinierade händelsevariabler är tillgängliga för användning i den vänstra delen av uttrycksredigeraren. Du kan också skapa nya variabler genom att initiera en ny variabel i koden.

![](assets/event-variables.png)

Förutom dessa händelsvariabler kan du även använda **[!UICONTROL Conditions]** i den vänstra rutan för att skapa villkor och **[!UICONTROL Add current date]** -meny om du vill använda funktioner för datumformatering.
