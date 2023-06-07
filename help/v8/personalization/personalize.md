---
title: Anpassa ert innehåll i Campaign
description: Läs om hur du anpassar ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Anpassa innehållet{#add-personalization}

## Anpassa ämnesraden i ett meddelande {#personalize-subject-line}

Lägga till personalisering i **[!UICONTROL Subject line]** i meddelandet, följ stegen nedan:

1. Öppna en leverans och klicka på **[!UICONTROL Edit content]**.
1. Klicka på **[!UICONTROL Open personalization dialog]** ikonen till höger om **[!UICONTROL Subject line]** fält för e-post eller **[!UICONTROL Title]** fält för push/SMS-leveranser.

   ![](assets/perso-subject.png){width="600"}

1. Ange ämnesraden eller titeln och välj de anpassningsattribut som ska läggas till.

1. Klicka **[!UICONTROL Confirm]** att validera. Anpassningsattributen läggs till i innehållet.

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

