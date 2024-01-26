---
audience: end-user
title: Lägg till erbjudanden i dina meddelanden
description: Lär dig lägga till och skicka erbjudanden
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Begränsad tillgänglighet"
source-git-commit: f614919e0ad253aa4625f774e7fe102426e25807
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---


# Lägg till erbjudanden i dina meddelanden {#offers-content}

Med Adobe Campaign Web kan du skicka med leveranserbjudanden som har skapats i konsolen via **[!UICONTROL Interaction]** -modul. Mer information om interaktion och hur du hanterar en erbjudandekatalog i konsolen finns i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

Så här skickar du erbjudanden med en leverans:

1. [Konfigurera de erbjudanden som ska föreslås](#configure)
1. [Lägg in erbjudandena i leveransen](#insert)

## Konfigurera de erbjudanden som ska föreslås {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Definiera erbjudandeparametrarna"
>abstract="Konfigurera vilka erbjudanden som ska föreslås för mottagarna genom att definiera ett erbjudandeutrymme, eventuellt en kategori och ett tema, och ange hur många erbjudanden du vill infoga i leveransen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Ange avancerade inställningar för erbjudanden"
>abstract="Du kan aktivera uteslutning av mottagare för vilka det inte finns tillräckligt med giltiga erbjudanden och välja hur meddelandet ska behandlas om ett av förslagen inte finns."

Med Adobe Campaign kan ni svara i realtid under en interaktion med en viss kontakt genom att föreslå en eller flera specifika erbjudanden. Erbjudandena kan vara enkla kommunikationsmeddelanden, specialerbjudanden för en eller flera produkter eller en tjänst.

Följ stegen nedan för att välja vilka erbjudanden som ska läggas till i leveransen.

1. Klicka på **[!UICONTROL Set up offers]** på skärmen för utgåva av leveransinnehåll.

   ![](assets/offer-setup.png)

1. Konfigurera vilka erbjudanden som ska föreslås för mottagarna.

   Markera först **[!UICONTROL Offer space]** som matchar er erbjudandemiljö. Lär dig hur du skapar ett erbjudandeutrymme på [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}.

   ![](assets/offer-create-content.png)

1. Om du vill förfina motorns val av erbjudanden väljer du en specifik **[!UICONTROL Offer category]** där erbjudandena sorteras.

   När du väljer en mapp inkluderas alla undermappar automatiskt och kan inte tas bort. Observera att [!DNL Campaign] gränssnittets beteende återspeglas inte.

   >[!NOTE]
   >
   >Om ingen kategori anges beaktas alla erbjudanden i miljön, såvida inte en **[!UICONTROL Offer theme]** är markerat.

1. (valfritt) Ange ett tema för att filtrera kategorier. Teman är nyckelord som definieras uppströms i kategorierna. De fungerar som ett filter och låter dig förfina antalet erbjudanden som ska presenteras genom att välja dem i en uppsättning kategorier.

1. Använd **[!UICONTROL Propositions]** för att ange antalet erbjudanden du vill infoga i leveransen.

1. Välj **[!UICONTROL Exclude non-eligible recipients]** vid behov.

   Med det här alternativet kan du aktivera eller inaktivera exkluderingen av mottagare för vilka det inte finns tillräckligt med giltiga erbjudanden:

   * Om alternativet är aktiverat exkluderas mottagare som inte har tillräckligt med erbjudanden från leveransen.
   * Om alternativet är inaktiverat utesluts inte dessa mottagare, men de kan inte ha det begärda antalet förslag.

1. Om det behövs väljer du **[!UICONTROL Hide everything if no offer is selected]** alternativ.

   Med det här alternativet kan du välja hur meddelandet ska behandlas om något av förslagen inte finns:

   * Om alternativet är aktiverat visas inte representationen av det saknade förslaget och inget innehåll visas i meddelandet för det här förslaget.
   * Om alternativet är inaktiverat avbryts själva meddelandet när det skickas och mottagarna kan inte längre ta emot några meddelanden.

När du har konfigurerat de erbjudanden du vill föreslå i leveransen kan du infoga dem i leveransinnehållet.

## Lägg in erbjudanden i leveransen {#insert}

Erbjudandena kan läggas till i leveransen med [uttrycksredigerare](../personalization/gs-personalization.md#access). De kan läggas in antingen på ärenderaden eller i leveransenheten.

>[!CAUTION]
>
>Kontrollera att du har [konfigurerade vilka erbjudanden som ska erbjudas med den leveransen](#configure).

Följ stegen nedan för att infoga ett erbjudande med uttrycksredigeraren.

1. Gå till ämnesraden eller innehållet i alla leveranser.

1. Placera musmarkören där du vill infoga erbjudandet och öppna uttrycksredigeraren med ikonen för personalisering.

   ![](assets/offer-insert-perso-icon.png)

1. Välj **[!UICONTROL Propositions]** -menyn. Tillgängliga förslag visas i listan.

   >[!NOTE]
   >
   >Antalet offerter definieras när [konfigurera erbjudanden](#configure) för aktuell leverans.

1. Definiera varje förslag med hjälp av anpassningsfälten, återgivningsfunktionerna eller tillgängliga attribut.

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >Antalet tillgängliga offerter beror på hur motoranropet är konfigurerat och deras ordning beror på erbjudandenas prioritet. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. Spara ändringarna.

1. Slutför innehållet, testa och skicka leveransen. [Läs mer](gs-messages.md)

När en mottagare får leveransen visas rätt erbjudande för just den profilen.
