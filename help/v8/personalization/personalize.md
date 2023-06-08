---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 551e6b9efa8b29475bd2f0a71ce016681bf70289
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---


# Anpassa innehållet {#add-personalization}

Personalisering kan läggas till i alla leveranser med uttrycksredigeraren, som är tillgänglig i alla fält med **[!UICONTROL Open personalization dialog]** ikon, t.ex. ämnesradfältet, eller e-postlänkar och text-/knappinnehållskomponenter. [Lär dig var du lägger till dynamiskt innehåll](gs-personalization.md/#access)

## Anpassningssyntax {#syntax}

En personaliseringstagg använder alltid följande syntax: `<%=table.field%>`. Om du till exempel vill infoga namnet på mottagaren, som lagras i mottagartabellen, använder personaliseringstaggen syntaxen &lt;%= mottagare.efternamn %>.

När en leverans förbereds tolkas dessa taggar automatiskt av Adobe Campaign och ersätts av fältvärdet för en viss mottagare. Den fysiska ersättningen kan sedan visas när du simulerar ditt innehåll.

## Lägg till personaliseringstaggar {#add}

Om du vill lägga till personaliseringstaggar i en leverans öppnar du uttrycksredigeraren med **[!UICONTROL Open personalization dialog]** -ikoner som är tillgängliga från redigeringsfält av texttyp, t.ex. ämnesraden eller SMS-brödtexten. [Lär dig var du lägger till dynamiskt innehåll](gs-personalization.md/#access)

![](assets/perso-access.png)

Uttrycksredigeraren visas. Anpassningsfält ordnas i flera menyer, som finns till vänster på skärmen. Dessa menyer ger åtkomst till alla fält som är tillgängliga i Adobe Campaign-databasen.

![](assets/perso-insert-field.png)

| Meny | Beskrivning |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | The **[!UICONTROL Subscribers application]** På -menyn visas alla fält som är relaterade till prenumeranterna av ett program, t.ex. terminalen eller operativsystemet som används. *Den här menyn är endast tillgänglig för push-meddelanden* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | The **[!UICONTROL Recipient]** I visas alla fält som definierats i mottagartabellen, t.ex. mottagarnas namn, ålder eller adress. |
| ![](assets/do-not-localize/perso-message-menu.png) | The **[!UICONTROL Message]** -menyn innehåller alla fält som hör till leveransloggarna, dvs. alla meddelanden som skickas till mottagare eller enheter i alla kanaler, t.ex. datumet för den senaste händelsen med en viss mottagare |
| ![](assets/do-not-localize/perso-delivery-menu.png) | The **[!UICONTROL Delivery]** På menyn visas alla fält som hör till de parametrar som krävs för att utföra leveranser, t.ex. leveranskanal, etikett osv. |

>[!NOTE]
>
>Som standard visar varje meny alla fält i den markerade tabellen (Mottagare, Meddelande / Leverans). Om du vill ta med fält från tabeller som är länkade till den markerade tabellen aktiverar du **[!UICONTROL Display advanced attributes]** alternativ som finns under listan.

Om du vill lägga till ett anpassningsfält placerar du markören på önskad plats i innehållet och klickar på plusknappen (+) för att infoga den.

När innehållet är klart kan du spara det och testa återgivningen av personaliseringen genom att simulera innehållet. I exemplet nedan personaliserar vi ett SMS-meddelande med målprofilens förnamn.

*Lägg till personaliseringstaggen i meddelandeinnehållet*

![](assets/perso-preview1.png)

*Simulera återgivningen av personaliseringen för en given testprofil*

![](assets/perso-preview2.png)
