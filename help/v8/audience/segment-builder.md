---
audience: end-user
title: Arbeta med segmentbyggaren
description: Webbdokumentation för Campaign v8
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: bf55b13011f7d2bdafcc55b1b2539c4ce590dd85
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Arbeta med segmentbyggaren {#segment-builder}

>[!NOTE]
>
>Dokumentationen håller på att byggas och uppdateras ofta. Den slutliga versionen av detta innehåll är klar i januari 2023.

I det här avsnittet beskrivs hur du skapar en målgrupp när du utformar ett nytt e-postmeddelande. Den skapade målgruppen kan bara användas i det här e-postmeddelandet.

Med segmentbyggaren kan du definiera den målgrupp som meddelandet riktar sig till genom att filtrera data i Adobe Campaign-databasen. Om du vill välja en befintlig målgrupp kan du läsa detta [section](add-audience.md).

Mer information om segmentbyggaren finns i [Dokumentation för segmenteringstjänst](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

Så här skapar du en ny publik när du utformar ett e-postmeddelande:

1. Från **Målgrupp** i leveransguiden klickar du på **[!UICONTROL Select audience]** -knappen.

   ![](assets/segment-builder0.png)

1. Välj **Skapa en egen**. Segmentbyggaren visas.

   ![](assets/segment-builder.png)

## Paletten

Paletten, som finns till vänster, innehåller alla element som du kan filtrera på för att skapa en målgrupp. Platserna i paletten måste flyttas till arbetsytan i mitten för att kunna konfigureras och beaktas. Paletten är uppdelad i två flikar:

* **Attribut**: På den här fliken kan du komma åt alla tillgängliga fält från schemat. Fältlistan beror på målschemat som definierats i e-postmallen.

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **Målgrupper**: På den här fliken kan du filtrera med hjälp av en av de befintliga målgrupperna som definieras i konsolen Campaign Classic.

   ![](assets/segment-builder3.png){width="70%" align="left"}

Du kan använda sökfältet för att snabbt hitta element.

## Arbetsytan

Arbetsytan är den centrala zon där du kan konfigurera och kombinera regler baserat på de element som läggs till från paletten. Om du vill lägga till en ny regel drar du en ruta från paletten och släpper den på arbetsytan. Därefter visas sammanhangsspecifika alternativ beroende på vilken typ av data som läggs till.

![](assets/segment-builder4.png){width="70%" align="left"}

## Rutan Regelegenskaper

Till höger **Regelegenskaper** kan du utföra följande åtgärder:

![](assets/segment-builder5.png){width="70%" align="left"}

* **Visa resultat:** visar listan med mottagare som målgruppen riktar sig till
* **kodvyn**: visar en kodbaserad version av målgruppen i SQL.
* **Visa avancerade attribut**: Markera det här alternativet om du vill visa hela listan med attribut på den vänstra paletten: noder, grupperingar, 1-1 länkar, 1-N länkar.
* **Attribut**: visar en beskrivning av den skapade målgruppen.

## Exempel

I det här exemplet kommer vi att bygga upp en målgrupp för alla kunder som bor i Atlanta eller Seattle och som är födda efter 1980.

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

1. Klicka **Visa resultat** för att visa listan och antalet mottagare som matchar frågan.

   ![](assets/segment-builder11.png)

1. Klicka **Bekräfta**.

Din målgrupp är definierad och klar att användas i ditt e-postmeddelande.