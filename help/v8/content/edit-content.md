---
audience: end-user
title: Redigera e-postinnehållet
description: Lär dig hur du redigerar e-postinnehåll i webbgränssnittet för Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Redigera e-postinnehållet {#configure-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Skapa e-postinnehåll"
>abstract="I det här avsnittet kan du skapa innehåll för ditt e-postmeddelande och använda e-postdesignern för att ge det ett snyggt utseende."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="E-posthuvud"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="E-postbilaga"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Spårningsalternativ"
>abstract="TBC"

Om du vill börja skapa innehållet i ett e-postmeddelande klickar du på **[!UICONTROL Edit content]** från skärmen där e-postmeddelanden skapas.

![](assets/edit-content.png)

På den här skärmen kan du definiera innehållet i e-postmeddelandet och komma åt e-postdesignern för att utforma det.

![](assets/content-dashboard.png)

Stegen för att definiera innehållet i e-postmeddelandet är följande:

1. Kontrollera **[!UICONTROL From name]** och **[!UICONTROL From email]** information. Dessa fält är skrivskyddade, de konfigureras i e-postmallen som väljs när e-postmeddelandet skapas.

1. Definiera e-postmeddelandet **[!UICONTROL Subject line]**. Det gör du genom att skriva in ämnet direkt i det dedikerade fältet eller genom att öppna Uttrycksredigeraren och definiera hur personalisering ska användas med olika attribut och innehållsblock eller erbjudanden. [Lär dig anpassa innehåll](../personalization/personalize.md)

1. Om du vill skicka erbjudanden via e-post väljer du dem med **[!UICONTROL Set up offers]** -knappen. Du kan sedan infoga dem i e-postmeddelandet med hjälp av anpassningsfält. [Lär dig hur du skickar erbjudanden](offers.md)

1. Klicka på **[!UICONTROL Edit email body]** för att strukturera och utforma innehållet i e-postmeddelandet. Mer information om hur du utformar e-postinnehåll finns i följande avsnitt:

   * [Lär dig hur du utformar e-postmeddelanden](create-email-content.md)
   * [Formatera innehållet](get-started-email-style.md)

1. Om du vill bifoga en fil till e-postmeddelandet klickar du på knappen **[!UICONTROL Add attachment]** och sedan markera en eller flera filer.

   För att undvika prestandaproblem rekommenderar vi att du inte inkluderar mer än en bifogad fil per e-post.

   <!--limitation on size + number of files?-->

1. Spårning är aktiverat som standard för leveransen. Du kan inaktivera det här alternativet från **[!UICONTROL Optional features]** -avsnitt. [Lär dig hur du lägger till länkar och hanterar spårning](message-tracking.md)

När innehållet i e-postmeddelandet har definierats använder du **[!UICONTROL Simulate content]** för att kontrollera hur det visas innan det skickas. [Lär dig hur du förhandsgranskar och testar e-postmeddelanden](../preview-test/preview-test.md)
