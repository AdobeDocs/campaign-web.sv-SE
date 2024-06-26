---
title: Definiera landningssidspecifikt innehåll
description: Lär dig hur du utformar innehåll för landningssidor på Campaign Web
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: 4dee53676949282b7c0e7664405b7d5a35ef64d2
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 1%

---

# Definiera landningssidspecifikt innehåll {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Använda innehållskomponenter"
>abstract="Innehållskomponenterna är tomma platshållare för innehåll som du kan använda för att skapa layouten för en landningssida. Använd formulärkomponenten för att definiera specifikt innehåll som gör att användare kan välja och skicka sina val."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definiera inställningar för den primära sidan"
>abstract="Den primära sidan visas omedelbart för användarna när de klickar på länken till din landningssida, till exempel från ett e-postmeddelande eller en webbplats."

Du kan redigera innehållet på vilken sida som helst av landningssidan.

Den första sidan, som visas omedelbart för användarna när de klickar på länken till landningssidan, är redan förfylld med [landningssidspecifik formulärkomponent](#use-form-component) för den valda mallen<!-- to enable users to select and submit their choices-->.

Innehållet i **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** och **[!UICONTROL Expiration]** sidorna är också förfyllda. Redigera dem efter behov.

Du kan också definiera [format för landningssidan](#lp-form-styles).

För att ytterligare utforma innehållet på landningssidan:

* Du kan använda samma komponenter som de som används för att utforma ett e-postmeddelande. [Läs mer](../email/content-components.md#add-content-components)

* Du kan lägga till villkorligt innehåll på dina landningssidor, på samma sätt som för ett e-postmeddelande. [Läs mer](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >Den här funktionen är begränsad tillgänglighet (LA). Den är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

## Använda formulärkomponenten {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Ange formulärkomponentfälten"
>abstract="Definiera hur dina mottagare ska se och skicka sina val från din landningssida."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Vad händer när du klickar på knappen"
>abstract="Definiera vad som ska hända när användare skickar in landningssidans formulär."

Om du vill definiera specifikt innehåll som ska göra det möjligt för användare att välja och skicka sina val från landningssidan redigerar du **[!UICONTROL Form]** -komponenten. Följ stegen nedan för att göra det.

1. Specifikt för landningssidan **[!UICONTROL Form]** -komponenten visas redan på arbetsytan för den valda mallen.

   >[!NOTE]
   >
   >The **[!UICONTROL Form]** -komponenten kan bara användas en gång på samma sida.

1. Markera den. The **[!UICONTROL Form content]** visas på den högra paletten så att du kan redigera de olika fälten i formuläret.

   ![](assets/lp-form-component.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Växla till **[!UICONTROL Styles]** när som helst för att redigera formaten för formulärkomponentens innehåll. [Läs mer](#lp-form-styles)

1. Expandera det första textfältet om det finns något, eller lägg till ett med **[!UICONTROL Add]** -knappen. Från **[!UICONTROL Text field 1]** kan du redigera fälttypen, det databasfält som ska uppdateras, etiketten och texten som ska visas i fältet innan användaren anger ett värde.

   ![](assets/lp-form-text-field.png){zoomable=&quot;yes&quot;}

1. Markera **[!UICONTROL Make form field mandatory]**-alternativet om det behövs.  I så fall kan landningssidan endast skickas om användaren har fyllt i detta fält.

   >[!NOTE]
   >
   >Om ett obligatoriskt fält inte är ifyllt visas ett felmeddelande när användaren skickar sidan.

1. Expandera eventuella kryssrutor eller lägg till en med **[!UICONTROL Add]** -knappen. Välj om kryssrutan ska uppdatera en tjänst eller ett fält från databasen.

   ![](assets/lp-form-checkbox.png){zoomable=&quot;yes&quot;}

   Om du väljer **[!UICONTROL Subscription & services]** väljer du en [service](../audience/manage-services.md) i listan och välj mellan de två alternativen nedan:

   * **[!UICONTROL Subscribe in if checked]**: Användarna måste markera kryssrutan för att godkänna (anmälan).
   * **[!UICONTROL Unsubscribe if checked]**: Användarna måste markera kryssrutan för att ta bort sitt samtycke (avanmälan).

   Om du väljer **[!UICONTROL Field]** markerar du ett fält i attributlistan och väljer mellan de två alternativen nedan:

   * **[!UICONTROL Yes if checked]**.<!--TBC-->

   * **[!UICONTROL No if checked]**.<!--TBC-->

1. Du kan ta bort och lägga till så många fält (t.ex. textfält, alternativknappar, kryssrutor, listrutor) efter behov.

1. När alla fält har lagts till eller uppdaterats klickar du på **[!UICONTROL Call to action]** för att expandera motsvarande avsnitt. Här kan du definiera hur knappen ska fungera i **[!UICONTROL Form]** -komponenten. [Lär dig mer](#define-actions-on-form-submission)

   ![](assets/lp-call-to-action.png){zoomable=&quot;yes&quot;}

1. Spara innehållet för att gå tillbaka till [egenskaper för landningssida](create-lp.md#create-landing-page).

### Definiera åtgärder när formulär skickas {#define-actions-on-form-submission}

1. Definiera vad som ska hända när du klickar på knappen:

   * **[!UICONTROL Confirmation page]**: Som standard omdirigeras användaren till **[!UICONTROL Confirmation]** siduppsättning för den aktuella landningssidan.

   * **[!UICONTROL Redirect URL]**: Ange URL-adressen till sidan som användarna ska omdirigeras till.

   * **[!UICONTROL Landing page]**: Du kan välja en annan landningssida som användare kan omdirigeras till. Kontrollera att du har konfigurerat den valda landningssidan i enlighet med detta.

1. Om du vill göra ytterligare uppdateringar när du skickar formuläret väljer du **[!UICONTROL Additional updates]** och markera det objekt som du vill uppdatera:
   * En prenumeration [service](../audience/manage-services.md) - i så fall, ange om du vill avanmäla dig eller avanmäla användare när du skickar formuläret. Om du definierar en **[!UICONTROL Landing page]**-type link to this landing page, the selected service will be automatically used. [Läs mer om att infoga länkar](../email/message-tracking.md)

     >[!NOTE]
     >
     >Använd **[!UICONTROL Service from URL]** som beskrivs nedan.

   * Kanalen - e-postadressen som användes när formuläret fylldes i.
   * Alla kanaler - när formuläret skickas in väljs användarna in eller ut (beroende på den valda mallen) till/från all kommunikation från ert varumärke i alla kanaler.
   * Ett fält från databasen - välj ett fält i attributlistan och definiera om det ska anges som Sant eller Falskt när formuläret skickas.

   ![](assets/lp-form-additionnal-updates.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Service from URL]** möjlighet att låta landningssidan användas för flera tjänster, så att den blir dynamisk. Definiera om du vill avanmäla dig eller avanmäla användare när du skickar formuläret.

   >[!AVAILABILITY]
   >
   >Den här funktionen är begränsad tillgänglighet (LA). Den är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

   ![](assets/lp-form-service-from-url.png){zoomable=&quot;yes&quot;}

   Om du definierar en **[!UICONTROL Landing page]**-type link to this landing page, you will be able all service from the list. Du kan sedan välja andra tjänster när du definierar andra länkar till den här landningssidan. [Läs mer om att infoga länkar](../email/message-tracking.md)

   ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

## Definiera format för landningssidor {#lp-form-styles}

1. Om du vill ändra formaten för formulärkomponentens innehåll växlar du när som helst till **[!UICONTROL Styles]** -fliken.

1. The **[!UICONTROL Text field]** -avsnittet är som standard utökat. Du kan redigera utseendet på textfälten, t.ex. etikettens teckensnitt, placeringen av etiketten, fältets bakgrundsfärg eller fältets kantlinje.

   ![](assets/lp-text-styles.png){zoomable=&quot;yes&quot;}

1. Expandera **[!UICONTROL Checkbox]** för att definiera utseendet på kryssrutorna och motsvarande text. Du kan till exempel justera teckensnittsfamiljen och storleken eller kryssrutans kantlinjefärg.

   ![](assets/lp-checkbox-style.png){zoomable=&quot;yes&quot;}

1. Utöka och redigera andra avsnitt som motsvarar andra fält som du har lagt till (alternativknapp, listruta, datum och tid osv.) till formuläret.

1. Expandera **[!UICONTROL Call to action]** för att ändra utseendet på knappen i komponentformuläret. Du kan till exempel ändra teckensnitt, lägga till en kant, redigera etikettfärgen vid hovring eller justera justeringen av knappen.

   ![](assets/lp-call-to-action-style.png){zoomable=&quot;yes&quot;}

   Du kan förhandsgranska vissa inställningar, t.ex. knappetikettfärg vid hovring med hjälp av **[!UICONTROL Simulate content]** -knappen. [Läs mer](create-lp.md#test-landing-page)

1. Spara ändringarna.
