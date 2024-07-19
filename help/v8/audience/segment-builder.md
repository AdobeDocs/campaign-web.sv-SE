---
audience: end-user
title: Bygg en målgrupp med Campaign rule builder
description: Lär dig hur du arbetar med regelbyggaren
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Arbeta med regelbyggaren {#segment-builder}

Med regelbyggaren kan du definiera målgruppen för leveransen genom att filtrera data i databasen. Du kan använda den för att skapa en målgrupp antingen från ett arbetsflöde med en **[!UICONTROL Build audience]**-aktivitet eller direkt när du skapar en leverans för att skapa en engångspublik.

* [Lär dig hur du skapar och sparar en publik](create-audience.md)
* [Lär dig skapa en engångspublik för en leverans](one-time-audience.md)

## Paletten

Paletten, som finns till vänster, innehåller alla element som du kan filtrera på för att skapa en målgrupp. Du kan använda sökfältet för att snabbt hitta element. Platserna i paletten måste flyttas till arbetsytan i mitten för att kunna konfigureras och beaktas.

![](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

Paletten är uppdelad i två flikar:

* **Attribut**: På den här fliken kan du komma åt alla tillgängliga fält från schemat. Fältlistan beror på målschemat som definierats i e-postmallen.

* **Publiker**: På den här fliken kan du filtrera med en av de befintliga målgrupperna som definieras i Campaign Classic Console eller från Adobe Experience Platform. Lär dig övervaka och hantera målgrupper i [det här avsnittet](manage-audience.md)

  >[!NOTE]
  >
  >Om du vill utnyttja Adobe Experience Platform målgrupper måste du konfigurera integreringen med Destinations. Mer information finns i [Adobe Experience Platform Destinations-dokumentationen](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.htmll?lang=sv){target="_blank"}.

## Arbetsytan

Arbetsytan är den centrala zon där du kan konfigurera och kombinera regler baserat på de element som läggs till från paletten. Om du vill lägga till en ny regel drar du en ruta från paletten och släpper den på arbetsytan. Du kan sedan få sammanhangsberoende alternativ beroende på vilken typ av data som läggs till.

![](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## Rutan Regelegenskaper

På höger sida kan du utföra de åtgärder som anges nedan i rutan **Regelegenskaper**.

![](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Visa resultat:** visar listan med profiler som målgruppen har.
* **Kodvyn**: visar en kodbaserad version av målgruppen i SQL.
* **Visa avancerade attribut**: Markera det här alternativet om du vill visa den fullständiga listan med attribut på den vänstra paletten: noder, grupperingar, 1-1 länkar, 1-N länkar.
* **Beräkna**: uppdaterar och visar antalet profiler som din fråga har som mål.
* **Välj eller spara filter**: använd ett fördefinierat filter för att filtrera frågan, eller spara frågan som ett nytt filter för framtida återanvändning. [Lär dig arbeta med fördefinierade filter](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >I den versionen av produkten är vissa fördefinierade filter inte tillgängliga i användargränssnittet. Du kan fortfarande använda dem. [Läs mer](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Attribut**: visar en beskrivning av den skapade målgruppen.

## Exempel

I det här exemplet bygger vi en målgrupp för alla kunder som bor i Atlanta eller Seattle och som är födda efter 1980.

1. Sök efter fältet **Födelsedatum** på fliken **Attribut** på paletten. Dra rutan och släpp den på arbetsytan.

   ![](assets/segment-builder6.png){zoomable="yes"}

1. Välj operatorn **Efter** på arbetsytan och ange önskat datum.

   ![](assets/segment-builder7.png){zoomable="yes"}

1. På paletten söker du efter fältet **Ort** och lägger till det på arbetsytan nedanför den första regeln.

   ![](assets/segment-builder8.png){zoomable="yes"}

1. Ange namnet på den första orten i textfältet och tryck sedan på Retur.

   ![](assets/segment-builder9.png){zoomable="yes"}

1. Upprepa den här åtgärden för namnet på den andra staden.

   ![](assets/segment-builder10.png){zoomable="yes"}

1. Klicka på **Visa resultat** för att visa listan och antalet mottagare som matchar frågan. Du kan också lägga till kolumner för att visa och kontrollera data. Lägg till kolumnen **City** i vårt exempel och se Atlanta och Seattle.

   ![](assets/segment-builder11.png){zoomable="yes"}

1. Klicka på **Bekräfta**.