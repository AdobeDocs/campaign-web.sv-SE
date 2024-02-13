---
title: Arbeta med fördefinierade filter
description: Lär dig hur du skapar och hanterar fördefinierade filter i Adobe Campaign Web
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: 97b6de0763dbeb133d7d0346e6af4d056cc731e3
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Arbeta med fördefinierade filter {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Fördefinierad filterhantering"
>abstract="Campaign Web-gränssnittet har ett användarvänligt gränssnitt där du enkelt kan hantera och anpassa fördefinierade filter efter just dina behov. Skapa en gång och spara för framtida bruk."


<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card4"
>title="Fördefinierad filterhantering"
>abstract="Campaign Web har nu ett användarvänligt gränssnitt där ni enkelt kan hantera och anpassa fördefinierade filter efter just era behov. Skapa en gång och spara för framtida bruk."

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Fördefinierade filter"
>abstract="Campaign Web-gränssnittet är ett användarvänligt gränssnitt där du enkelt kan hantera och anpassa fördefinierade filter efter just dina behov. Skapa en gång och spara för framtida bruk."

Fördefinierade filter är anpassade filter som skapas och sparas för att vara tillgängliga för framtida bruk. De kan användas som genvägar under alla filtreringsåtgärder med frågemodelleraren, t.ex. när en lista med data filtreras eller när målgruppen för en leverans skapas.

Du kan använda befintliga inbyggda filter för att få tillgång till en viss delmängd av dina data, eller skapa egna fördefinierade filter och spara dem.

![](assets/predefined-filters-menu.png){zoomable=&quot;yes&quot;}{zoomable=&quot;yes&quot;}

## Skapa ett fördefinierat filter {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Skapa ett fördefinierat filter"
>abstract="Ange en etikett för det fördefinierade filtret och markera den tabell det gäller. Öppna de andra alternativen för att lägga till en beskrivning och ange det här filtret som en favorit. Använd sedan knappen Skapa regel för att definiera filtervillkoren."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Skapa fördefinierade filterregler"
>abstract="Om du vill definiera filtervillkoren för det anpassade filtret klickar du på knappen Skapa regel."

### Skapa ett filter från frågemodelleraren {#create-from-rule-builder}

Du kan spara ett eget filter från [frågemodellerare](../query/query-modeler-overview.md) för framtida bruk. Följ de här stegen:

1. Öppna frågemodelleraren och definiera filtervillkoren. I exemplet nedan filtrerar du mottagare som bor i Madrid och prenumererar på ett nyhetsbrev.
1. Klicka på **Markera eller spara filter** och markera **Spara som ett filter**.

   ![](assets/predefined-filters-save.png){zoomable=&quot;yes&quot;}

1. Välj **Skapa ett nytt filter** och ange ett namn och en beskrivning för filtret.

   ![](assets/predefined-filters-save-filter.png){zoomable=&quot;yes&quot;}

   Du kan spara filtret som en favorit om det behövs. Läs mer i [det här avsnittet](#fav-filter).

1. Klicka **Bekräfta** för att spara ändringarna.

Ditt anpassade filter finns nu i **Fördefinierade filter** och är tillgängliga för alla Campaign-användare.


### Skapa ett filter från filterlistan {#create-filter-from-list}

Du kan skapa ett filter från **Fördefinierade filter** i den vänstra menyn. Gör så här:

1. Sök i **Fördefinierade filter** i den vänstra menyn.
1. Klicka på **Skapa filter** -knappen.
1. Ange filternamnet och, från **Dokumenttyp** markerar du det schema det gäller för. Standardschemat är `Recipients(nms)`.


1. Definiera regeln för filtret. Till exempel profiler äldre än 30.

   ![](assets/filter-30+.png){zoomable=&quot;yes&quot;}


1. Spara ändringarna.

   ![](assets/new-filter.png){zoomable=&quot;yes&quot;}


Filtret läggs till i den fördefinierade filterlistan. Du kan spara filtret som en favorit om det behövs. Läs mer i [det här avsnittet](#fav-filter).


## Spara filtret som en favorit {#fav-filter}

När du skapar ett fördefinierat filter kan du aktivera **Spara som favorit** om du vill se det här fördefinierade filtret i dina favoriter.


När ett filter sparas som favorit är det tillgängligt för alla användare i **Favoritfilter** i listan där filter skapas, enligt nedan:

![](assets/predefined-filters-favorite.png){zoomable=&quot;yes&quot;}{width="30%" align="left"}

## Använda ett fördefinierat filter {#use-predefined-filter}

Fördefinierade filter är tillgängliga när du definierar regelegenskaper. Om du vill komma åt fördefinierade filter väljer du **Välj eget filter** i listrutan för frågemodelleraren.

Du kan sedan komma åt den fullständiga listan med fördefinierade filter som är tillgängliga för den aktuella kontexten och använda kortkommandon som finns i **Favoritfilter** i listrutan. Läs mer om favoriter i [det här avsnittet](#fav-filter).

Om du till exempel vill skapa en målgrupp från ett fördefinierat filter följer du de här stegen:

1. Gå till **Målgrupper** i den vänstra menyn och klicka på **Skapa publik** i det övre vänstra hörnet av målgruppslistan.
1. Ange målgruppens namn och klicka på **Skapa publik** -knappen.
1. Välj **Fråga** och, från den högra rutan, klicka på **Skapa målgrupper** -knappen.

   ![](assets/build-audience-from-filter.png){zoomable=&quot;yes&quot;}

1. Från **Markera eller spara filter** klickar du på **Välj eget filter** alternativ.

   ![](assets/build-audience-select-custom-filter.png){zoomable=&quot;yes&quot;}

1. Bläddra till det fördefinierade filtret som du vill använda för att skapa målgruppen, markera det och bekräfta.

   ![](assets/build-audience-filter-list.png){zoomable=&quot;yes&quot;}

1. Kontrollera regelegenskaperna för det här filtret och bekräfta.

   Filtret används nu som en fråga i **Fråga** aktivitet.

   ![](assets/build-audience-confirm.png){zoomable=&quot;yes&quot;}

1. Spara ändringarna och klicka på **Starta** för att bygga upp målgruppen och göra den tillgänglig i målgruppslistan.

## Hantera dina fördefinierade filter {#manage-predefined-filter}

Alla fördefinierade filter grupperas tillsammans i den dedikerade posten på den vänstra navigeringsmenyn.

![](assets/list-of-filters.png){zoomable=&quot;yes&quot;}

I den här listan kan du skapa ett nytt filter enligt beskrivningen ovan och utföra följande åtgärder:

* Redigera ett befintligt filter, ändra dess regler och egenskaper.
* Duplicera ett fördefinierat filter.
* Ta bort ett fördefinierat filter.

Du kan också lägga till ett fördefinierat filter som favorit för att få snabb åtkomst när du skapar målgrupper. Läs mer i [det här avsnittet](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->
