---
solution: Journey Optimizer
product: journey optimizer
title: Användningsexempel för landningssida
description: Upptäck de vanligaste användningsområdena med landningssidor i Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: landning, landningssida, fallstudie
exl-id: 8c00d783-54a3-45d9-bd8f-4dc58804d922
source-git-commit: 601cc62c5640069ce9e6ee4830f924c610e0915f
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Använda en landningssida {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Kopiera URL med försiktighet"
>abstract="Om du vill testa eller utnyttja landningssidan fullt ut kan du inte kopiera och klistra in länken direkt i en webbläsare eller i leveranser. Använd i stället **Simulera innehåll** för att testa den och följa de steg som beskrivs i dokumentationen för att använda landningssidan på rätt sätt."

Om du vill använda landningssidan på rätt sätt bör du referera till den som en länk i en leverans med det dedikerade alternativet.

>[!CAUTION]
>
>Om du vill utnyttja din landningssida fullt ut kan du inte kopiera och klistra in länken som visas på den publicerade kontrollpanelen för leverans direkt på leveransen eller till en webbsida.

I [!DNL Adobe Campaign Web] fyra färdiga mallar gör det möjligt att implementera olika användningsområden. Huvudstegen är dock fortfarande desamma och beskrivs nedan.

1. [Skapa en landningssida](create-lp.md#create-landing-page) och välj en mall beroende på ditt användningssätt:

   * [Förvärv](#lp-acquisition)
   * [Prenumeration](#lp-subscription)
   * [Avsluta prenumeration](#lp-unsubscription)
   * [Blockeringslista](#lp-denylist)

1. Definiera egenskaper och inställningar för landningssidan.

   ![](assets/lp-uc-properties.png)

1. Välj **[!UICONTROL Acquisition]**, **[!UICONTROL Subscription]**, **[!UICONTROL Unsubscription]** eller **[!UICONTROL Denylist]** sida.

1. Sidans innehåll visas. Markera den del som motsvarar landningssidans formulär.

   ![](assets/lp-uc-form.png)

1. Gör så många andra uppdateringar av landningssidans etiketter och fält som behövs. Redigera resten av materialet som du vill, spara ändringarna och stäng det.

1. Följ stegen nedan för varje användningsfall.

1. Redigera **[!UICONTROL Confirmation]** sida efter behov, samt **[!UICONTROL Error]** och **[!UICONTROL Expiration]** sidor. Den visas för mottagarna när de har skickat in registreringsformuläret.

   ![](assets/lp-uc-confirmation-page.png)

1. Testa och [publicera](create-lp.md#publish-landing-page) din landningssida.

1. Skapa en [e-post](../email/create-email.md) leverans för att köra trafik till landningssidan.

1. [Infoga en länk](../email/message-tracking.md#insert-links) i ert meddelandeinnehåll. Välj **[!UICONTROL Landing page]** som **[!UICONTROL Link type]** och väljer [landningssida](create-lp.md#configure-primary-page) som du skapade.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Om du vill kunna skicka ditt meddelande kontrollerar du att landningssidan du valt inte har gått ut ännu. Lär dig hur du uppdaterar förfallodatumet [i det här avsnittet](create-lp.md#create-landing-page).

När mottagarna har fått e-postmeddelandet klickar du på länken till landningssidan och skickar landningssidans formulär, dirigeras de till bekräftelsesidan och eventuella andra åtgärder som definieras på landningssidan tillämpas (till exempel kommer användarna att prenumerera på din tjänst eller kommer inte att få mer information från dig).

Nedan finns några exempel på hur du kan använda [!DNL Adobe Campaign] landningssidor så att dina kunder kan välja att inte ta emot vissa eller alla meddelanden.

## Profilinsamling {#lp-acquisition}

1. [Skapa en landningssida](create-lp.md#create-landing-page). Välj **[!UICONTROL Acquisition]** mall.

1. Definiera egenskaper och inställningar för landningssidan.

   ![](assets/lp-uc-properties.png)

1. Välj **[!UICONTROL Acquisition]** sida för att redigera innehållet.

1. Sidans innehåll visas. Markera den del som motsvarar landningssidans formulär.

## Prenumeration på en tjänst {#lp-subscription}

Ett av de vanligaste användningsområdena är att bjuda in kunderna till [prenumerera på en tjänst](../audience/manage-services.md) (till exempel ett nyhetsbrev eller ett evenemang) via en landningssida. Följ stegen nedan.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Börja med att skapa en bekräftelsemall för användare som prenumererar på ditt evenemang, så att du enkelt kan välja det när du skapar tjänsten. [Läs mer](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. Skapa en prenumerationstjänst som lagrar registrerade användare till ditt evenemang. [Lär dig skapa en tjänst](../audience/manage-services.md)

1. Välj den mall som du skapade som det bekräftelsemeddelande som användarna får när de prenumererar.

   ![](assets/lp-uc-subscription-service.png)

1. [Skapa en landningssida](create-lp.md#create-landing-page) för att göra det möjligt för mottagarna att registrera sig för evenemanget. Välj **[!UICONTROL Subscription]** mall.

   <!--![](assets/lp-uc-subscription-template.png)-->

1. Definiera egenskaper och inställningar för landningssidan.

   <!--![](assets/lp-uc-properties.png)-->

1. Välj **[!UICONTROL Subscription]** sida för att redigera innehållet.

   ![](assets/lp-uc-subscription-page-edit.png)

1. Sidans innehåll visas. Markera den del som motsvarar landningssidans formulär och utöka **[!UICONTROL Checkbox 1]** -avsnitt.

   I **[!UICONTROL Subscriptions & services]** markerar du den tjänst du skapade för evenemanget. Lämna **[!UICONTROL Subscribe if checked]** aktiverat alternativ.

   ![](assets/lp-uc-subscription-checkbox-1.png)

1. Du kan till exempel lägga till ytterligare en kryssruta för att erbjuda prenumerationer i nyhetsbrevet.

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. Gör så många andra uppdateringar av landningssidans etiketter och fält som behövs. Redigera resten av materialet som du vill, spara ändringarna och stäng det.

1. Redigera **[!UICONTROL Confirmation]** sida efter behov, samt **[!UICONTROL Error]** och **[!UICONTROL Expiration]** sidor. Den visas för mottagarna när de har skickat in registreringsformuläret.

   ![](assets/lp-uc-confirmation-page.png)

1. Testa och [publicera](create-lp.md#publish-landing-page) din landningssida.

1. Skapa en **E-post** leverans för att köra trafik till landningssidan för registrering. Designa e-postmeddelandet för att meddela att registreringen nu är öppen för ditt event.

1. [Infoga en länk](../email/message-tracking.md#insert-links) i ert meddelandeinnehåll. Välj **[!UICONTROL Landing page]** som **[!UICONTROL Link type]** och väljer [landningssida](create-lp.md#configure-primary-page) som du har skapat för registrering.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Om du vill kunna skicka ditt meddelande kontrollerar du att landningssidan du valt inte har gått ut ännu. Lär dig hur du uppdaterar förfallodatumet [i det här avsnittet](create-lp.md#create-landing-page).

När mottagarna har fått e-postmeddelandet och klickar på länken till landningssidan och skickar landningssidans formulär dirigeras de till bekräftelsesidan och läggs till i prenumerationslistan.

## Avsluta prenumeration {#lp-unsubscription}

1. [Skapa en landningssida](create-lp.md#create-landing-page). Välj **[!UICONTROL Unsubscription]** mall.

1. Definiera egenskaper och inställningar för landningssidan.

1. Välj **[!UICONTROL Unsubscription]** sida för att redigera innehållet.

1. Sidans innehåll visas. Markera den del som motsvarar landningssidans formulär.

## Konfigurera landningssidor för avanmälan {#lp-denylist}

Att ge mottagarna möjlighet att avbryta prenumerationen på information från ett varumärke är ett juridiskt krav. Läs mer om gällande lagstiftning i [Experience Platform dokumentation](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html#regulations){target="_blank"}.

Därför måste du alltid inkludera en **avbeställ länk** i varje e-postmeddelande som skickas till mottagarna:

* När du klickar på den här länken dirigeras mottagarna till en landningssida med en knapp som bekräftar att de avanmäler sig.
* När du klickar på avanmälningsknappen uppdateras profildata med den här informationen.

Du kan konfigurera en **[!UICONTROL Denylist]** landningssida som gör det möjligt för användare att välja bort alla leveranser.

Om du vill att användarna ska kunna välja bort alla leveranser måste du skapa och publicera en **[!UICONTROL Denylist]** landningssida.

När en användare klickar på landningssidans länk visas **[!UICONTROL No longer contact (by any channel)]** i profilen väljs automatiskt.

![](assets/blocklisting_allchannels.png)

definiera **[!UICONTROL Opt-out]** kryssruta och välj att uppdatera **[!UICONTROL Channel (email)]**: den profil som kontrollerar avanmälningsrutan på din landningssida avvisas från all kommunikation.

När meddelandet har tagits emot visas din startsida om en mottagare klickar på länken för att avbryta prenumerationen i e-postmeddelandet.

![](assets/lp_opt-out-submit-form.png)

Om mottagaren markerar rutan och skickar formuläret:

* Mottagaren omdirigeras till bekräftelsemeddelandeskärmen.

* Profildata uppdateras och kommer inte att få information från ert varumärke om ni inte prenumererar igen.

Om du vill kontrollera att den aktuella profilens val har uppdaterats går du till Profiler och väljer profilen.







