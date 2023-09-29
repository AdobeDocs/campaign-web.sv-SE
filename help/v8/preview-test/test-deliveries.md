---
audience: end-user
title: Skicka testleveranser
description: Lär dig hur du definierar och skickar testleveranser
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Beta"
source-git-commit: 2f065c6a0d4daef1cafbcb5f9d8d666fbe716932
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Skicka testleveranser {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Förhandsgranskningsläge"
>abstract="Förhandsgranska och testa meddelandet genom att inkludera testpopulationen i huvudmålet."

När meddelandeinnehållet har definierats kan du förhandsgranska och testa det genom att skicka testleveranser till testprofiler. Om du har infogat anpassat innehåll kan du kontrollera hur det här innehållet visas i meddelandet med hjälp av testprofildata.

Om du vill identifiera eventuella fel i meddelandeinnehållet eller personaliseringsinställningarna skickar du testmeddelanden till testprofiler innan du skickar dem till målgruppen. Ett testmeddelande ska skickas varje gång en ändring görs för att validera det senaste innehållet. Att skicka testleveranser (som tidigare kallats korrektur) är ett viktigt steg när det gäller att validera kampanjen och identifiera potentiella problem. Mottagarna av ett testmeddelande kan kontrollera olika element som länkar, avanmälningslänkar, bilder eller spegelsidor samt upptäcka eventuella fel i återgivning, innehåll, personaliseringsinställningar och leveranskonfiguration.

## Simulera innehåll med testmottagare {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Testpopulation"
>abstract="Välj ett testpopulationsläge."

Innan du skickar ett test måste du definiera en målgrupp för leveransen. [Läs mer](../audience/about-recipients.md)


Så här börjar du testa ditt meddelandeinnehåll:

1. Redigera innehållet i leveransen.
1. Klicka på knappen **[!UICONTROL Simulate content]**.
1. Klicka på **[!UICONTROL Test]** för att skicka testmeddelanden.

   ![](assets/simulate-test-button-email.png)

1. Välj testmottagare.

   Beroende på meddelandekanalen kan testmeddelanden skickas till följande typer av mottagare:

   * För SMS och e-post kan du använda [testprofiler](#test-profiles), som är specifika ytterligare mottagare i databasen. Dessa mottagare skapas i [!DNL Campaign] klientkonsol. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * För SMS och e-post kan du även använda [ersättning från huvudmålet](#substitution-profiles) läge, som skickar testmeddelanden till e-postadress eller telefonnummer och använder personaliseringsdata för en befintlig profil. På så sätt kan du uppleva meddelandet som mottagarna, vilket ger dig en korrekt representation av innehållet som profilen kommer att ta emot.

   * För push-meddelanden kan du använda [prenumeranter](#subscribers), som är fiktiva prenumeranter som läggs till i databasen. De skapas i [!DNL Campaign] konsol. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   Detaljerad konfiguration för varje läge finns nedan.

## Använda testprofiler {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Mål för beviset"
>abstract="Du kan överföra ytterligare en fil som &#39;mål för korrekturet&#39; om du vill testa leveransen innan du skickar till huvudmålet."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Överför profiler"
>abstract="Du kan överföra ytterligare en fil med ytterligare profiler om du vill testa leveransen med en annan uppsättning än den som du har använt för huvudmålet."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Mallfil"
>abstract="Formateringen för filen måste vara densamma som för originalfilen.<br/>Filformat som stöds: txt, csv. Största filstorlek: 15 MB. Använd den första raden som kolumnrubrik."


Testprofiler är dirigerade adresser, som är ytterligare mottagare i databasen. De kan skapas i [!DNL Adobe Campaign] klientkonsol. Stegen för att skicka testmeddelanden till dirigerade adresser beskrivs nedan.

1. Klicka på **[!UICONTROL Simulate content]** och **[!UICONTROL Test]** -knappen.

1. Från **[!UICONTROL Mode]** nedrullningsbar lista, välja **[!UICONTROL Test profiles]** för att rikta sig till fiktiva mottagare som får testmeddelandet eller SMS-leveransen.

   ![](assets/simulate-profile-mode.png)

1. Om du redan har valt profiler till [förhandsgranska meddelandet](preview-content.md) på skärmen för innehållssimulering är dessa profiler förmarkerade som testmottagare. Du kan rensa markeringen och/eller lägga till fler mottagare med **[!UICONTROL Add test profile(s)]** -knappen.

1. Om du även vill skicka det slutliga meddelandet till mottagarna av testleveransen väljer du **[!UICONTROL Include test population in the main target]** alternativ.

1. När du har valt testprofilerna kan du [skicka testleveransen](#send-test).

## Ersätt profildata {#substitution-profiles}

Använd profilersättning för att skicka testmeddelanden till en viss e-postadress eller ett visst telefonnummer, samtidigt som data från en befintlig profil i [!DNL Adobe Campaign] databas. Gör så här:


1. Klicka på **[!UICONTROL Simulate content]** och **[!UICONTROL Test]** -knappen.

1. Från **[!UICONTROL Mode]** nedrullningsbar lista, välja **[!UICONTROL Substitute from main target]** för att skicka ett test till en viss e-postadress eller ett visst telefonnummer samtidigt som data från en befintlig profil visas.

   >[!CAUTION]
   >
   >Om du inte har valt en [publik](../audience/about-recipients.md) för leverans, **[!UICONTROL Substitute from main target]** är nedtonat och du kan inte välja ersättningsprofiler.

1. Klicka på **[!UICONTROL Add address]** och ange den e-postadress eller det telefonnummer som ska ta emot testleveransen.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >Du kan ange valfri e-postadress eller valfritt telefonnummer. Detta gör att du kan skicka testleveranser till alla mottagare, även om de inte är användare av [!DNL Adobe Campaign].

1. Välj profilen från det mål som du har definierat för leveransen som ska användas som ersättning. Du kan också låta [!DNL Adobe Campaign] välj en slumpmässig profil från målet. Profildata från den valda profilen visas vid testleveransen.

1. Bekräfta mottagaren och upprepa åtgärden för att lägga till så många e-postadresser eller telefonnummer som behövs.

   ![](assets/simulate-profile-substitute.png)

1. Om du även vill skicka det slutliga meddelandet till mottagarna av testleveransen väljer du **[!UICONTROL Include test population in the main target]** alternativ.

1. När ersättningsprofilerna är valda kan du [skicka testleveransen](#send-test).

## Skicka tester till prenumeranter {#subscribers}

När du arbetar med push-meddelanden kan testleveranser bara skickas till dina appprenumeranter. Följ stegen nedan för att välja dem.

1. Klicka på **[!UICONTROL Simulate content]** och **[!UICONTROL Test]** -knappen.

   ![](assets/simulate-test-button-push.png)

1. Om du redan har valt abonnenter på [förhandsgranska leveransen](preview-content.md) på skärmen för innehållssimulering är dessa profiler förvalda som testprenumeranter.

   Du kan rensa urvalet och/eller lägga till ytterligare prenumeranter med den dedikerade knappen.

   ![](assets/simulate-test-subscribers.png)

1. Om du även vill skicka det sista push-meddelandet till testprenumeranterna väljer du **[!UICONTROL Include test population in the main target]** alternativ.

1. När prenumeranterna har valts kan du [skicka testleveransen](#send-test).

## Skicka testleveransen {#send-test}

Följ stegen nedan för att skicka testleveransen till de valda mottagarna.

1. Klicka på knappen **[!UICONTROL Send test]**.

1. Bekräfta sändningen.

   ![](assets/simulate-send-test.png)

1. Skicka så många tester som behövs tills du har slutfört innehållet i leveransen.

När du är klar kan du förbereda och skicka leveransen till huvudmålet. Läs mer i avsnitten nedan:

* [Skicka e-post](../monitor/prepare-send.md)
* [Skicka push-meddelanden](../push/send-push.md#send-push)
* [Skicka SMS-leverans](../sms/send-sms.md#send-sms)

## Åtkomst till skickade testleveranser {#access-proofs}

När testleveranserna har skickats kan du få åtkomst till dedikerade loggar från **[!UICONTROL View test log]** -knappen.

Med dessa loggar kan du få tillgång till alla tester som skickats för den valda leveransen och visualisera specifik statistik som relaterar till deras sändning. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Du kan även komma åt skickade tester via [leveranslista](../msg/gs-messages.md), som alla leveranser.

![](assets/simulate-deliveries-list.png)
