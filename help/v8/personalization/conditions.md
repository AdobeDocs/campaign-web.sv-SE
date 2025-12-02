---
title: Skapa villkorsstyrt innehåll
description: Lär dig hur du definierar villkor för att anpassa ditt innehåll i Adobe Campaign Web
feature: Personalization
topic: Personalization
old-role: Data Engineer
role: Developer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Skapa villkorsstyrt innehåll {#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Lägga till villkorligt innehåll"
>abstract="Konfigurera villkorsstyrda innehållsfält för att skapa avancerad dynamisk personalisering baserat på mottagarens profildata. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt."

## Kom igång med villkorsstyrt innehåll {#gs}

Villkorligt innehåll är en kraftfull funktion som möjliggör dynamisk personalisering baserat på mottagarens profildata. Det ersätter automatiskt textblock och bilder när vissa villkor uppfylls. Den här funktionen förbättrar kampanjer och levererar målinriktade, personaliserade upplevelser till er målgrupp.

Genom att konfigurera fält för villkorligt innehåll kan du skapa avancerad dynamisk personalisering baserat på mottagarens profil. Textblock, länkar, ämnesrader och bilder ersätts till exempel i meddelandeinnehållet när ett visst villkor uppfylls. Du kan t.ex. visa&quot;Herr&quot; eller&quot;fru&quot; enligt värdet i fältet Kön i Adobe Campaign-databasen eller inkludera en annan länk utifrån mottagarens favoritspråk.

Om du vill skapa villkorsstyrt innehåll konfigurerar du villkoren i **uttrycksredigeraren** med hjälp av specifika hjälpfunktioner. Den här metoden är tillgänglig för alla leveranskanaler, i alla fält där du kan komma åt uttrycksredigeraren, till exempel ämnesraden, e-postlänkar och text-/knappinnehållskomponenter. [Lär dig hur du kommer åt uttrycksredigeraren](gs-personalization.md#access).

Använd dessutom den dedikerade **villkorliga innehållsbyggaren** när du utformar ett e-postmeddelande för att skapa flera varianter för ett element i din e-postbrödtext. [Lär dig hur du skapar villkorligt innehåll i e-postmeddelanden](#condition-condition-builder).

## Skapa villkor i uttrycksredigeraren {#condition-perso-editor}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_conditions"
>title="Villkor"
>abstract="På den här menyn kan du använda hjälpfunktioner för att definiera villkorat innehåll."

Följ de här stegen för att definiera villkorligt innehåll för en leverans med uttrycksredigeraren. I det här exemplet skapas villkorligt innehåll baserat på mottagarens språk (franska eller engelska).

1. Öppna en leverans och navigera till delen för innehållsredigering.

1. Leta reda på fältet där du vill lägga till villkorligt innehåll. Du kan till exempel lägga till villkorligt innehåll i ett SMS-meddelande.

1. Klicka på ikonen **[!UICONTROL Open personalization dialog]** bredvid fältet för att öppna uttrycksredigeraren.

   ![Skärmbild som visar ikonen Öppna personalisering bredvid fältet i SMS-meddelanderedigeraren.](assets/open-perso-editor-sms.png){zoomable="yes"}

1. Gå till menyn **[!UICONTROL Conditions]** till vänster i personaliseringsredigeraren.

1. Klicka på plustecknet bredvid funktionen **If** för att börja skapa ditt villkor. Följande rad har lagts till på den centrala skärmen: `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersätt `<FIELD>` med ett anpassningsfält, till exempel mottagarens språk: `recipient.language`.
   * Ersätt `<VALUE>` med värdet som ska uppfyllas, till exempel `'French'`.
   * Ersätt `Insert content here` med innehållet som ska visas i profiler som uppfyller det angivna villkoret.

     ![Skärmbild som visar ett exempelvillkor i uttrycksredigeraren med platshållare för fält, värde och innehåll.](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. Ange vilket innehåll som ska visas om mottagarna inte uppfyller villkoret. Använd en **else**-hjälpfunktion:

   1. Placera markören före uttryckets avslutande tagg `%>` och klicka på `+` bredvid funktionen **Annars**.

   1. Ersätt `Insert content here` med det innehåll som ska visas i profiler som inte uppfyller if-funktionens villkor.

   ![Skärmbild som visar Else-funktionen som lagts till i villkoret i uttrycksredigeraren.](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   Använd hjälpfunktionen **else if** om du vill skapa villkor med flera innehållsvarianter. Uttrycket nedan visar till exempel tre varianter av ett meddelande beroende på mottagarens språk:

   ![Skärmbild som visar ett villkor med flera varianter baserade på mottagarens språk.](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >Varje gång en hjälpfunktion läggs till läggs taggar för att öppna (`<%`) och stänga (`%>`) automatiskt till före och efter funktionen.
   >
   >Exempel efter att du har lagt till en Else-hjälpfunktion i ett uttryck:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Se till att du tar bort de här taggarna för att undvika syntaxfel. I det här exemplet är det korrigerade uttrycket efter att funktionstaggarna **else** har tagits bort:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Spara innehållet och kontrollera återgivningen genom att simulera innehållet.

## Skapa villkorligt innehåll i e-postmeddelanden {#condition-condition-builder}

Villkorligt innehåll i e-postmeddelanden kan skapas på två sätt:
* I uttrycksredigeraren skapar du ett villkor med hjälpfunktioner.
* I en dedikerad villkorsstyrd innehållsbyggare som är tillgänglig när du utformar ett e-postmeddelande.

Följande avsnitt innehåller stegvisa instruktioner om hur du skapar villkor med funktionen för villkorligt Designer-innehåll. Detaljerad information om hur du skapar villkor med uttrycksredigeraren finns [här](#condition-perso-editor).

I det här exemplet skapas ett e-postmeddelande med flera varianter baserat på mottagarens språk. Följ de här stegen:

1. Skapa eller öppna en e-postleverans, redigera innehållet och klicka på knappen **[!UICONTROL Edit email body]** för att öppna arbetsytan för e-postdesign.

1. Markera en innehållskomponent och klicka på ikonen **[!UICONTROL Enable conditional content]**.

   ![Skärmbild med ikonen Aktivera villkorligt innehåll i e-postdesignern.](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. **[!UICONTROL Conditional Content]**-rutan öppnas till vänster på skärmen. I den här rutan skapar du flera varianter av den markerade innehållskomponenten med villkor.

1. Konfigurera din första variant. Håll pekaren över **[!UICONTROL Variant - 1]** i rutan **[!UICONTROL Conditional Content]** och klicka på knappen **[!UICONTROL Add condition]**.

   ![Skärmbild med knappen Lägg till villkor i rutan Villkorligt innehåll.](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. Frågemodelleraren öppnas så att du kan skapa ett villkor genom att filtrera mottagarens profildata. [Lär dig arbeta med frågemodelleraren](../query/query-modeler-overview.md).

   När villkoret för den första varianten av meddelandet är klart klickar du på **[!UICONTROL Confirm]**. I det här exemplet skapas en regel som riktar sig till mottagare vars språk är franska.

   ![Skärmbild som visar ett villkor för mottagare vars språk är franska.](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. Regeln är nu associerad med varianten. För bättre läsbarhet byter du namn på varianten genom att klicka på ellipsmenyn.

1. Konfigurera hur komponenten ska visas om regeln uppfylls när meddelandet skickas. I det här exemplet visar du texten på franska om det är mottagarens favoritspråk.

   ![Skärmbild som visar den franska textvarianten i e-postdesignern.](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. Lägg till så många varianter som behövs för innehållskomponenten. Växla mellan varianterna när som helst för att kontrollera hur innehållskomponenten visas baserat på deras villkorsregler.

   >[!NOTE]
   >Om ingen av reglerna som definieras i varianterna uppfylls när meddelandet skickas, kommer innehållskomponenten att visa innehållet som definierats i **[!UICONTROL Default variant]** från rutan **[!UICONTROL Conditional Content]**.

## Använd variabler för villkorligt innehåll {#variables-conditional}

Variabler kan användas för villkorligt innehåll i leveransen.

Läs mer om att [lägga till variabler i en leverans](../advanced-settings/delivery-settings.md#variables-delivery).

Välj det element där du vill placera villkorligt innehåll.

![Skärmbild som visar användningen av variabler för villkorat innehåll.](assets/variables-conditional.png){zoomable="yes"}

Om du vill använda variabeln konfigurerar du villkoret med knappen **[!UICONTROL Edit expression]**, som visas nedan. I det här exemplet visas den här bilden när variabelvärdet är `launch`.

![Skärmbild som visar ett villkor med hjälp av en variabel med värdet &#39;launch&#39;.](assets/variables-condition.png){zoomable="yes"}

Skapa en annan variant med värdet `reminder`, till exempel där en annan bild visas.