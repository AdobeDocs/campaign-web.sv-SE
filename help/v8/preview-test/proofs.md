---
audience: end-user
title: Skicka testmeddelanden
description: Lär dig hur du definierar och skickar testmeddelanden
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: d305cc7055008ecf25e41a51fabe1e5ece683b72
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Skicka testmeddelanden {#send-proofs}

![](../assets/do-not-localize/badge.png)

Att skicka testmeddelanden är ett viktigt steg när det gäller att validera din e-postkampanj och identifiera potentiella problem. Genom att skicka testmeddelanden kan du kontrollera olika element som länkar, avanmälningslänkar, bilder och spegelsidor samt upptäcka eventuella fel.

Testmeddelanden kan skickas till två typer av mottagare:

* **Testprofiler**: skicka testmeddelanden till dirigerade adresser, som är ytterligare och fiktiva mottagare i databasen. De kan skapas i Adobe Campaign Console i **[!UICONTROL Resources]** / **[!UICONTROL Campaign Management]** / **[!UICONTROL Seed addresses]** mapp.

* **Ersättning från huvudmål**: skicka testmeddelanden till en viss e-postadress samtidigt som du personifierar en befintlig profil. På så sätt kan du uppleva e-postmeddelandet som mottagarna vill, vilket ger dig en korrekt representation av meddelandet som profilen kommer att ta emot.

## Välj testmottagare {#recipients}

1. Öppna skärmen för simulering av e-postinnehåll och klicka sedan på **[!UICONTROL Test]** -knappen.

   ![](assets/test-button.png)

1. Använd **[!UICONTROL Mode]** nedrullningsbar lista där du kan välja vilken typ av mottagare som ska få testmeddelandet:

   * **Testprofiler**: skicka testmeddelandet till startadresser som är ytterligare och fiktiva mottagare i databasen,

   * **Ersättning från huvudmål**: skicka testmeddelandet till en viss e-postadress samtidigt som du personifierar en befintlig profil. På så sätt kan du uppleva e-postmeddelandet som mottagarna vill, vilket ger dig en korrekt representation av meddelandet som profilen kommer att ta emot.

   ![](assets/test-mode.png)

   >[!NOTE]
   >
   >Som standard är **[!UICONTROL Test profiles]** läge är valt. Om du redan har markerat profiler för att förhandsgranska e-postmeddelandet på innehållssimuleringsskärmen, markeras de profilerna som testmottagare. Du kan rensa markeringen och/eller lägga till fler mottagare.

1. Om du vill skicka testmeddelanden till ersättningsprofiler väljer du **[!UICONTROL Substitution from target]** gör du så här:

   1. Klicka på **[!UICONTROL Add address]** och ange den e-postadress som ska ta emot testmeddelandet.

      Du kan ange valfri e-postadress. Detta gör att du kan skicka testmeddelanden till alla användare, även om de inte är användare av Adobe Campaign V8.

   1. Välj den profil från målet som ska användas för att skicka testmeddelandet. Du kan också låta Adobe Campaign välja en slumpmässig profil från målet.

   1. Bekräfta mottagaren och upprepa åtgärden för att lägga till så många adresser som behövs.

      ![](assets/substitution.png)

1. När testmottagarna har valts kan du skicka testmeddelandet. [Lär dig hur du skickar testmeddelanden](#send)

   >[!NOTE]
   >
   >Om du vill skicka det sista e-postmeddelandet till mottagarna av testmeddelandet aktiverar du **[!UICONTROL Include test population in the main target]** på.

## Skicka testmeddelandet {#send}

Om du vill skicka testmeddelandet till de valda mottagarna klickar du på **[!UICONTROL Send test email]** bekräfta sändningen.

![](assets/send-proof.png)

Skicka så många testmeddelanden som behövs tills du är klar med innehållet. När detta är klart kan du skicka e-postmeddelandet till huvudmålet. [Lär dig hur du förbereder och skickar e-post](../monitor/prepare-send.md)

## Få tillgång till skickade testmeddelanden {#access-proofs}

När testmeddelandena har skickats kan du få åtkomst till dedikerade loggar från **[!UICONTROL View test email log]** -knappen.

Med dessa loggar kan du få tillgång till alla testmeddelanden som skickats för den valda leveransen och visa specifik statistik som relaterar till deras sändning. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

![](assets/proof-log.png)

Du kan även komma åt skickade testmeddelanden från leveranslistan, precis som vid alla leveranser.

![](assets/delivery-list.png)
