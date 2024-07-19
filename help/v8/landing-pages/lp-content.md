---
title: Definiera landningssidspecifikt innehåll
description: Lär dig hur du utformar innehåll för landningssidor på Campaign Web
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: 4dee53676949282b7c0e7664405b7d5a35ef64d2
workflow-type: tm+mt
source-wordcount: '1067'
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

Den första sidan, som visas omedelbart för användarna när de klickar på länken till landningssidan, är redan ifylld med den [landningssidsspecifika formulärkomponenten](#use-form-component) för den valda mallen<!-- to enable users to select and submit their choices-->.

Innehållet på sidorna **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** och **[!UICONTROL Expiration]** är också förifyllt. Redigera dem efter behov.

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

Om du vill definiera specifikt innehåll som gör att användare kan välja och skicka sina val från din landningssida redigerar du komponenten **[!UICONTROL Form]**. Följ stegen nedan för att göra det.

1. Den landningssidspecifika **[!UICONTROL Form]**-komponenten visas redan på arbetsytan för den valda mallen.

   >[!NOTE]
   >
   >Komponenten **[!UICONTROL Form]** kan bara användas en gång på samma sida.

1. Markera den. Fliken **[!UICONTROL Form content]** visas på den högra paletten så att du kan redigera de olika fälten i formuläret.

   ![](assets/lp-form-component.png){zoomable="yes"}

   >[!NOTE]
   >
   >Växla till fliken **[!UICONTROL Styles]** när du vill om du vill redigera formaten för formulärkomponentinnehållet. [Läs mer](#lp-form-styles)

1. Expandera det första textfältet om det finns något, eller lägg till ett med knappen **[!UICONTROL Add]**. I avsnittet **[!UICONTROL Text field 1]** kan du redigera fälttypen, det databasfält som ska uppdateras, etiketten och texten som ska visas i fältet innan användarna anger ett värde.

   ![](assets/lp-form-text-field.png){zoomable="yes"}

1. Markera **[!UICONTROL Make form field mandatory]**-alternativet om det behövs.  I så fall kan landningssidan endast skickas om användaren har fyllt i detta fält.

   >[!NOTE]
   >
   >Om ett obligatoriskt fält inte är ifyllt visas ett felmeddelande när användaren skickar sidan.

1. Expandera eventuella kryssrutor eller lägg till en med knappen **[!UICONTROL Add]**. Välj om kryssrutan ska uppdatera en tjänst eller ett fält från databasen.

   ![](assets/lp-form-checkbox.png){zoomable="yes"}

   Om du väljer **[!UICONTROL Subscription & services]** väljer du en [tjänst](../audience/manage-services.md) i listan och väljer mellan de två alternativen nedan:

   * **[!UICONTROL Subscribe in if checked]**: Användarna måste markera kryssrutan för att godkänna (anmälan).
   * **[!UICONTROL Unsubscribe if checked]**: Användarna måste markera kryssrutan för att ta bort sitt samtycke (avanmälan).

   Om du väljer **[!UICONTROL Field]** markerar du ett fält i attributlistan och väljer mellan de två alternativen nedan:

   * **[!UICONTROL Yes if checked]**.<!--TBC-->

   * **[!UICONTROL No if checked]**.<!--TBC-->

1. Du kan ta bort och lägga till så många fält (t.ex. textfält, alternativknappar, kryssrutor, listrutor) efter behov.

1. När alla fält har lagts till eller uppdaterats klickar du på **[!UICONTROL Call to action]** för att expandera motsvarande avsnitt. Det gör att du kan definiera beteendet för knappen i komponenten **[!UICONTROL Form]**. [Lär dig hur](#define-actions-on-form-submission)

   ![](assets/lp-call-to-action.png){zoomable="yes"}

1. Spara ditt innehåll för att gå tillbaka till [landningssidans egenskaper](create-lp.md#create-landing-page).

### Definiera åtgärder när formulär skickas {#define-actions-on-form-submission}

1. Definiera vad som ska hända när du klickar på knappen:

   * **[!UICONTROL Confirmation page]**: Som standard omdirigeras användaren till siduppsättningen **[!UICONTROL Confirmation]** för den aktuella landningssidan.

   * **[!UICONTROL Redirect URL]**: Ange URL-adressen till sidan som användarna ska omdirigeras till.

   * **[!UICONTROL Landing page]**: Du kan välja en annan landningssida som användare kan omdirigeras till. Kontrollera att du har konfigurerat den valda landningssidan i enlighet med detta.

1. Om du vill göra ytterligare uppdateringar när du skickar formuläret väljer du **[!UICONTROL Additional updates]** och markerar det objekt som du vill uppdatera:
   * En prenumeration på [tjänst](../audience/manage-services.md) - i så fall, definiera om du vill avanmäla dig eller avanmäla användare när du skickar formuläret. Om du definierar en länk av typen **[!UICONTROL Landing page]** till den här landningssidan när du utformar ett e-postmeddelande används den valda tjänsten automatiskt. [Läs mer om att infoga länkar](../email/message-tracking.md)

     >[!NOTE]
     >
     >Om du vill använda flera tjänster med den här landningssidan använder du alternativet **[!UICONTROL Service from URL]** som beskrivs nedan.

   * Kanalen - e-postadressen som användes när formuläret fylldes i.
   * Alla kanaler - när formuläret skickas in väljs användarna in eller ut (beroende på den valda mallen) till/från all kommunikation från ert varumärke i alla kanaler.
   * Ett fält från databasen - välj ett fält i attributlistan och definiera om det ska anges som Sant eller Falskt när formuläret skickas.

   ![](assets/lp-form-additionnal-updates.png){zoomable="yes"}

1. Välj alternativet **[!UICONTROL Service from URL]** om du vill tillåta att landningssidan används för flera tjänster, vilket gör den dynamisk. Definiera om du vill avanmäla dig eller avanmäla användare när du skickar formuläret.

   >[!AVAILABILITY]
   >
   >Den här funktionen är begränsad tillgänglighet (LA). Den är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

   ![](assets/lp-form-service-from-url.png){zoomable="yes"}

   Om du definierar en länk av typen **[!UICONTROL Landing page]** till den här landningssidan när du utformar ett e-postmeddelande kan du välja vilken tjänst som helst i listan. Du kan sedan välja andra tjänster när du definierar andra länkar till den här landningssidan. [Läs mer om att infoga länkar](../email/message-tracking.md)

   ![](assets/email-link-to-landing-page.png){zoomable="yes"}

## Definiera format för landningssidor {#lp-form-styles}

1. Om du vill ändra formaten för formulärkomponentinnehållet växlar du när som helst till fliken **[!UICONTROL Styles]**.

1. Avsnittet **[!UICONTROL Text field]** är expanderat som standard. Du kan redigera utseendet på textfälten, t.ex. etikettens teckensnitt, placeringen av etiketten, fältets bakgrundsfärg eller fältets kantlinje.

   ![](assets/lp-text-styles.png){zoomable="yes"}

1. Expandera avsnittet **[!UICONTROL Checkbox]** för att definiera utseendet på kryssrutorna och motsvarande text. Du kan till exempel justera teckensnittsfamiljen och storleken eller kryssrutans kantlinjefärg.

   ![](assets/lp-checkbox-style.png){zoomable="yes"}

1. Utöka och redigera andra avsnitt som motsvarar andra fält som du har lagt till (alternativknapp, listruta, datum och tid osv.) till formuläret.

1. Expandera avsnittet **[!UICONTROL Call to action]** om du vill ändra utseendet på knappen i komponentformuläret. Du kan till exempel ändra teckensnitt, lägga till en kant, redigera etikettfärgen vid hovring eller justera justeringen av knappen.

   ![](assets/lp-call-to-action-style.png){zoomable="yes"}

   Du kan förhandsgranska vissa inställningar, till exempel knappetikettsfärg vid hovring, med knappen **[!UICONTROL Simulate content]**. [Läs mer](create-lp.md#test-landing-page)

1. Spara ändringarna.
