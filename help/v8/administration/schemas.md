---
title: Arbeta med scheman
description: Lär dig hur du arbetar med scheman.
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Arbeta med scheman {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Scheman"
>abstract="**[!DNL Adobe Campaign]** använder XML-baserade scheman för att definiera den fysiska och logiska datastrukturen i programmet. På den här skärmen kan du visa alla befintliga scheman. Det finns filter som kan användas för att förfina listan, t.ex. bara för redigerbara scheman."

## Om scheman {#about}

**[!DNL Adobe Campaign]** använder XML-baserade scheman för att definiera den fysiska och logiska datastrukturen i programmet. Ett schema är ett XML-dokument som är länkat till en databastabell som definierar:

* SQL-tabellstrukturen (tabellnamn, fält, relationer).
* XML-datastrukturen (element, attribut, hierarki, typer, standardvärden, etiketter).

Scheman spelar en nyckelroll i:

* Mappar programdata till databastabeller.
* Definiera relationer mellan dataobjekt.
* Ange struktur och egenskaper för varje fält.

Varje entitet i Adobe Campaign har ett dedikerat schema som säkerställer datakonsekvens och -organisation.

Detaljerad information om scheman finns i [dokumentationen för kampanjkonsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

## Få åtkomst till scheman i webbanvändargränssnittet {#access}

Scheman är tillgängliga från menyn **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.

![](assets/schemas-list.png)

På den här skärmen kan du visa alla befintliga scheman. Det finns filter som kan användas för att förfina listan, t.ex. bara för redigerbara scheman.

Om du vill öppna ett schema markerar du dess namn. En detaljerad schemavy visas.

![](assets/schema-details.png)

### Schemaöversikt {#overview}

Fliken **[!UICONTROL Overview]** innehåller en allmän vy av schemat:

* Avsnittet **[!UICONTROL Properties]** visar nyckelinformation, till exempel schemanamn, namnområde och associerat tabellnamn.

* Avsnittet **[!UICONTROL Schema definition]** innehåller detaljerad information om schemadefinitionen, t.ex. den primärnyckel som används för dataavstämning och dess länkar till andra tabeller.

  Klicka på knappen **[!UICONTROL Schema preview]** för att visa de olika fälten och länkarna som utgör schemat. På så sätt kan du kontrollera hela strukturen för ett schema. Om schemat har utökats med anpassade fält kan du visualisera alla tillägg.

* Avsnittet **[!UICONTROL Content]** visar XML-innehållet i schemat så att du kan växla mellan källan och den genererade syntaxen.

### Schemadata {#data}

Fliken **[!UICONTROL Data]** innehåller information om schemadata.

![](assets/schemas-data.png)

## Redigera anpassade fält {#fields}

Anpassade fält är ytterligare attribut som läggs till i färdiga scheman via Adobe Campaign-konsolen. Med dem kan du anpassa scheman genom att ta med nya attribut som passar organisationens behov.

Anpassade fält kan visas på olika skärmar, t.ex. profilinformation i webbgränssnittet för Campaign. Du kan styra vilka fält som visas och hur de visas i gränssnittet. Det gör du genom att klicka på knappen **[!UICONTROL Edit custom detail]** på menyn **[!UICONTROL Schemas]**.

![](assets/schemas-custom.png)

Detaljerad information om hur du redigerar anpassade fält i ett schema finns i följande avsnitt: [Konfigurera anpassade fält](../administration/custom-fields.md).
