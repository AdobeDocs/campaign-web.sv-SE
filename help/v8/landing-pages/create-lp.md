---
title: Skapa en landningssida
description: Lär dig konfigurera och publicera en landningssida på Campaign Web
feature: Landing Pages
exl-id: d4a49048-5ab1-4b69-9e12-1ffa235c51f4
source-git-commit: e82c19df7faecbb75521bca54e32b1ba84ea1f81
workflow-type: tm+mt
source-wordcount: '1544'
ht-degree: 1%

---


# Skapa och publicera landningssidor {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Skapa och hantera landningssidor"
>abstract="Med Adobe Campaign kan du skapa, designa och dela landningssidor för att dirigera dina användare till webbsidor på webben där du kan hantera kundvärvning, prenumeration/avprenumeration och blocklist användningsfall, baserat på inbyggda mallar."

Med användargränssnittet för Campaign-webben kan du skapa, designa och publicera landningssidor. Efter publiceringen kan du infoga en länk till formuläret i en leverans. När mottagarna klickar på länken dirigeras de till motsvarande landningssida.

[!DNL Adobe Campaign] innehåller fyra mallar för att hantera följande användningsfall: **förvärv**, **prenumeration**, **unsubscription** och **blockeringslista**. [Läs mer](lp-use-cases.md)

## Åtkomst till landningssidor {#access-landing-pages}

Välj **[!UICONTROL Content management]** > **[!UICONTROL Landing pages]** på den vänstra menyn för att komma åt landningssidans lista.

![Skärmbild som visar landningssidornas lager i webbgränssnittet för Campaign.](assets/lp-inventory.png){zoomable="yes"}

Lagret **[!UICONTROL Landing pages]** visar alla skapade artiklar. Du kan filtrera dem med knappen **[!UICONTROL Show filters]**.

* Du kan filtrera objekt som du har skapat eller ändrat.
* Du kan begränsa resultaten till en viss [mapp](../get-started/permissions.md#folders) med hjälp av listrutan eller lägga till regler med [frågemodelleraren](../query/query-modeler-overview.md).

![Skärmbild som visar filteralternativen i lagret för landningssidor.](assets/lp-inventory-filter.png){zoomable="yes"}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Du kan inte visa eller redigera landningssidor som skapats från klientkonsolen (webbformulär) i gränssnittet för Campaign-webben. Läs mer i dokumentationen för [Campaign-konsolen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=sv-SE){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Du kan duplicera eller ta bort en landningssida. Klicka på ellipsen bredvid en landningssida för att välja önskad åtgärd.

## Skapa en landningssida {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definiera egenskaperna för landningssidan"
>abstract="Fyll i egenskapsfälten, till exempel etiketten, och ändra schemat om det behövs. Dessutom kan du redigera det interna namnet, ändra mappen där landningssidan lagras och ange en beskrivning."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Definiera innehållet på varje sida"
>abstract="Justera innehållet på varje sida som är en del av landningssidan, t.ex. själva formuläret, bekräftelsesidan som visas när formuläret skickas eller så dirigeras sidanvändarna till om ett fel inträffar."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Schemalägg din landningssida"
>abstract="Definiera startdatum och slutdatum för landningssidan. När sidan når slutet av giltighetsperioden är formuläret inte längre tillgängligt. Sidan **Förfallotid** visas i stället."

>[!CONTEXTUALHELP]
>id="acw_landingpages_preload"
>title="Definiera förinläsningsalternativ"
>abstract="När alternativet **Förifyll med data som refereras till i formuläret** har valts och om besökaren på landningssidan matchar en profil från databasen, förinläses profilinformationen automatiskt i formuläret. När alternativet **Godkänn frånvaro av ID** har valts kan alla besökare, inklusive anonyma användare, få åtkomst till landningssidan."

<!--With the **Skip preloading if no ID** option selected, each profile entered will be added to the database after approval of the form."-->

>[!CONTEXTUALHELP]
>id="acw_landingpages_storage"
>title="Definiera lagringsalternativ"
>abstract="I avsnittet med förinläsning kan du ange hur du ska hitta den post som ska uppdateras i databasen."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

Så här skapar du en landningssida:

1. Klicka på **[!UICONTROL Landing pages]** i **[!UICONTROL Create landing page]**-lagret.

   ![Skärmbild som visar knappen Skapa landningssida.](assets/lp-create-button.png){zoomable="yes"}

1. Välj en mall:
   * **[!UICONTROL Acquisition]**: Det här är standardmallen för landningssidor, som gör att du kan hämta och uppdatera profildata.
   * **[!UICONTROL Subscription]**: Använd den här mallen om du vill att användare ska kunna prenumerera på en viss [tjänst](../audience/manage-services.md).
   * **[!UICONTROL Unsubscription]**: Den här mallen kan användas i en leverans som skickas till prenumeranterna av en tjänst, så att de kan avbryta prenumerationen på den här [tjänsten](../audience/manage-services.md).
   * **[!UICONTROL Denylist]**: Den här mallen ska användas när en profil klickar på en länk för avanmälan i en leverans och inte längre vill bli kontaktad.

   ![Skärmbild som visar startsidans mallar.](assets/lp-templates.png){zoomable="yes"}

   >[!NOTE]
   >
   >Lär dig hur du implementerar de olika användningsfall som motsvarar varje mall på [den här sidan](lp-use-cases.md).

1. Klicka på **[!UICONTROL Create]**.

1. Fyll i fälten **[!UICONTROL Properties]**, till exempel etiketten.

   Som standard lagras landningssidor i mappen **[!UICONTROL Web applications]**. Du kan ändra den genom att bläddra till önskad plats i **[!UICONTROL Additional options]**. [Lär dig arbeta med mappar](../get-started/permissions.md#folders).

   Du kan också konfigurera captcha för att skydda din landningssida. [Läs mer här](#captcha).

   ![Skärmbild som visar egenskapssektionen för landningssidan.](assets/lp-properties.png){zoomable="yes"}

1. Följande alternativ är tillgängliga i avsnittet **[!UICONTROL Data preload]**:

   * När alternativet **[!UICONTROL Pre-fill with the data referenced in the form]** har valts och besökaren på landningssidan matchar en profil från databasen, förinläses profilinformationen automatiskt i formuläret. Användaren behöver bara fylla i de saknade fälten och uppdatera de befintliga värdena om det behövs. Detta gör att du kan sammanfoga data för befintliga profiler i stället för att skapa dubbletter.

     >[!NOTE]
     >
     >Det här alternativet är markerat som standard för alla mallar för landningssidor.

   * Alternativet **[!UICONTROL Authorize absence of ID]** ger alla besökare åtkomst till landningssidan. Om du avmarkerar det här alternativet hindras anonyma besökare från att använda det, vilket innebär att endast identifierade användare kan komma åt och skicka formuläret.

     För mallarna **[!UICONTROL Acquisition]** och **[!UICONTROL Subscription]** är det här alternativet valt som standard. För mallarna **[!UICONTROL Unsubscription]** och **[!UICONTROL Denylist]** är det här alternativet omarkerat som standard och kan inte ändras.

1. En landningssida kan ha efterföljande sidor. Om du vill lägga till sidor bläddrar du i avsnittet **[!UICONTROL Pages]** och klickar på knappen **[!UICONTROL Edit content]** för varje sida som du vill designa för den här landningssidan. Innehållet på varje sida är redan förfyllt. Redigera dem efter behov. [Läs mer](lp-content.md).

   ![Skärmbild som visar sidavsnittet i landningssidans redigerare.](assets/lp-pages.png){zoomable="yes"}

1. I avsnittet **[!UICONTROL Storage]** är alternativet **[!UICONTROL Update the preloaded record]** markerat som standard. Det gör det möjligt att uppdatera de profiler som lagras i databasen via landningssidan. I rutan för förinläsning kan du ange hur posten ska uppdateras i databasen.

   Du kan också välja bland fälten i den aktuella kontexten på landningssidan, de som ska användas för att hitta motsvarande profil i databasen. Om du vill göra det avmarkerar du alternativet **[!UICONTROL Update the preloaded record]** och kontrollerar fälten under **[!UICONTROL Reconciliation options]**.

   ![Skärmbild som visar lagringsalternativen för landningssidan.](assets/lp-storage.png){zoomable="yes"}

1. Skapa **[!UICONTROL Additional data]** för att lagra interna data när landningssidan skickas. Informationen är inte synlig för användare som besöker sidan. Endast konstanta värden tas i beaktning.

   ![Skärmbild som visar ytterligare dataavsnitt.](assets/lp-additional-data.png){zoomable="yes"}

1. Du kan definiera ett startdatum och ett slutdatum för landningssidan. Välj **[!UICONTROL Enable scheduling]** och ange datum.

   ![Skärmbild med schemaläggningsalternativ för landningssidan.](assets/lp-schedule.png){zoomable="yes"}

   * Landningssidan publiceras automatiskt på det angivna startdatumet/den angivna starttiden.

     >[!NOTE]
     >
     >Om inget startdatum definieras blir landningssidan live så snart den har publicerats.

   * När sidan når slutdatumet är formuläret inte längre tillgängligt. Sidan **[!UICONTROL Expiration]** visas i stället.

     >[!NOTE]
     >
     >Adobe rekommenderar att du anger ett slutdatum av säkerhetsskäl och av plattformsprestanda.

1. Klicka på **[!UICONTROL Review and publish]**.

När du har definierat alla inställningar och [designat](lp-content.md) alla sidor kan du [testa](#test-landing-page) och [publicera](#publish-landing-page) din landningssida enligt anvisningarna nedan.

## Skydda din landningssida med en captcha {#captcha}

Genom att konfigurera en captcha kan du skydda din landningssida mot skräppost och missbruk.

Om du vill använda den går du till **[!UICONTROL Properties]** på landningssidan.
I **[!UICONTROL Additional options]** också. Aktivera växeln **[!UICONTROL Additional Enable captcha solution]**.

![Skärmbild som visar växlingen för Additional Enable captcha solution](assets/lp-properties-captcha.png){zoomable="yes"}

Om du vill kontrollera bildspelsinställningarna klickar du på knappen **[!UICONTROL Review and publish]** och **[!UICONTROL Simulate content]**. När du skickar formuläret ser du att widgeten Capture fungerar under valideringen enligt nedan.

![Skärmbild av captcha-widgeten](assets/lp-captcha.png){zoomable="yes"}

>[!NOTE]
>
>Captcha-widgeten i Adobe Campaign v8 är ALTCHA i flytande läge. Det visas under valideringen och försvinner när processen är klar.


## Testa landningssidan {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulera landningssidan"
>abstract="Du kan se en förhandsgranskning av landningssidan i gränssnittet för webben i Campaign eller öppna den på en ny webbläsarflik."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Förhandsgranska och testa landningssidan"
>abstract="När du har definierat inställningarna för landningssidan och innehållet kan du använda testprofiler för att förhandsgranska den."

När inställningarna för landningssidan och innehållet har definierats kan du använda testprofiler för att förhandsgranska den. Om du infogade [anpassat innehåll](../personalization/gs-personalization.md) kan du med hjälp av testprofildata kontrollera hur det här innehållet visas på landningssidan.

>[!CAUTION]
>
>Du måste ha testprofiler tillgängliga för att kunna förhandsgranska dina meddelanden och skicka korrektur. [Läs mer om testprofiler](../audience/test-profiles.md)

Så här testar du landningssidan:

1. När du har klickat på **[!UICONTROL Review and publish]** väljer du knappen **[!UICONTROL Simulate content]** på kontrollpanelen för landningssidan för att komma åt valet av testprofil.

   ![Skärmbild av knappen Simulera innehåll](assets/lp-simulate-content.png){zoomable="yes"}

1. Välj en eller flera testprofiler på skärmen **[!UICONTROL Simulate]**.

   Stegen för att välja testprofiler är desamma som när du testar ett meddelande. De beskrivs i avsnittet [Förhandsgranska och testa](../preview-test/preview-test.md).

1. När du testar en dynamisk landningssida (med alternativet **[!UICONTROL Service from URL]** markerat - [läs mer](../landing-pages/create-lp.md#define-actions-on-form-submission))

1. Välj **[!UICONTROL Open preview]** om du vill testa landningssidan.

   ![Skärmbild av knappen Öppna förhandsvisning](assets/lp-open-preview.png){zoomable="yes"}

1. Förhandsgranskningen av landningssidan öppnas på en ny flik. Personaliserade element ersätts med valda testprofildata.

   Om du valde alternativet **[!UICONTROL Pre-fill with the data referenced in the form]** i inställningarna för landningssidan fylls formulärfälten automatiskt i med motsvarande testprofildata.<!--TBC-->

   ![Exempel på leverans](assets/lp-preview.png){zoomable="yes"}

1. Välj andra testprofiler om du vill förhandsgranska återgivningen för varje variant av landningssidan.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publicera landningssidan {#publish-landing-page}

När landningssidan är klar och validerad publicerar du den för att göra den tillgänglig för användning i en leverans med motsvarande knapp.

Publicerad:

* Landningssidan läggs till i listan över landningssidor med statusen **[!UICONTROL Published]**. Den är nu live och klar att refereras till i innehållet.

* Du kan kopiera och klistra in **[!UICONTROL Landing page URL]** som visas överst på sidan i en webbläsare för att förhandsgranska din startsida.

>[!CAUTION]
>
>Om du vill testa eller utnyttja landningssidan fullt ut kan du inte kopiera och klistra in länken direkt i en webbläsare eller i leveranser. Använd i stället funktionen [Simulera innehåll](#test-landing-page) för att testa det och följ stegen som beskrivs i [det här avsnittet](lp-use-cases.md) för att använda landningssidan på rätt sätt.

![Skärmbild som visar URL för landningssida](assets/lp-published.png){zoomable="yes"}

Du kan övervaka landningssidans påverkan via loggarna <!--and specific reports-->. Klicka på knappen **[!UICONTROL Logs]**.