---
title: Skapa villkorsstyrt innehåll
description: Lär dig hur du definierar villkor för att anpassa ditt innehåll i Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Skapa villkorsstyrt innehåll{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Lägga till villkorligt innehåll"
>abstract="Konfigurera villkorsstyrda innehållsfält för att skapa avancerad dynamisk personalisering baserat på mottagarens profildata. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt."

## Kom igång med villkorsstyrt innehåll {#gs}

Villkorligt innehåll är en kraftfull funktion som gör att du kan skapa dynamisk personalisering baserat på mottagarens profildata och automatiskt ersätta textblock och bilder när vissa villkor uppfylls. Den här funktionen kan lyfta era kampanjer till nya höjder och leverera målinriktade, personaliserade upplevelser till er målgrupp.

Genom att konfigurera fält för villkorligt innehåll kan du skapa avancerad dynamisk personalisering som till exempel baseras på mottagarens profil. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt. Du kan t.ex. visa&quot;Herr&quot; eller&quot;fru&quot; enligt värdet i fältet Kön i Adobe Campaign-databasen, eller inkludera en annan länk baserat på vilket mottagarspråk som föredras.

Om du vill skapa villkorsstyrt innehåll måste du skapa villkor i **uttrycksredigeraren** med hjälp av specifika hjälpfunktioner. Den här metoden är tillgänglig för alla leveranskanaler, i alla fält där du kan komma åt uttrycksredigeraren, till exempel ämnesraden, e-postlänkar och text-/knappinnehållskomponenter. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md#access)

Förutom uttrycksredigeraren kan du använda en dedikerad **villkorsstyrd innehållsbyggare** när du utformar ett e-postmeddelande som gör att du kan skapa flera varianter för ett element i din e-postbrödtext. [Lär dig hur du skapar villkorligt innehåll i e-postmeddelanden](#condition-condition-builder)

## Skapa villkor i uttrycksredigeraren {#condition-perso-editor}

Följ stegen nedan för att definiera villkorligt innehåll för en leverans med uttrycksredigeraren. I det här exemplet vill vi skapa villkorligt innehåll baserat på mottagarens språk (franska eller engelska).

1. Öppna en leverans och navigera till delen för innehållsredigering.

1. Leta reda på fältet där du vill lägga till villkorligt innehåll. Du kan till exempel lägga till villkorligt innehåll i ett SMS-meddelande.

1. Klicka på ikonen **[!UICONTROL Open personalization dialog]** bredvid fältet för att öppna uttrycksredigeraren.

   ![](assets/open-perso-editor-sms.png){zoomable="yes"}

1. Gå till menyn **[!UICONTROL Conditions]** till vänster i personaliseringsredigeraren.

1. Klicka på plustecknet bredvid funktionen **If** för att börja skapa ditt villkor. Följande rad har lagts till på den centrala skärmen:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersätt `<FIELD>` med ett anpassningsfält, till exempel mottagarens språk: `recipient.language`.
   * Ersätt `<VALUE>` med värdet som ska uppfyllas. Exempel: `'French'`.
   * Ersätt `Ìnsert content here` med det innehåll som du vill visa i de profiler som uppfyller det angivna villkoret.

     ![](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. Ange det innehåll som ska visas om mottagarna inte uppfyller villkoret. Använd en hjälpfunktion för **else** för att göra detta:

   1. Placera markören före uttryckets avslutande tagg `%>` och klicka på `+` bredvid funktionen **Annars**.

   1. Ersätt `Ìnsert content here` med det innehåll som du vill visa i de profiler som inte uppfyller if-funktionens villkor.

   ![](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   Du kan också använda hjälpfunktionen **else if** för att skapa villkor med flera innehållsvarianter. Uttrycket nedan visar till exempel tre varianter av ett meddelande beroende på mottagarens språk:

   ![](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >Varje gång en hjälpfunktion läggs till läggs taggar för att öppna (`<%`) och stänga (`%>`) automatiskt till före och efter funktionen.
   >
   >Exempel efter att du har lagt till en Else-hjälpfunktion i ett uttryck: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Se till att du tar bort de här taggarna för att undvika syntaxfel. I det här exemplet är det korrigerade uttrycket efter att funktionstaggarna **else** har tagits bort:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. När villkoret är klart kan du spara innehållet och kontrollera återgivningen genom att simulera innehållet.

## Skapa villkorligt innehåll i e-postmeddelanden {#condition-condition-builder}

Villkorligt innehåll i e-postmeddelanden kan skapas på två sätt:
* I uttrycksredigeraren genom att skapa ett villkor med hjälpfunktioner,
* I en dedikerad villkorsstyrd innehållsbyggare som är tillgänglig när du utformar ett e-postmeddelande.

Följande avsnitt innehåller stegvisa instruktioner om hur du skapar villkor med funktionen för att skicka villkorsstyrt Designer-innehåll via e-post. Detaljerad information om hur du skapar villkor med uttrycksredigeraren finns [här](#condition-perso-editor).

I det här exemplet vill vi skapa ett e-postmeddelande med flera varianter baserade på mottagarens språk. Följ de här stegen:

1. Skapa eller öppna en e-postleverans, redigera innehållet och klicka på knappen **[!UICONTROL Edit email body]** för att öppna arbetsytan för e-postdesign.

1. Markera en innehållskomponent och klicka på ikonen **[!UICONTROL Enable conditional content]**.

   ![](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. **[!UICONTROL Conditional Content]**-rutan öppnas till vänster på skärmen. I den här rutan kan du skapa flera varianter av den markerade innehållskomponenten med villkor.

1. Konfigurera din första variant. Håll pekaren över **[!UICONTROL Variant - 1]** i rutan **[!UICONTROL Conditional Content]** och klicka på knappen **[!UICONTROL Add condition]**.

   ![](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. Frågemodelleraren öppnas. Det gör att du kan skapa ett villkor genom att filtrera mottagarens profildata. [Lär dig arbeta med frågemodelleraren](../query/query-modeler-overview.md).

   När villkoret för den första varianten av meddelandet är klart klickar du på **[!UICONTROL Confirm]**. I det här exemplet skapar vi en regel som riktar sig till mottagare vars språk är &quot;franska&quot;.

   ![](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. Regeln är nu associerad med varianten. För bättre läsbarhet rekommenderar vi att du byter namn på varianten genom att klicka på ellipsmenyn.

1. Konfigurera hur komponenten ska visas om regeln uppfylls när meddelandet skickas. I det här exemplet vill vi visa texten på franska om det är mottagarens favoritspråk.

   ![](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. Lägg till så många varianter som behövs för innehållskomponenten. Du kan växla mellan varianterna när som helst för att kontrollera hur innehållskomponenten visas baserat på deras villkorsregler.

   >[!NOTE]
   >Om ingen av reglerna som definieras i varianterna uppfylls när meddelandet skickas, kommer innehållskomponenten att visa innehållet som definierats i **[!UICONTROL Default variant]** från rutan **[!UICONTROL Conditional Content]**.

## Använd variabler för villkorligt innehåll {#variables-conditional}

Variablerna kan användas för villkorligt innehåll i leveransen.

Läs mer om att [lägga till variabler i en leverans](../advanced-settings/delivery-settings.md#variables-delivery).

Välj det element där du vill placera ett villkorligt innehåll.

![](assets/variables-conditional.png){zoomable="yes"}

Om du vill använda variabeln konfigurerar du villkoret med knappen **[!UICONTROL Edit expression]**, som visas nedan.
I det här exemplet visas den här bilden när variabelvärdet är `launch`.

![](assets/variables-condition.png){zoomable="yes"}

Du kan också skapa en annan variant med värdet `reminder`, till exempel där en annan bild visas.
