---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: d12c3019fb47164864259ecc40225fcb04de0e6c
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Anpassa innehållet{#add-personalization}

Personalisering kan läggas till i alla leveranser med uttrycksredigeraren.

En personaliseringstagg använder alltid följande syntax: `<%=table.field%>`Om du till exempel vill infoga namnet på mottagaren, som lagras i mottagartabellen, använder personaliseringstaggen syntaxen &lt;%= mottagare.efternamn %>.

När en leverans förbereds tolkas dessa taggar automatiskt av Adobe Campaign och ersätts av fältvärdet för en viss mottagare. Den fysiska ersättningen kan sedan visas när du simulerar ditt innehåll.

Om du vill lägga till personaliseringstaggar i en leverans klickar du på ikonen Öppna personalisering som är tillgänglig från redigeringsfält av texttyp, till exempel ämnesraden eller SMS-brödtexten.

![](assets/perso-access.png)

Uttrycksredigeraren visas. Anpassningsfält är ordnade i tre menyer, som finns till vänster på skärmen. Dessa menyer ger åtkomst till alla fält som är tillgängliga i Adobe Campaign-databasen.

| Meny | Beskrivning |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | The **[!UICONTROL Recipient]** I visas alla fält som definierats i mottagartabellen, t.ex. mottagarnas namn, ålder eller adress. |
| ![](assets/do-not-localize/perso-message-menu.png) | The **[!UICONTROL Message]** -menyn innehåller alla fält som hör till leveransloggarna, dvs. alla meddelanden som skickas till mottagare eller enheter i alla kanaler, t.ex. datumet för den senaste händelsen med en viss mottagare |
| ![](assets/do-not-localize/perso-delivery-menu.png) | The **[!UICONTROL Delivery]** På menyn visas alla fält som hör till de parametrar som krävs för att utföra leveranser, t.ex. leveranskanal, etikett osv. |

>[!NOTE]
>
>Som standard visas alla fält i den markerade tabellen (Mottagare, Meddelande / Leverans). Om du vill ta med fält från tabeller som är länkade till den markerade tabellen aktiverar du **[!UICONTROL Display advanced attributes]** alternativ som finns under listan.

Om du vill lägga till ett anpassningsfält placerar du markören på önskad plats i innehållet och klickar på plusknappen (+) för att infoga den.

![](assets/perso-insert-field.png)
