---
audience: end-user
title: Skicka testmeddelanden
description: Lär dig hur du definierar och skickar testmeddelanden
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positive"
source-git-commit: acc6cdd89b78a26f7c2435e19fba148a71e4f18f
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Skicka testmeddelanden {#send-test-emails}

**[!UICONTROL Adobe Campaign]** gör att du kan testa ett meddelande innan det skickas till huvudmålgruppen.

Att skicka testmeddelanden är ett viktigt steg när det gäller att validera din e-postkampanj och identifiera potentiella problem.

Mottagarna av ett test kan kontrollera olika element som länkar, avanmälningslänkar, bilder och spegelsidor samt upptäcka eventuella fel i återgivning, innehåll, personaliseringsinställningar och e-postkonfiguration.

## Välj testmottagare {#test-recipients}

Testmeddelanden kan skickas till två typer av mottagare:

* **Testprofiler** - skicka testmeddelanden till dirigerade adresser som är ytterligare och fiktiva mottagare i databasen. De kan skapas i [!DNL Campaign] konsolen i **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** mapp. Läs mer i [Kampanjdokumentation v8 (konsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* **Ersätt från huvudmål** - skicka testmeddelanden till en viss e-postadress samtidigt som du personifierar en befintlig profil. På så sätt kan du uppleva e-postmeddelandet som mottagarna vill, vilket ger dig en korrekt representation av meddelandet som profilen kommer att ta emot.

Följ stegen nedan för att välja mottagare av e-posttestet.

1. Öppna e-postmeddelandet [Redigera innehåll](../content/edit-content.md) eller till [E-postdesigner](../content/get-started-email-designer.md)klickar du på **[!UICONTROL Simulate content]** -knappen.

1. Klicka på knappen **[!UICONTROL Test]**.

   ![](assets/simulate-test-button.png)

1. Använd **[!UICONTROL Mode]** nedrullningsbar lista där du kan välja vilken typ av mottagare som ska få testmeddelandet:

   * **Testprofiler** inrikta sig på fiktiva mottagare

   * **Ersätt från huvudmål** för att skicka ett test till en viss e-postadress samtidigt som data från en befintlig profil visas.

   ![](assets/simulate-profile-mode.png)

   >[!NOTE]
   >
   >Som standard är **[!UICONTROL Use test profiles]** läge är valt. Om du redan har markerat profiler för att förhandsgranska e-postmeddelandet på innehållssimuleringsskärmen, markeras de profilerna som testmottagare. Du kan rensa markeringen och/eller lägga till fler mottagare.

1. Om du vill skicka testmeddelanden till ersättningsprofiler väljer du **[!UICONTROL Substitute from target]** gör du så här:

   1. Klicka på **[!UICONTROL Add address]** och ange den e-postadress som tar emot testmeddelandet.

      Du kan ange valfri e-postadress. Detta gör att du kan skicka testmeddelanden till alla användare, även om de inte är användare av [!DNL Adobe Campaign].

   1. Välj den profil från målet som ska användas som ersättning. Du kan också låta [!DNL Adobe Campaign] välj en slumpmässig profil från målet. Profildata från den valda profilen visas i testmeddelandet.

   1. Bekräfta mottagaren och upprepa åtgärden för att lägga till så många adresser som behövs.

      ![](assets/simulate-profile-substitute.png)

1. När testmottagarna har valts kan du [skicka testmeddelandet](#send-test).

   >[!NOTE]
   >
   >Om du även vill skicka det sista e-postmeddelandet till mottagarna av testmeddelandet väljer du **[!UICONTROL Include test population in the main target]** alternativ.

## Skicka testmeddelandet {#send-test}

Följ stegen nedan för att skicka testmeddelandet till de valda mottagarna.

1. Klicka på **[!UICONTROL Send test email]**.

1. Bekräfta sändningen.

   ![](assets/simulate-send-test.png)

1. Skicka så många testmeddelanden som behövs tills du är klar med innehållet.

När detta är klart kan du [förbereda och skicka e-post](../monitor/prepare-send.md) till huvudmålet.

## Få tillgång till skickade testmeddelanden {#access-proofs}

När testmeddelandena har skickats kan du få åtkomst till dedikerade loggar från **[!UICONTROL View test email log]** -knappen.

Med dessa loggar kan du få tillgång till alla testmeddelanden som skickats för den valda leveransen och visa specifik statistik som relaterar till deras sändning. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Du kan även komma åt skickade testmeddelanden via [leveranslista](../msg/gs-messages.md), som alla leveranser.

![](assets/simulate-deliveries-list.png)
