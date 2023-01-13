---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 0d74cababf2b4d66d3b2ce9b0ae2a0f00cb1cdef
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Anpassa innehållet{#add-personalization}

![](../assets/do-not-localize/badge.png)

Du kan anpassa meddelandeinnehållet genom att:

* Infoga dynamisk **personaliseringsfält**

   Anpassningsfält används för personalisering på första nivån av dina meddelanden. Du kan välja vilket fält som helst tillgängligt i databasen från personaliseringsredigeraren. För en leverans kan du välja vilket fält som helst som är relaterat till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten.

   ![](assets/perso-subject-line.png)

   Följande syntax infogar mottagarens ort i ditt innehåll: &lt;%= mottagare.location.city %>.

* Infoga fördefinierad **innehållsblock**

   Campaign innehåller en uppsättning personaliseringsblock som innehåller en specifik återgivning som du kan infoga i dina leveranser. Du kan till exempel lägga till en logotyp, ett hälsningsmeddelande eller en länk till meddelandets spegelsida. Innehållsblock är tillgängliga från ett dedikerat tävlingsbidrag via personaliseringsredigeraren.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Anpassa ämnesraden för e-post {#personalize-subject-line}

Lägga till personalisering i **[!UICONTROL Subject line]** i meddelandet, följ stegen nedan:

1. Klicka på **Öppna dialogrutan för personalisering** ikonen till höger om **Subject line** fält.
1. Ange innehållet på ämnesraden och välj de anpassningsattribut som ska läggas till.
1. Klicka **Bekräfta** att validera. Anpassningsattributen läggs till på ämnesraden.

![](assets/perso-subject.png)

## Anpassa e-postinnehållet {#personalize-emails}

Om du vill anpassa e-postinnehållet öppnar du meddelandet i e-postdesignern och:

1. Klicka inuti ett textblock.
1. Välj **Lägg till personalisering**.

   ![](assets/perso-add-to-content.png)

1. Ange namnet på mottagaren i personaliseringsredigeraren och bekräfta.

   ![](assets/perso-add-name.png)

   Anpassningsattributet läggs till i e-postinnehållet.

   Du kan simulera innehållet för att kontrollera återgivningen. [Läs mer](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## Anpassa länkar i e-postmeddelanden {#personalize-links}

För att personalisera en **link**:

1. Markera ett textblock eller en bild.
1. Välj **Lägg till personalisering**.

   ![](assets/perso-link.png)

1. Använd personaliseringsredigeraren för att definiera och personalisera länken.

## Anpassa era erbjudanden {#personalize-offers}

Du kan även komma åt personaliseringsredigeraren när du lägger till textinnehåll till offerternas representationer. Läs mer i [det här avsnittet](../content/offers.md).
