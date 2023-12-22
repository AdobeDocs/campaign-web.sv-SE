---
audience: end-user
title: Bygg en målgrupp med Campaign rule builder
description: Lär dig hur du arbetar med regelbyggaren
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 9992ae7007b5af80e927dd96b6fff25840d8c3e1
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Arbeta med regelbyggaren {#segment-builder}


Med regelbyggaren kan du definiera målgruppen för leveransen genom att filtrera data i databasen. Du kan använda den för att skapa en målgrupp från ett arbetsflöde med **[!UICONTROL Build audience]** -aktivitet, eller direkt när du skapar en leverans för att skapa en enda målgrupp.

* [Lär dig skapa en målgrupp](create-audience.md)
* [Lär dig skapa en engångspublik för en leverans](one-time-audience.md)

## Paletten

Paletten, som finns till vänster, innehåller alla element som du kan filtrera på för att skapa en målgrupp. Du kan använda sökfältet för att snabbt hitta element. Platserna i paletten måste flyttas till arbetsytan i mitten för att kunna konfigureras och beaktas.

![](assets/segment-builder2.png){width="70%" align="left"}

Paletten är uppdelad i två flikar:

* **Attribut**: den här fliken ger dig åtkomst till alla tillgängliga fält från schemat. Fältlistan beror på målschemat som definierats i e-postmallen.

* **Målgrupper**: på den här fliken kan du filtrera med hjälp av en av de befintliga målgrupperna som definieras i Campaign Classic Console eller från Adobe Experience Platform. [Lär dig övervaka och hantera målgrupper](manage-audience.md)

  >[!NOTE]
  >
  >Om du vill utnyttja Adobe Experience Platform målgrupper måste du konfigurera integreringen med Destinations. Se [Dokumentation för Adobe Experience Platform Destinations](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.htmll?lang=sv){target="_blank"}.

## Arbetsytan

Arbetsytan är den centrala zon där du kan konfigurera och kombinera regler baserat på de element som läggs till från paletten. Om du vill lägga till en ny regel drar du en ruta från paletten och släpper den på arbetsytan. Du kan sedan få sammanhangsberoende alternativ beroende på vilken typ av data som läggs till.

![](assets/segment-builder4.png){width="70%" align="left"}

## Rutan Regelegenskaper

På höger sida **Regelegenskaper** kan du utföra de åtgärder som anges nedan.

![](assets/segment-builder5.png){width="70%" align="left"}

* **Visa resultat:** visar en lista över mottagare som målgruppen har.
* **kodvyn**: visar en kodbaserad version av målgruppen i SQL.
* **Visa avancerade attribut**: markera det här alternativet om du vill visa den fullständiga listan med attribut på den vänstra paletten: noder, grupperingar, 1-1 länkar, 1-N länkar.
* **Beräkna**: uppdaterar och visar antalet profiler som din fråga har som mål.
* **Markera eller spara filter**: använd ett fördefinierat filter för att filtrera frågan, eller spara frågan som ett nytt filter för framtida återanvändning. [Lär dig hur du arbetar med fördefinierade filter](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >I den versionen av produkten är vissa fördefinierade filter inte tillgängliga i användargränssnittet. Du kan fortfarande använda dem. [Läs mer](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Attribut**: visar en beskrivning av den skapade målgruppen.

## Exempel

I det här exemplet bygger vi en målgrupp för alla kunder som bor i Atlanta eller Seattle och som är födda efter 1980.

1. I **Attribut** palettens flik, sök efter **Födelsedatum** fält. Dra rutan och släpp den på arbetsytan.

   ![](assets/segment-builder6.png)

1. Välj **Efter** och ange önskat datum.

   ![](assets/segment-builder7.png)

1. På paletten söker du efter **Ort** och lägg till det på arbetsytan under den första regeln.

   ![](assets/segment-builder8.png)

1. Ange namnet på den första orten i textfältet och tryck sedan på Retur.

   ![](assets/segment-builder9.png)

1. Upprepa den här åtgärden för namnet på den andra staden.

   ![](assets/segment-builder10.png)

1. Klicka **Visa resultat** för att visa listan och antalet mottagare som matchar frågan. Du kan också lägga till kolumner för att visa och kontrollera data. I vårt exempel lägger du till **Ort** i Atlanta och Seattle.

   ![](assets/segment-builder11.png)

1. Klicka **Bekräfta**.