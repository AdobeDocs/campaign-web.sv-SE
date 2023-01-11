---
audience: end-user
title: Skicka korrektur
description: Webbdokumentation för Campaign v8
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 3%

---

# Skicka korrektur {#send-proofs}

![](../assets/do-not-localize/badge.png)

Genom att skicka testmeddelanden kan du validera din e-post och kontrollera olika element som länkar, avanmälningslänkar och spegelsidor, bilder och upptäcka eventuella fel.

Korrektur kan skickas till två typer av mottagare:

* **Testprofiler**: skicka korrektur till startadresser, som är ytterligare och fiktiva mottagare i databasen,
* **Ersättningsprofiler**: skicka korrektur till en viss e-postadress med hjälp av en befintlig profil. På så sätt kan du placera dig själv i profilernas position och få en exakt representation av meddelandet som profilen får.

## Välj korrekturmottagare {#recipients}

1. Öppna skärmen för att skapa e-postinnehåll och klicka sedan på **[!UICONTROL Simulate content]**.

1. Klicka på **[!UICONTROL Test]** använder du **[!UICONTROL Mode]** i listrutan för att välja vilken typ av mottagare som ska få korrektur:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Skicka korrektur till testprofiler

1. Välj **[!UICONTROL Use test profiles]**-läget.

1. Lägg till de testprofiler som ska ta emot testmeddelanden.

   <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

   ![](assets/test-profiles-audience.png)

### Skicka korrektur till ersättningsprofiler

1. Välj **[!UICONTROL Substitution from target]**-läget.

1. Lägg till den eller de e-postadresser som ska ta emot korrekturen.

   >[!NOTE]
   >
   >Du kan ange valfri e-postadress. Detta gör att du kan skicka korrektur till alla användare, även om de inte är användare av Adobe Campaign V8.

1. För varje e-postadress väljer du profilen i det mål som ska användas. Du kan också låta Adobe Campaign välja en slumpmässig profil från målet.

   ![](assets/substitution.png)

När du har valt korrekturmottagare kan du skicka testmeddelandet. [Lär dig hur du skickar korrektur](#send)

>[!NOTE]
>
>Om du vill skicka det sista e-postmeddelandet till mottagarna av korrekturet aktiverar du **[!UICONTROL Include test population in the main target]** på.

## Skicka korrektur {#send}

Om du vill skicka korrekturen till de valda mottagarna klickar du på **[!UICONTROL Send test email]** bekräfta sändningen.

![](assets/send-proof.png)

Skicka så många korrektur som behövs tills du är klar med leveransens innehåll. När detta är klart kan du skicka e-postmeddelandet till huvudmålet. [Lär dig hur du förbereder och skickar e-post](../monitor/prepare-send.md)

## Åtkomst till skickade korrektur {#access-proofs}

När korrekturet har skickats kan du få åtkomst till dedikerade loggar från **[!UICONTROL View test email log]** -knappen. Med dessa loggar kan du komma åt alla korrektur som skickats för den valda leveransen och visa specifik statistik som relaterar till deras sändning.

![](assets/proof-log.png)

Du kan även komma åt korrektur från leveranslistan, precis som vid alla leveranser.

![](assets/delivery-list.png)
