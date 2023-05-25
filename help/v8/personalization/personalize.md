---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 048f754005744bcab5b64f265e9e9cdf9776dca8
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---


# Anpassa innehållet{#add-personalization}

Du kan anpassa meddelandeinnehållet genom att:

* Infoga dynamisk **personaliseringsfält**

   Anpassningsfält används för personalisering på första nivån av dina meddelanden. Du kan välja vilket fält som helst tillgängligt i databasen från personaliseringsredigeraren. För en leverans kan du välja vilket fält som helst som är relaterat till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten.

   ![](assets/perso-subject-line.png)

   Följande syntax infogar mottagarens ort i ditt innehåll: &lt;%= mottagare.location.city %>.

* Infoga fördefinierad **innehållsblock**

   Campaign innehåller en uppsättning personaliseringsblock som innehåller en specifik återgivning som du kan infoga i dina leveranser. Du kan till exempel lägga till en logotyp, ett hälsningsmeddelande eller en länk till meddelandets spegelsida. Innehållsblock är tillgängliga från ett dedikerat tävlingsbidrag via personaliseringsredigeraren.

   ![](assets/perso-content-blocks.png)

* Skapa **villkorligt innehåll**

   Konfigurera villkorsstyrt innehåll för att lägga till dynamisk personalisering baserat på mottagarens profil till exempel. Textblock och/eller bilder infogas när ett visst villkor är true.


## Anpassa ämnesraden för e-post {#personalize-subject-line}

Lägga till personalisering i **[!UICONTROL Subject line]** i meddelandet, följ stegen nedan:

1. Klicka på **[!UICONTROL Open personalization dialog]** ikonen till höger om **[!UICONTROL Subject line]** fält.

   ![](assets/perso-subject.png){width="600"}

1. Ange innehållet på ämnesraden och välj de anpassningsattribut som ska läggas till.

1. Klicka **[!UICONTROL Confirm]**** för att validera. Anpassningsattributen läggs till på ämnesraden.

## Anpassa e-postinnehållet {#personalize-emails}

Om du vill anpassa e-postinnehållet öppnar du meddelandet i e-postdesignern och:

1. Klicka inuti ett textblock.
1. Välj **[!UICONTROL Add personalization]**.

   ![](assets/perso-add-to-content.png)

1. Ange namnet på mottagaren i personaliseringsredigeraren och bekräfta.

   ![](assets/perso-add-name.png)

   Anpassningsattributet läggs till i e-postinnehållet.

   Du kan simulera innehållet för att kontrollera återgivningen. [Läs mer](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. Om du vill lägga till ett innehållsblock i e-postmeddelandet följer du samma steg och väljer ett innehållsblock från den sista ikonen:

   ![](assets/perso-insert-block.png)

1. När innehållsblocket har infogats läggs det till i e-postinnehållet. Det anpassas automatiskt till mottagarprofilen när personalisering skapas, i leveransförberedelsesteget.

   ![](assets/perso-content-block-in-email.png)

## Anpassa länkar i e-postmeddelanden {#personalize-links}

För att personalisera en **link**:

1. Markera ett textblock eller en bild.
1. Välj **Infoga länk**.

   ![](assets/perso-link.png)

1. Ange länketiketten och använd **Infoga länk** för att anpassa länken.

   ![](assets/perso-link-insert-icon.png)

1. Använd personaliseringsredigeraren för att definiera och anpassa länken och bekräfta.

   ![](assets/perso-link-edit.png)


## Anpassa era erbjudanden {#personalize-offers}

Du kan även komma åt personaliseringsredigeraren när du lägger till textinnehåll till offerternas representationer. Läs mer i [det här avsnittet](../content/offers.md).

## Inbyggda innehållsblock {#ootb-content-blocks}

Inbyggda innehållsblock är:

* **[!UICONTROL Enabled by Adobe Campaign]**: infogar logotypen&quot;Enabled by Adobe Campaign&quot;.
* **[!UICONTROL Formatting function for proper nouns]**: genererar **[!UICONTROL toSmartCase]** Javascript-funktionen, som ändrar den första bokstaven i varje ord till versaler.
* **[!UICONTROL Greetings]**: infogar hälsningar med mottagarens fullständiga namn följt av ett kommatecken. Exempel: &quot;Hej John Doe.&quot;
* **[!UICONTROL Insert logo]**: infogar en logotyp som är definierad i instansinställningarna.
* **[!UICONTROL Link to mirror page]**: infogar en länk till [spegelsida](../content/mirror-page.md). Standardformatet är: &quot;Om du inte kan visa det här meddelandet korrekt klickar du här&quot;.
* **[!UICONTROL Mirror page URL]**: infogar spegelsidans URL, vilket gör att leveransdesigners kan kontrollera länken.
* **[!UICONTROL Offer acceptance URL in unitary mode]**: infogar en URL som gör att ett erbjudande kan anges till **[!UICONTROL Accepted]**. (Det här blocket är tillgängligt om interaktionsmodulen är aktiverad)
* **[!UICONTROL Registration confirmation]**: infogar en länk som bekräftar prenumerationen.
* **[!UICONTROL Registration link]**: infogar en prenumerationslänk. Den här länken definieras i instansinställningarna. Standardinnehållet är: &quot;Registrera dig genom att klicka här.&quot;
* **[!UICONTROL Registration link (with referrer)]**: infogar en prenumerationslänk som gör det möjligt att identifiera besökaren och leveransen. Den här länken definieras i instansinställningarna.
* **[!UICONTROL Registration page URL]**: infogar en prenumerations-URL
* **[!UICONTROL Style of content emails]** och **[!UICONTROL Notification style]**: generera kod som formaterar ett e-postmeddelande med fördefinierade HTML-format.
* **[!UICONTROL Unsubscription link]**: infogar en länk som gör det möjligt att avbryta prenumerationen på alla leveranser (blockeringslista). Standardinnehållet är: &quot;Du får det här meddelandet eftersom du har haft kontakt med ***ditt organisationsnamn*** eller ett närstående bolag. Ta inte längre emot meddelanden från ***ditt organisationsnamn*** klicka här.&quot;
