---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign Web
feature: Personalization
topic: Personalization
old-role: Data Engineer
role: Developer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Anpassa innehållet {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="Lägg till aktuellt datum"
>abstract="Den här menyn innehåller funktioner för datumformatering som du kan använda för att anpassa innehållet."

Personalization av leveransinnehåll är en nyckelfunktion som gör att ni kan skräddarsy meddelanden för enskilda mottagare och göra kommunikationen mer relevant och engagerande.

I Adobe Campaign kan du med hjälp av [profildata](#data-personalization), t.ex. profilens namn, plats eller tidigare interaktioner samt specifika [variabler för leveransen](#variables-personalization), dynamiskt anpassa element som text, bilder och erbjudanden i kommunikationen.

Leveranspersonalisering förbättrar användarupplevelsen och ökar engagemangsfrekvensen, vilket leder till högre konverteringsgrad och nöjdare kunder.

## Använda profildata för personalisering {#data-personalization}

Du kan anpassa alla leveranser med profildata med hjälp av uttrycksredigeraren, som är tillgänglig i fält med ikonen **[!UICONTROL Open personalization dialog]** , t.ex. ämnesraden, e-postlänkar och innehållskomponenter för text/knapp. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md#access).

### Personalization syntax {#syntax}

Personalization-taggar följer en specifik syntax: `<%= table.field %>`. Om du till exempel vill infoga mottagarens efternamn från mottagartabellen använder du syntaxen `<%= recipient.lastName %>`.

Under leveransförberedelseprocessen tolkar Adobe Campaign dessa taggar och ersätter dem med motsvarande fältvärden för varje mottagare. Du ser den faktiska ersättningen genom att simulera innehållet.

När du överför kontakter från en extern fil för en fristående e-postleverans är alla fält i indatafilen tillgängliga för personalisering. Syntaxen är följande: `<%= dataSource.field %>`.

### Lägg till personaliseringstaggar {#add}

Så här lägger du till personaliseringstaggar i en leverans:

1. Öppna uttrycksredigeraren med ikonen **[!UICONTROL Open personalization dialog]** som du kommer åt från redigeringsfält av texttyp, till exempel ämnesraden eller SMS-brödtexten. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md#access).

   ![Skärmbild som visar hur du kommer åt dialogrutan för anpassning](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. Uttrycksredigeraren öppnas. Anpassningsfält som finns i Adobe Campaign-databasen är ordnade i flera menyer till vänster på skärmen:

   ![Skärmbild som visar anpassningsfältmenyn](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Meny | Beskrivning |
   |------|-------------|
   | ![Programmenyikon för prenumeranter](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Subscribers application]** visar fält som är relaterade till prenumeranterna av ett program, till exempel den använda terminalen eller operativsystemet. *Den här menyn är endast tillgänglig för push-meddelanden.* |
   | ![Ikon på menyn Mottagare](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Recipient]** visar fält som definierats i mottagartabellen, t.ex. mottagarnas namn, sidor eller adresser. När [överför kontakter från en extern fil](../audience/file-audience.md) för en fristående e-postleverans visas alla fält som är tillgängliga i indatafilen på den här menyn. |
   | ![Ikon för meddelandemeny](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Message]** listar fält som är relaterade till leveransloggarna, inklusive alla meddelanden som skickas till mottagare eller enheter över alla kanaler, till exempel datumet för den senaste händelsen med en viss mottagare. |
   | ![Ikon för leveransmenyn](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Menyn **[!UICONTROL Delivery]** visar fält som är relaterade till de parametrar som krävs för att utföra leveranser, till exempel leveranskanalen eller etiketten. |

   >[!NOTE]
   >
   >Som standard visar varje meny alla fält i den markerade tabellen (Mottagare, Meddelande / Leverans). Om du vill ta med fält från tabeller som är länkade till den markerade tabellen aktiverar du alternativet **[!UICONTROL Display advanced attributes]** som finns nedanför listan.

1. Om du vill lägga till ett anpassningsfält placerar du markören på önskad plats i innehållet och infogar det genom att klicka på knappen `+`.

1. När innehållet är klart sparar du det och testar återgivningen av personaliseringen genom att simulera innehållet. I exemplet nedan visas personaliseringen av ett SMS-meddelande med mottagarnas förnamn.

   ![Skärmbild med förhandsgranskning av SMS-personalisering med mottagarens förnamn](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![Skärmbild med förhandsgranskning av SMS-personalisering med mottagarens förnamn](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Använda variabler för personalisering {#variables-personalization}

Ni använder också variabler för att personalisera leveransen. Läs mer om att [lägga till variabler i en leverans](../advanced-settings/delivery-settings.md#variables-delivery).

Variabeln `deliveryType` definieras till exempel enligt nedan.

![Skärmbild som visar definitionen för variabeln deliveryType ](assets/variables-deliveryType.png){zoomable="yes"}

Den här variabeln används i innehållet i leveransen med hjälp av ikonen **[!UICONTROL Add Personalization]** och uttrycket `<%= variables.deliveryType %>` för det här exemplet.

![Skärmbild som visar användningen av variabeln deliveryType i personalisering](assets/variables-perso.png){zoomable="yes"}

Kontrollera hur variabeln används med knappen **[!UICONTROL Simulate Content]**.

![Skärmbild som visar simulering av innehåll med variabeln deliveryType ](assets/variables-simulate.png){zoomable="yes"}