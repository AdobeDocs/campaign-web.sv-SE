---
audience: end-user
title: Redigera e-postinnehållet
description: Lär dig hur du redigerar e-postinnehållet i användargränssnittet för Campaign Web
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# Konfigurera e-postinnehållet {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definiera e-postinnehållet"
>abstract="The **Redigera innehåll** kan du definiera grundläggande element i meddelandet, t.ex. avsändarens adress och ämnesrad, utföra ytterligare åtgärder som att lägga till bilagor eller erbjudanden samt komma åt e-post-Designer för att ge meddelandet ett snyggt utseende."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Ange e-postegenskaper"
>abstract="The **Grundläggande information** I kan du uppdatera avsändarens adress och svarsadress och definiera ämnesraden med hjälp av uttrycksredigeraren."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Bifoga filer i e-postmeddelandet"
>abstract="Markera en eller flera filer som ska infogas i meddelandet. För att undvika prestandaproblem rekommenderar vi att du inte inkluderar mer än en bifogad fil per e-post."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Redigeringsspårning"
>abstract="Spårning är aktiverat som standard för leverans, vilket innebär att alla länkar som ingår i meddelandeinnehållet spåras. Du kan inaktivera det här alternativet härifrån."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/email/content/design-content/message-tracking.html" text="Lägga till länkar och spåra meddelanden"

E-postmeddelandet **[!UICONTROL Edit content]** kan du göra följande:

* Definiera grundläggande element i meddelandet, t.ex. avsändarens adress och ämnesraden
* Utför ytterligare åtgärder som att lägga till bilagor eller konfigurera erbjudanden
* Öppna [E-posta Designer](get-started-email-designer.md#start-authoring) för att börja skapa rätt innehåll i e-postmeddelandet

>[!NOTE]
>
>Alla redigerbara textfält på den här skärmen kan fyllas i med hjälp av anpassningsfält. [Lär dig anpassa innehåll](../personalization/personalize.md)

Följ stegen nedan för att konfigurera eller redigera innehållet i ett e-postmeddelande.

1. Klicka på **[!UICONTROL Edit content]** från [kontrollpanel för e-postleverans](../email/create-email.md) skärm.

   ![](assets/email-edit-content-button.png){zoomable="yes"}

1. E-postinnehållets versionsskärm öppnas.

   ![](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Om ditt e-postmeddelande konfigureras **[!UICONTROL From name]** och **[!UICONTROL From email]** fälten har redan fyllts i.

1. The **[!UICONTROL From name]** -fältet definieras i e-postmallen. Om du vill ändra det använder du ett namn som mottagarna lätt kan identifiera, till exempel ert varumärkes namn, för att öka öppningshastigheten för era leveranser.

   >[!NOTE]
   >
   >Om du vill förbättra mottagarens upplevelse ytterligare kan du lägga till en persons namn, t.ex. &quot;Eva from Luma&quot;.

1. The **[!UICONTROL From email]** adressfältet definieras också i e-postmallen. Kontrollera att adressdomänen är densamma som den underdomän som du delegerat till Adobe.

   >[!NOTE]
   >
   >Du kan ändra den del som föregår @, men inte domänadressen.

1. Expandera **[!UICONTROL Reply-to fields]** -avsnitt. Avsändarens namn och adresser används som standard för svar. Adobe rekommenderar dock att man använder en befintlig riktig adress som till exempel kundtjänst för ert varumärke. Om en mottagare skickar ett svar kan kundtjänst hantera det.

   ![](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Definiera e-postmeddelandet **[!UICONTROL Subject line]**. Skriv in ämnet direkt i det dedikerade fältet eller öppna uttrycksredigeraren för att lägga till [personalisering](../personalization/personalize.md) med olika attribut och innehållsblock, eller erbjudanden.

1. Om du vill bifoga en fil till e-postmeddelandet klickar du på **[!UICONTROL Add attachment]** och sedan markera en eller flera filer.

   >[!NOTE]
   >
   >    För att undvika prestandaproblem rekommenderar vi att du inte inkluderar mer än en bifogad fil per e-post.

   <!--limitation on size + number of files?-->

1. Om du vill skicka erbjudanden via e-post väljer du dem med **[!UICONTROL Set up offers]** -knappen.

   Du kan sedan infoga dem i e-postmeddelandet med hjälp av anpassningsfält. [Lär dig skicka erbjudanden](../msg/offers.md)

1. Klicka på **[!UICONTROL Edit email body]** för att strukturera och utforma innehållet i e-postmeddelandet med [E-posta Designer](get-started-email-designer.md#start-authoring). Mer information om hur du utformar e-postinnehåll finns i följande avsnitt:

   * [Skapa e-postmeddelanden från grunden](create-email-content.md)
   * [Formatera innehållet](get-started-email-style.md)

   >[!NOTE]
   >
   >Du kan också hovra över e-postförhandsgranskningen och välja **[!UICONTROL Open email designer]**.

1. Spårning är aktiverat som standard för leveransen. Du kan inaktivera det här alternativet på **[!UICONTROL Optional features]** -avsnitt. [Lär dig hur du lägger till länkar och hanterar spårning](message-tracking.md)

1. När innehållet i e-postmeddelandet har definierats använder du **[!UICONTROL Simulate content]** för att kontrollera hur det visas innan det skickas. [Lär dig hur du förhandsgranskar och testar e-postmeddelanden](../preview-test/preview-test.md)

