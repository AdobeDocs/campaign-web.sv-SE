---
audience: end-user
title: Välj attribut och lägg till dem i favoriter
description: Lär dig hur du arbetar med attribut och enkelt kommer åt attribut du gillar och nyligen använt.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: c0c9c5da3369e55269411b7348004006cd3c139e
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Välj attribut och lägg till dem i favoriter {#folders}

Med användargränssnittet för Campaign-webben kan användare välja attribut från databasen på olika platser, beroende på vilken åtgärd som utförs. Du kan till exempel välja attribut när du definierar utdatakolumner för en direktpostleverans eller en fil som ska extraheras. På samma sätt kan du välja attribut när du använder frågemodelleraren för att skapa regler, filter eller skapa målgrupper.

![Välj attribut från databasgränssnittet och visa attributalternativ.](assets/attributes-list.png)

Om du snabbt vill återanvända attribut som används ofta lägger du till dem i Favoriter. Detta gör att de är lättillgängliga för framtida uppgifter. Förutom favoriter kan användare visa och använda de senast valda attributen.

Gränssnittet innehåller också ett verktyg för värdedistribution som gör att du kan visualisera fördelningen av ett attributs värden i en tabell. Det här verktyget hjälper till att identifiera värdeintervall och värdefrekvens och säkerställer datakonsekvens när frågor eller uttryck skapas.

## Favoriter och nyligen använda attribut {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favoriter och senaste"
>abstract="Menyn **[!UICONTROL Favorites & Recents]** i attributväljaren innehåller en ordnad vy över attribut som du har lagt till i favoriter, tillsammans med en lista över nyligen använda attribut. Favoritattribut visas först, följt av nyligen använda attribut, vilket gör det enkelt att hitta de attribut du behöver."

Menyn **[!UICONTROL Favorites & Recents]** i attributväljaren innehåller en ordnad vy över attribut som lagts till i favoriter, tillsammans med en lista över nyligen använda attribut. Favoritattribut visas först, följt av nyligen använda attribut, vilket gör det enkelt att hitta de attribut som krävs.

![Favoriter och menyn Senaste attribut, med favoritattribut och nyligen använda attribut.](assets/attributes-favorites.png)

Om du vill lägga till ett attribut i favoriter håller du pekaren över informationsknappen och väljer stjärnikonen. Attributet läggs sedan automatiskt till i favoritlistan. Om du vill ta bort ett attribut från favoriter väljer du stjärnikonen igen.

Användare kan lägga till upp till 20 attribut till favoriter. Favoriter och nyligen använda attribut kopplas till varje användare i en organisation, vilket ger en smidig upplevelse på olika datorer och enheter.

## Identifiera fördelningen av värden i en tabell {#distribution}

Knappen **Distribution av värden**, som är tillgänglig i informationsfönstret för ett attribut, gör att användare kan analysera värdefördelningen för det attributet i tabellen. Den här funktionen är användbar för att förstå tillgängliga värden, antal och procenttal. Det kan också hjälpa dig att undvika problem som inkonsekvent skiftläge eller stavning när du skapar frågor eller skapar uttryck.

![Distribution av värdeverktygsgränssnittet, med antal och procentandelar av attributvärden.](assets/attributes-distribution-values.png)

För attribut med ett stort antal värden visas endast de första tjugo. I sådana fall visas ett **[!UICONTROL Partial load]**-meddelande som indikerar den här begränsningen. Använd avancerade filter för att förfina det visade resultatet och fokusera på specifika värden eller delmängder av data. Detaljerad vägledning om hur du använder filter finns [här](../get-started/work-with-folders.md#filter-the-values).

Mer information om hur du använder värdefördelningsverktyget i olika sammanhang finns i följande avsnitt:

* [Distribution av värden i en mapp](../get-started/work-with-folders.md##distribution-values-folder)
* [Distribution av värden i en fråga](../query/build-query.md#distribution-values-query)