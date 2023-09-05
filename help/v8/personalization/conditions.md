---
title: Skapa villkorsstyrt innehåll
description: Lär dig hur du definierar villkor för att anpassa ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 351b60464d8623c34dea2c19bf86b2fa7b4fa45a
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Skapa villkorsstyrt innehåll{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Lägga till villkorligt innehåll"
>abstract="Konfigurera villkorsstyrda innehållsfält för att skapa avancerad dynamisk personalisering baserat på mottagarens profildata. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt."

Villkorligt innehåll är en kraftfull funktion som gör att du kan skapa dynamisk personalisering baserat på mottagarens profil och automatiskt ersätta textblock och bilder när vissa villkor uppfylls. Den här funktionen kan lyfta era kampanjer till nya höjder och leverera målinriktade, personaliserade upplevelser till er målgrupp.

Genom att konfigurera fält för villkorligt innehåll kan du skapa avancerad dynamisk personalisering som till exempel baseras på mottagarens profil. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt. Du kan t.ex. visa&quot;Herr&quot; eller&quot;fru&quot; enligt värdet i fältet Kön i Adobe Campaign-databasen, eller inkludera en annan länk baserat på vilket mottagarspråk som föredras.

## Så här skapar du villkorsstyrt innehåll

Om du vill skapa villkorligt innehåll måste du skapa villkor i **uttrycksredigerare** med specifika hjälpfunktioner. Den här metoden är tillgänglig för alla leveranskanaler, i alla fält där du kan komma åt uttrycksredigeraren, till exempel ämnesraden, e-postlänkar och text-/knappinnehållskomponenter. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md/#access)

Förutom uttrycksredigeraren kan du använda en **villkorsstyrd innehållsbyggare** när du utformar ett e-postmeddelande som gör att du kan skapa villkor med enbart profilattribut. [Lär dig hur du skapar villkorat innehåll i e-postmeddelanden](#condition-condition-builder)

## Skapa villkor i uttrycksredigeraren {#condition-perso-editor}

Följ stegen nedan för att definiera villkorligt innehåll för en leverans med uttrycksredigeraren. I det här exemplet vill vi skapa villkorligt innehåll baserat på mottagarens språk (franska eller engelska).

1. Öppna en leverans och navigera till delen för innehållsredigering.

1. Leta reda på fältet där du vill lägga till villkorligt innehåll. Du kan till exempel lägga till villkorligt innehåll i ett SMS-meddelande.

1. Klicka på **[!UICONTROL Open personalization dialog]** -ikonen bredvid fältet för att öppna uttrycksredigeraren.

   ![](assets/open-perso-editor-sms.png)

1. I personaliseringsredigeraren går du till **[!UICONTROL Helper functions]** till vänster.

1. Klicka på plustecknet bredvid ikonen för att börja skapa villkoret **If** funktion. Följande rad ska läggas till på den centrala skärmen:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersätt `<FIELD>` med ett anpassningsfält, t.ex. mottagarens språk: `recipient.language`.
   * Ersätt `<VALUE>` med det värde som ska uppfyllas. Exempel, `'French'`.
   * Ersätt `Ìnsert content here` med det innehåll som du vill visa för de profiler som uppfyller det angivna villkoret.

     ![](assets/condition-sample1.png){width="800" align="center"}

1. Ange det innehåll som ska visas om mottagarna inte uppfyller villkoret. För att göra detta använder du **else** hjälpfunktion:

   1. Placera markören före uttryckets avslutande tagg `%>` och klicka på `+` bredvid **Annars** funktion.

   1. Ersätt `Ìnsert content here` med det innehåll som du vill visa för de profiler som inte uppfyller if-funktionens villkor.

   ![](assets/condition-sample2.png){width="800" align="center"}

   Du kan också använda **else if** hjälpfunktion för att skapa villkor med flera innehållsvarianter. Uttrycket nedan visar till exempel tre varianter av ett meddelande beroende på mottagarens språk:

   ![](assets/condition-sample3.png){width="800" align="center"}

   >[!NOTE]
   >
   >Varje gång en hjälpfunktion läggs till öppnas (`<%`) och avslutande (`%>`) läggs taggar automatiskt till före och efter funktionen.
   >
   >Exempel efter att du har lagt till en Else-hjälpfunktion i ett uttryck: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Se till att du tar bort de här taggarna för att undvika syntaxfel. I det här exemplet har det korrigerade uttrycket tagits bort **else** funktionstaggar är:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. När villkoret är klart kan du spara innehållet och kontrollera återgivningen genom att simulera innehållet.

## Skapa villkorligt innehåll i e-postmeddelanden {#condition-condition-builder}

Villkorligt innehåll i e-postmeddelanden kan skapas på två sätt:
* I uttrycksredigeraren genom att skapa ett villkor med hjälpfunktioner,
* I en dedikerad villkorsstyrd innehållsbyggare som är tillgänglig när du utformar ett e-postmeddelande.

Det finns detaljerad information om hur du skapar villkor med uttrycksredigeraren [här](#condition-perso-editor). Följande avsnitt innehåller stegvisa instruktioner om hur du skapar villkor med e-postdesignerns funktion för villkorligt innehåll. I det här exemplet vill vi skapa ett e-postmeddelande med flera varianter baserade på mottagarens språk. Följ de här stegen:

1. Skapa eller öppna en e-postleverans, redigera innehållet och klicka på **[!UICONTROL Edit email body]** för att öppna arbetsytan för e-postdesign.

1. Markera en innehållskomponent och klicka på **[!UICONTROL Enable conditional content]** -ikon.

   ![](assets/condition-email-enable.png){width="800" align="center"}

1. The **[!UICONTROL Conditional Content]** öppnas till vänster på skärmen. I den här rutan kan du skapa flera varianter av den markerade innehållskomponenten med villkor.

1. Konfigurera din första variant. Hovring **[!UICONTROL Variant - 1]** i **[!UICONTROL Conditional Content]** och klicka på **[!UICONTROL Add condition]** -ikon.

1. En regelbyggare visas. Använd profilattribut för att skapa villkoret för den första varianten av meddelandet och klicka på **[!UICONTROL Confirm]**. I det här exemplet skapar vi en regel som riktar sig till mottagare vars språk är &quot;franska&quot;.

   ![](assets/condition-email-rule.png){width="800" align="center"}

1. Regeln är nu associerad med varianten. För bättre läsbarhet rekommenderar vi att du byter namn på varianten genom att klicka på ellipsmenyn.

1. Konfigurera hur komponenten ska visas om regeln uppfylls när meddelandet skickas. I det här exemplet vill vi visa texten på franska om det är mottagarens favoritspråk.

   ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Lägg till så många varianter som behövs för innehållskomponenten. Du kan växla mellan varianterna när som helst för att kontrollera hur innehållskomponenten visas baserat på deras villkorsregler.

   >[!NOTE]
   >Om inga regler som definieras i varianterna uppfylls när meddelandet skickas, kommer innehållskomponenten att visa innehållet som definierats i **[!UICONTROL Default variant]** från **[!UICONTROL Conditional Content]** fönster.
