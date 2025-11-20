---
audience: end-user
title: Lägg till erbjudanden i dina meddelanden
description: Lär dig lägga till och skicka erbjudanden
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Lägg till erbjudanden i dina meddelanden {#offers-content}

Du kan lägga till erbjudanden i Adobe Campaign webbgränssnitt. Erbjudandena finns på den vänstra menyn **Erbjudanden** som ger dig tillgång till listan med erbjudanden. Alla erbjudanden är skrivskyddade och måste skapas i Campaign-klientkonsolen med modulen **[!UICONTROL Interaction]**. Mer information om interaktion och hur du hanterar en erbjudandekatalog i konsolen finns i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=sv-SE){target="_blank"}.

Så här skickar du erbjudanden med leverans:

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

Med Adobe Campaign kan ni svara i realtid under en interaktion med en viss kontakt genom att föreslå ett eller flera specifika erbjudanden. Erbjudandena kan vara enkla kommunikationsmeddelanden, specialerbjudanden för en eller flera produkter eller en tjänst.

Följ stegen nedan för att välja vilka erbjudanden som ska läggas till i leveransen.

1. Klicka på knappen **[!UICONTROL Set up offers]** på skärmen för leveransutgåva.

   ![Skärmbild som visar inställningsknappen för erbjudandet på skärmen för leveransutgåva](assets/offer-setup.png){zoomable="yes"}

1. Konfigurera vilka erbjudanden som ska föreslås för mottagarna.

   Välj först **[!UICONTROL Offer space]** som matchar din erbjudandemiljö. Lär dig hur du skapar ett erbjudandeutrymme i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html?lang=sv-SE){target="_blank"}.

   ![Skärmbild som visar det lediga utrymmet i innehållet som skapar erbjudandet](assets/offer-create-content.png){zoomable="yes"}

1. Om du vill förfina motorns val av erbjudanden väljer du en specifik **[!UICONTROL Offer category]** där erbjudandena sorteras.

   När du väljer en mapp inkluderas alla undermappar automatiskt och kan inte tas bort. Observera att gränssnittet [!DNL Campaign] inte återspeglar det här beteendet.

   >[!NOTE]
   >
   >Om ingen kategori anges, beaktas alla erbjudanden i miljön av erbjudandemotorn, såvida inte **[!UICONTROL Offer theme]** har valts.

1. (Valfritt) Ange ett tema för att filtrera kategorier. Teman är nyckelord som definieras uppströms i kategorierna. De fungerar som ett filter och förfinar antalet erbjudanden genom att välja dem i en uppsättning kategorier.

1. Använd fältet **[!UICONTROL Propositions]** för att ange antalet erbjudanden du vill infoga i leveransen.

1. Välj alternativet **[!UICONTROL Exclude non-eligible recipients]** om det behövs.

   Med det här alternativet kan du aktivera eller inaktivera exkluderingen av mottagare för vilka det inte finns tillräckligt med giltiga erbjudanden:

   * Om alternativet är aktiverat exkluderas mottagare som inte har tillräckligt med erbjudanden från leveransen.
   * Om alternativet är inaktiverat utesluts inte dessa mottagare, men de kan inte ha det begärda antalet förslag.

1. Välj alternativet **[!UICONTROL Hide everything if no offer is selected]** om det behövs.

   Med det här alternativet kan du välja hur meddelandet ska behandlas om något av förslagen inte finns:

   * Om alternativet är aktiverat visas inte representationen av det saknade förslaget och inget innehåll visas i meddelandet för det här förslaget.
   * Om alternativet är inaktiverat avbryts själva meddelandet när det skickas och mottagarna kan inte längre ta emot några meddelanden.

När du har konfigurerat de erbjudanden du vill föreslå i leveransen kan du infoga dem i leveransinnehållet.

## Lägg in erbjudanden i leveransen {#insert}

Erbjudanden kan läggas till i leveransen med [uttrycksredigeraren](../personalization/gs-personalization.md#access). De kan läggas in antingen på ärenderaden eller i leveransenheten.

>[!CAUTION]
>
>Innan du infogar ett erbjudande i en leverans måste du kontrollera att du har [konfigurerat vilka erbjudanden som ska erbjudas med den leveransen](#configure).

Följ stegen nedan för att infoga ett erbjudande med uttrycksredigeraren.

1. Gå till ämnesraden eller innehållet i alla leveranser.

1. Placera markören där du vill infoga erbjudandet och öppna uttrycksredigeraren med personaliseringsikonen.

   ![Skärmbild som visar den personaliseringsikon som används för att öppna uttrycksredigeraren](assets/offer-insert-perso-icon.png){zoomable="yes"}

1. Välj menyn **[!UICONTROL Propositions]**. Tillgängliga förslag visas i listan.

   >[!NOTE]
   >
   >Antalet offerter definieras när [du ställer in erbjudanden](#configure) för den aktuella leveransen.

1. Definiera varje förslag med hjälp av anpassningsfält, återgivningsfunktioner eller tillgängliga attribut.

   ![Skärmbild som visar ett erbjudande som infogats i leveransinnehållet](assets/offer-inserted.png){zoomable="yes"}

   >[!NOTE]
   >
   >Antalet tillgängliga offerter beror på hur motoranropet är konfigurerat och deras ordning beror på prioriteten för erbjudandena. Läs mer i [dokumentationen för Campaign v8 (klientkonsolen)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=sv-SE){target="_blank"}.

1. Spara ändringarna.

1. Slutför innehållet, testa och skicka leveransen. [Läs mer](gs-messages.md).

När en mottagare får leveransen visas rätt erbjudande för just den profilen.