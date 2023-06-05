---
audience: end-user
title: Redigera e-postinnehållet
description: Lär dig hur du redigerar e-postinnehåll i webbgränssnittet för Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: 46f2f42f724232b15f826f01c5957c0295c61f26
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Konfigurera e-postinnehållet {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Skapa e-postinnehåll"
>abstract="I det här avsnittet kan du skapa innehåll för ditt e-postmeddelande och använda e-postdesignern för att ge det ett snyggt utseende."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="E-postparametrar"
>abstract="E-postvärdena Från och Från definieras i e-postmallen. Subject line kan anpassas med Expression Editor."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="E-postbilaga"
>abstract="Markera en eller flera filer som ska infogas i meddelandet."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Spårningsalternativ"
>abstract="Spårning är aktiverat som standard för leveransen. Du kan inaktivera det här alternativet härifrån."

Om du vill börja skapa innehållet i ett e-postmeddelande klickar du på **[!UICONTROL Edit content]** från [kontrollpanel för e-postleverans](../email/create-email.md) skärm.

![](assets/email-edit-content.png)

På skärmen som öppnas kan du definiera grundläggande information, utföra ytterligare åtgärder som att lägga till bilagor eller konfigurera erbjudanden samt få tillgång till [E-postdesigner](#start-authoring) för att skapa innehåll.

![](assets/email-edit-content-dashboard.png)

Så här redigerar du innehållet i ditt e-postmeddelande:

1. I **[!UICONTROL From name]** används ett namn som lätt kan identifieras av mottagarna, till exempel ert varumärkes namn, för att öka öppningshastigheten för era leveranser.

   Om du vill förbättra mottagarens upplevelse ytterligare kan du lägga till en persons namn, till exempel&quot;Emma from Megastore&quot;.

1. I **[!UICONTROL From email]** adressfältet, kontrollera att adressdomänen är densamma som den underdomän som du delegerat till Adobe.

   >[!NOTE]
   >
   >    Du kan ändra den del som föregår @, men inte domänadressen.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Definiera e-postmeddelandet **[!UICONTROL Subject line]**. Skriv in ämnet direkt i det dedikerade fältet eller öppna uttrycksredigeraren för att lägga till personalisering med olika attribut och innehållsblock eller erbjudanden. [Lär dig anpassa innehåll](../personalization/personalize.md)

1. Om du vill bifoga en fil till e-postmeddelandet klickar du på knappen **[!UICONTROL Add attachment]** och sedan markera en eller flera filer.

   >[!NOTE]
   >
   >    För att undvika prestandaproblem rekommenderar vi att du inte inkluderar mer än en bifogad fil per e-post.

   <!--limitation on size + number of files?-->

1. Om du vill skicka erbjudanden via e-post väljer du dem med **[!UICONTROL Set up offers]** -knappen.

   Du kan sedan infoga dem i e-postmeddelandet med hjälp av anpassningsfält. [Lär dig hur du skickar erbjudanden](offers.md)

1. Klicka på **[!UICONTROL Edit email body]** för att strukturera och utforma innehållet i e-postmeddelandet med [E-postdesigner](#start-authoring). Mer information om hur du utformar e-postinnehåll finns i följande avsnitt:

   * [Lär dig hur du utformar e-postmeddelanden](create-email-content.md)
   * [Formatera innehållet](get-started-email-style.md)

1. Spårning är aktiverat som standard för leveransen. Du kan inaktivera det här alternativet på **[!UICONTROL Optional features]** -avsnitt. [Lär dig hur du lägger till länkar och hanterar spårning](message-tracking.md)

1. När innehållet i e-postmeddelandet har definierats använder du **[!UICONTROL Simulate content]** för att kontrollera hur det visas innan det skickas. [Lär dig hur du förhandsgranskar och testar e-postmeddelanden](../preview-test/preview-test.md)

