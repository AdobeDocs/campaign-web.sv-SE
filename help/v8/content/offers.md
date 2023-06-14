---
audience: end-user
title: Skicka erbjudanden
description: Skicka erbjudanden
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha"
source-git-commit: 3de1ff02f095abf49a5ac23ad291408a81f80b51
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# Skicka erbjudanden {#offers-content}

Med Adobe Campaign v8 Web kan du skicka med e-posterbjudanden som har skapats i konsolen via **[!UICONTROL Interaction]** -modul. Mer information om interaktion och hur du hanterar en erbjudandekatalog i konsolen finns i [Kampanjdokumentation v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

Så här skickar du erbjudanden via e-post:

1. [Konfigurera erbjudandena att föreslå](#configure),
1. [Infoga erbjudandena i e-postmeddelandet](#insert).

## Konfigurera erbjudandena att föreslå {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Inställningar för erbjudanden"
>abstract="Konfigurera vilka erbjudanden som ska föreslås för mottagarna."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Avancerade inställningar för erbjudanden"
>abstract="Konfigurera avancerade alternativ för erbjudanden."

1. Klicka på knappen **[!UICONTROL Offers]** från skärmen för utgåva av e-postinnehåll.

   ![](assets/setup-offers.png)

1. Konfigurera vilka erbjudanden som ska föreslås för mottagarna. Markera först **[!UICONTROL Offer space]** som matchar er erbjudandemiljö.

   ![](assets/create-content-offers.png)

1. Om du vill förfina motorns val av erbjudanden väljer du en specifik **[!UICONTROL Offer category]** där erbjudandena sorteras. När du väljer en mapp inkluderas alla undermappar automatiskt och kan inte tas bort. Observera att användargränssnittet inte återspeglar detta beteende.

   Om ingen kategori anges beaktas alla erbjudanden i miljön, såvida inte en **[!UICONTROL Offer theme]** är markerat.

1. (valfritt) Ange ett tema för att filtrera kategorier. Teman är nyckelord som definieras uppströms i kategorierna. De fungerar som ett filter och låter dig förfina antalet erbjudanden som ska presenteras genom att välja dem i en uppsättning kategorier.

1. Använd **[!UICONTROL Propositions]** för att ange antalet erbjudanden som du vill infoga i e-postmeddelandet.

1. Välj **[!UICONTROL Exclude non-eligible recipients]** vid behov.

   Med det här alternativet kan du aktivera eller inaktivera exkluderingen av mottagare för vilka det inte finns tillräckligt med giltiga erbjudanden.

   * Om alternativet är aktiverat exkluderas mottagare som inte har tillräckligt med erbjudanden från leveransen.
   * Om alternativet är inaktiverat utesluts inte dessa mottagare, men de kan inte ha det begärda antalet förslag.

1. Om det behövs väljer du **[!UICONTROL Hide everything if no offer is selected]** alternativ.

   Med det här alternativet kan du välja hur meddelandet ska behandlas om något av förslagen inte finns.

   * Om alternativet är aktiverat visas inte representationen av det saknade förslaget och inget innehåll visas i meddelandet för det här förslaget.
   * Om alternativet är inaktiverat avbryts själva meddelandet när det skickas och mottagarna kan inte längre ta emot några meddelanden.

När du har konfigurerat erbjudandena att föreslå i ditt e-postmeddelande kan du infoga dem i e-postmeddelandet med hjälp av uttrycksredigeraren. [Lär dig hur du infogar erbjudanden i e-postmeddelandet](#insert)

## Infoga erbjudanden i e-postmeddelandet {#insert}

Erbjudanden kan läggas till i e-postmeddelandet med uttrycksredigeraren. De kan infogas antingen:

* I e-postens ämnesrad
* I e-postbrödtexten genom att tillåta personalisering i alla innehållskomponenter. [Lär dig hur du lägger till innehållskomponenter](content-components.md)

>[!NOTE]
>
>Innan du infogar ett erbjudande måste du se till att du har [konfigurerade vilka erbjudanden som ska erbjudas med e-postmeddelandet](#configure).

Så här infogar du ett erbjudande med Expression Editor:

1. Öppna uttrycksredigeraren och välj sedan **[!UICONTROL Propositions]** -menyn.

   Tillgängliga förslag visas i listan. Antalet offerter definieras när erbjudandena konfigureras.

   ![](assets/offer-insertion.png)

1. Lägg till förslagen i e-postmeddelandets ämne eller innehåll med hjälp av anpassningsfälten, återgivningsfunktionerna eller de attribut som är tillgängliga för varje erbjudande.

   ![](assets/offer-inserted.png)
