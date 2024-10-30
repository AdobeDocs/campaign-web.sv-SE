---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---


# Anpassa innehållet {#add-personalization}

Personalization av leveransinnehåll är en nyckelfunktion som gör att ni kan skräddarsy meddelanden för enskilda mottagare och göra kommunikationen mer relevant och engagerande.

I Adobe Campaign kan du med hjälp av [profildata](#data-personalization), t.ex. profilens namn, plats eller tidigare interaktioner samt specifika [variabler för leveransen](#variables-personalization), dynamiskt anpassa element som text, bilder och erbjudanden i kommunikationen.

Leveranspersonaliseringen förbättrar inte bara användarupplevelsen utan även engagemangsfrekvensen, vilket leder till högre konverteringsgrad och nöjdare kunder.

## Använda profildata för personalisering {#data-personalization}

Du kan anpassa alla leveranser med profildata med hjälp av uttrycksredigeraren, som är tillgänglig i fält med ikonen **[!UICONTROL Open personalization dialog]** , till exempel ämnesraden, e-postlänkar och text/knappinnehållskomponenter. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md/#access)

### Personalization syntax {#syntax}

Personalization-taggar följer en specifik syntax: `<%= table.field %>`. Om du till exempel vill infoga mottagarens efternamn från mottagartabellen använder du syntaxen `<%= recipient.lastName %>`.

Under leveransförberedelseprocessen tolkar Adobe Campaign automatiskt dessa taggar och ersätter dem med motsvarande fältvärden för varje mottagare. Du kan visa den faktiska ersättningen genom att simulera innehållet.

När du överför kontakter från en extern fil för en fristående e-postleverans är alla fält i indatafilen tillgängliga för personalisering. Syntaxen är följande: `<%= dataSource.field %>`.

### Lägg till personaliseringstaggar {#add}

Så här lägger du till personaliseringstaggar i en leverans:

1. Öppna uttrycksredigeraren med ikonen **[!UICONTROL Open personalization dialog]** som är tillgänglig från redigeringsfält av texttyp, till exempel ämnesraden eller SMS-brödtexten. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. Uttrycksredigeraren öppnas. Anpassningsfält som finns i Adobe Campaign-databasen är ordnade i flera menyer till vänster på skärmen:

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Meny | Beskrivning |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Subscribers application]** visar fält som är relaterade till prenumeranterna av ett program, till exempel den använda terminalen eller operativsystemet. *Den här menyn är bara tillgänglig för push-meddelanden* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Recipient]** visar fält som definierats i mottagartabellen, t.ex. mottagarnas namn, sidor eller adresser. När [överför kontakter från en extern fil](../audience/file-audience.md) för en fristående e-postleverans visas alla fält som är tillgängliga i indatafilen på den här menyn. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Message]** listar fält som är relaterade till leveransloggarna, inklusive alla meddelanden som skickas till mottagare eller enheter över alla kanaler, till exempel datumet för den senaste händelsen med en viss mottagare |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Delivery]** visar fält som är relaterade till de parametrar som krävs för att utföra leveranser, t.ex. leveranskanalen eller etiketten. |

   >[!NOTE]
   >
   >Som standard visar varje meny alla fält i den markerade tabellen (Mottagare, Meddelande / Leverans). Om du vill ta med fält från tabeller som är länkade till den markerade tabellen aktiverar du alternativet **[!UICONTROL Display advanced attributes]** som finns nedanför listan.

1. Om du vill lägga till ett anpassningsfält placerar du markören på önskad plats i innehållet och klickar på knappen `+` för att infoga den.

1. När innehållet är klart kan du spara det och testa återgivningen av personaliseringen genom att simulera innehållet. I exemplet nedan visas personaliseringen av ett SMS-meddelande med mottagarnas förnamn.

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Använda variabler för personalisering {#variables-personalization}

Du kan också använda variabler för att anpassa leveransen.
Läs mer om att [lägga till variabler i en leverans](../advanced-settings/delivery-settings.md#variables-delivery).

Variabeln `deliveryType` har till exempel definierats enligt nedan.

![](assets/variables-deliveryType.png){zoomable="yes"}

Den här variabeln kan användas i innehållet i leveransen med ikonen **[!UICONTROL Add Personalization]** och uttrycket `<%= variables.deliveryType %>` som exempel.

![](assets/variables-perso.png){zoomable="yes"}

Du kan kontrollera hur variabeln används med knappen **[!UICONTROL Simulate Content]**.

![](assets/variables-simulate.png){zoomable="yes"}
