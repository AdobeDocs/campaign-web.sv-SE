---
audience: end-user
title: Skicka korrektur
description: Lär dig hur du definierar och skickar korrektur
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Skicka korrektur {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Förhandsgranskningsläge"
>abstract="Förhandsgranska och testa meddelandet genom att inkludera testpopulationen i huvudmålet."

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_proof_target"
>title="Ytterligare korrekturmål"
>abstract="Ytterligare korrekturmål."

När meddelandeinnehållet har definierats kan du förhandsgranska och testa det genom att skicka korrektur för att testa profiler. Om du har infogat anpassat innehåll kan du kontrollera hur det här innehållet visas i meddelandet med hjälp av testprofildata.

Om du vill identifiera eventuella fel i inställningarna för meddelandeinnehåll eller personalisering skickar du korrektur för att testa profiler innan du skickar dem till målgruppen. Ett korrektur ska skickas varje gång en ändring görs för att validera det senaste innehållet. Att skicka in korrektur är ett viktigt steg när det gäller att validera kampanjen och identifiera potentiella problem. Korrekturmottagarna kan kontrollera olika element som länkar, avanmälningslänkar, bilder eller spegelsidor samt upptäcka eventuella fel i återgivning, innehåll, personaliseringsinställningar och leveranskonfiguration.

## Simulera innehåll med testprofiler {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Testpopulation"
>abstract="Välj ett testpopulationsläge."

Innan du skickar ett bevis måste du definiera en målgrupp för leveransen. [Läs mer](../audience/add-audience.md)

Så här börjar du testa ditt meddelandeinnehåll:

1. Redigera innehållet i leveransen.
1. Klicka på knappen **[!UICONTROL Simulate content]**.
1. Klicka på knappen **[!UICONTROL Send proof]** för att skicka korrektur.

   ![Simulera innehållsknapp för e-posttestning](assets/simulate-test-button-email.png){zoomable="yes"}

1. Välj mottagare av korrektur.

   Beroende på meddelandekanalen kan korrektur skickas till följande typer av mottagare:

   * För SMS och e-post kan du använda [testprofiler](#test-profiles), som är specifika ytterligare mottagare i databasen. Du kan också använda läget [Ersättning från huvudmålet](#substitution-profiles), som skickar korrekturet till en e-posttestadress eller ett telefonnummer, och som använder personaliseringsdata för en befintlig profil. På så sätt kan du uppleva meddelandet som mottagarna, vilket ger dig en korrekt representation av innehållet som profilen kommer att ta emot.

   * För push-meddelanden kan du använda [prenumeranter](#subscribers), som är fiktiva prenumeranter som läggs till i databasen. De skapas i konsolen [!DNL Campaign]. Läs mer i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=sv-SE){target="_blank"}

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

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Inkludera testprofiler i huvudmålgruppen"
>abstract="Aktivera det här alternativet om du även vill skicka det sista meddelandet till korrekturmottagarna."

Testprofiler är ytterligare mottagare i databasen. De skapas från menyn **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]**. [Läs mer](../audience/test-profiles.md#create-test-profiles)

Stegen för att skicka korrektur till testprofiler beskrivs nedan.

1. Klicka på knappen **[!UICONTROL Simulate content]** och på knappen **[!UICONTROL Send proof]** från innehållet i leveransen.

1. I listrutan **[!UICONTROL Mode]** väljer du **[!UICONTROL Test profiles]** för att rikta in dig på fiktiva mottagare som ska få korrektur eller SMS-leverans.

   ![Testa profilläge](assets/simulate-profile-mode.png){zoomable="yes"}

1. Om du redan har markerat profiler för att [förhandsgranska meddelandet](preview-content.md) på skärmen för innehållssimulering, är de profilerna förmarkerade som korrekturmottagare. Du kan rensa markeringen och/eller lägga till fler mottagare med knappen **[!UICONTROL Add test profile(s)]**.

1. När du bläddrar i testprofilen eller profillistorna kan du använda filter för att förfina sökningen. Du kan till exempel definiera en regel för att hitta alla testprofiler med statusen **[!UICONTROL Prospect]**. Lär dig hur du lägger till regler med [frågemodelleraren](../query/query-modeler-overview.md).

   ![Testprofiler för filter](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Om du även vill skicka det sista meddelandet till mottagarna av korrekturet väljer du alternativet **[!UICONTROL Include test population in the main target]**.

   ![Inkludera testpopulationsalternativ](assets/simulate-include-test.png){zoomable="yes"}

1. När testprofilerna har valts kan du [skicka korrekturet](#send-test).

## Ersätt profildata {#substitution-profiles}

Använd profilersättning för att skicka korrektur till en viss e-postadress eller ett visst telefonnummer, samtidigt som data från en befintlig profil i databasen [!DNL Adobe Campaign] visas. Det här läget kan bara väljas om målgruppen för leveransen är definierad.

Om du vill ersätta profildata från huvudmålet följer du stegen nedan:

1. Klicka på knappen **[!UICONTROL Simulate content]** och på knappen **[!UICONTROL Send proof]** från innehållet i leveransen.

1. Välj **[!UICONTROL Mode]** i listrutan **[!UICONTROL Substitute from main target]** om du vill skicka ett korrektur till en viss e-postadress eller ett visst telefonnummer samtidigt som data från en befintlig profil visas.

   >[!CAUTION]
   >
   >Om du inte har valt en [målgrupp](../audience/about-recipients.md) för leveransen är alternativet **[!UICONTROL Substitute from main target]** nedtonat och du kan inte välja ersättningsprofiler. Dessutom, även om en målgrupp har valts, kommer det här alternativet fortfarande att vara nedtonat när huvudleveransen är en mall för återkommande typer av leveranser.

1. Klicka på knappen **[!UICONTROL Add address]** och ange den e-postadress eller det telefonnummer som ska ta emot korrekturet.

   ![Lägg till ersättningsadress](assets/simulate-add-substitution-address.png){zoomable="yes"}

   >[!NOTE]
   >
   >Du kan ange valfri e-postadress eller valfritt telefonnummer. Detta gör att du kan skicka korrektur till alla mottagare, även om de inte är användare av [!DNL Adobe Campaign].

1. Välj profilen från det mål som du har definierat för leveransen som ska användas som ersättning. Du kan också låta [!DNL Adobe Campaign] välja en slumpmässig profil från målet. Profildata från den valda profilen visas i korrekturet.

1. Bekräfta mottagaren och upprepa åtgärden för att lägga till så många e-postadresser eller telefonnummer som behövs.

   ![Ersätt profildata](assets/simulate-profile-substitute.png){zoomable="yes"}

1. Om du även vill skicka det sista meddelandet till mottagarna av korrekturet väljer du alternativet **[!UICONTROL Include test population in the main target]**.

1. När ersättningsprofilerna har valts kan du [skicka korrekturet](#send-test).

## Skicka korrektur till appprenumeranter {#subscribers}

När du utformar med push-meddelanden kan du bara skicka korrektur till appprenumeranterna. Följ stegen nedan för att välja dem.

1. Klicka på knappen **[!UICONTROL Simulate content]** och på knappen **[!UICONTROL Send proof]** från innehållet i din push-leverans.

   ![Simulera innehållsknappen för push-meddelanden](assets/simulate-test-button-push.png){zoomable="yes"}

1. Om du redan har valt att [förhandsgranska leveransen](preview-content.md) på skärmen för innehållssimulering, är de profilerna förvalda som testprenumeranter.

   Du kan rensa urvalet och/eller lägga till ytterligare prenumeranter med den dedikerade knappen.

   ![Lägg till testprenumeranter](assets/simulate-test-subscribers.png){zoomable="yes"}

1. Om du även vill skicka det sista push-meddelandet till testprenumeranterna väljer du alternativet **[!UICONTROL Include test population in the main target]**.

1. När prenumeranterna har valts kan du [skicka beviset](#send-test).

## Skicka korrekturet {#send-test}

Följ stegen nedan för att skicka korrekturet till de valda mottagarna.

1. Klicka på knappen **[!UICONTROL Send proof]**.

1. Bekräfta sändningen.

   ![Skicka bekräftelse på bevis](assets/simulate-send-test.png){zoomable="yes"}

1. Skicka så många korrektur som behövs tills du är klar med leveransens innehåll.

När du är klar kan du förbereda och skicka leveransen till huvudmålet. Läs mer i avsnitten nedan:

* [Skicka e-post](../monitor/prepare-send.md)
* [Skicka push-meddelanden](../push/send-push.md#send-push)
* [Skicka SMS-leverans](../sms/send-sms.md#send-sms)

## Åtkomst till skickade korrektur {#access-test-deliveries}

När korrekturen har skickats kan du komma åt deras loggar från skärmen **[!UICONTROL Simulate content]**.

Med dessa loggar kan du komma åt alla korrektur som skickats för den valda leveransen och visualisera specifik statistik som relaterar till deras sändning. [Lär dig övervaka leveransloggar](../monitor/delivery-logs.md)

![Åtkomstkorrekturloggar](assets/simulate-test-log.png){zoomable="yes"}

Du kan även komma åt skickade korrektur från [leveranslistan](../msg/gs-messages.md), precis som alla leveranser.

![Vyn Leveranslista](assets/simulate-deliveries-list.png){zoomable="yes"}