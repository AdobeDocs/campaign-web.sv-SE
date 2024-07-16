---
audience: end-user
title: Använd arbetsflödesaktiviteten för avstämning
description: Lär dig hur du använder arbetsflödesaktiviteten för avstämning
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 935fba929c26d6d7b3057ee7c24148215a04e45e
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 10%

---

# Avstämning {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Avstämningsaktivitet"
>abstract="Aktiviteten **Avstämning** är en **målaktivitet** som gör att du kan definiera länken mellan data i Adobe Campaign-databasen och data i en arbetstabell. Aktiviteten **Avstämning** kan till exempel placeras efter en **Läs in fil** -aktivitet för att importera icke-standarddata till databasen. I det här fallet kan du med aktiviteten **Avstämning** definiera länken mellan data i Adobe Campaign-databasen och data i den externa tabellen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Avstämningsmarkeringsfält"
>abstract="Avstämningsmarkeringsfält"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Avstämning skapa villkor"
>abstract="Avstämning skapa villkor"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Avstämning genererar komplementtal"
>abstract="Avstämning genererar komplementtal"

Aktiviteten **Avstämning** är en **målaktivitet** som gör att du kan definiera länken mellan data i Adobe Campaign-databasen och data i en arbetstabell, till exempel data som lästs in från en extern fil.

Aktiviteten **Avstämning** kan till exempel placeras efter en **Läs in fil** -aktivitet för att importera icke-standarddata till databasen. I det här fallet kan du med aktiviteten **Avstämning** definiera länken mellan data i Adobe Campaign-databasen och data i arbetstabellen.

## Bästa praxis {#reconciliation-best-practices}

Med aktiviteten **Enrichment** kan du definiera ytterligare data som ska bearbetas i arbetsflödet (du kan använda en **Enrichment**-aktivitet för att kombinera data från flera uppsättningar eller för att skapa länkar till en tillfällig resurs), men med aktiviteten **Avstämning** kan du länka oidentifierade data till befintliga resurser.

>[!NOTE]
>Avstämningsåtgärden innebär att data för de länkade dimensionerna redan finns i databasen.  Om du till exempel importerar en inköpsfil som visar vilken produkt som köptes vid en viss tidpunkt, av en viss klient och så vidare, så måste produkten och klienten redan finnas i databasen.

## Konfigurera avstämningsaktiviteten {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Måldimension"
>abstract="Välj den nya måldimensionen. Med en dimension kan du definiera målpopulationen: mottagare, appprenumeranter, operatorer, prenumeranter osv. Som standard är den aktuella måldimensionen markerad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Avstämningsregler"
>abstract="Välj avstämningsregler som ska användas för dedupliceringen. Om du vill använda attribut markerar du alternativet **Enkla attribut** och väljer käll- och målfälten. Om du vill skapa ett eget avstämningsvillkor med frågemodelleraren väljer du alternativet **Avancerade avstämningsvillkor** ."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Arbeta med frågemodelleraren"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Välj måldimension"
>abstract="Välj måldimension för inkommande data som ska förenas med."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html#targeting-dimensions" text="Måldimensioner"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Behåll ej avstämda data"
>abstract="Som standard behålls ej avstämda data i den utgående övergången och är tillgängliga i arbetstabellen för framtida bruk. Om du vill ta bort ej avstämda data inaktiverar du alternativet **Behåll ej avstämda data**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Avstämningsattribut"
>abstract="Markera attributet som ska användas för att avstämma data och klicka på Bekräfta."

Så här konfigurerar du aktiviteten **Avstämning**:

1. Lägg till en **avstämningsaktivitet** i ditt arbetsflöde. Denna aktivitet bör läggas till efter en övergång som innehåller en befolkning vars målgruppsdimension inte kommer direkt från Adobe Campaign.

1. Välj den nya måldimensionen. Med en dimension kan du definiera målpopulationen: mottagare, appprenumeranter, operatorer, prenumeranter osv. [Läs mer om måldimensioner](../../audience/about-recipients.md#targeting-dimensions).

1. Välj de fält som ska användas för avstämningen. Du kan använda ett eller flera avstämningskriterier.

   1. Om du vill använda attribut för att stämma av data markerar du alternativet **Enkla attribut**. I fältet **Source** visas de fält som är tillgängliga i indataövergången och som ska avstämas. Fältet **Mål** motsvarar fälten i den valda måldimensionen. Data avstäms när källan och målet är lika. Markera till exempel fälten **E-post** för att ta bort dubbletter av profiler baserat på deras e-postadress.

      Om du vill lägga till ytterligare avstämningsvillkor klickar du på knappen **Lägg till regel** . Om flera kopplingsvillkor anges måste ALLA verifieras så att data kan länkas ihop.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. Om du vill använda andra attribut för att stämma av data väljer du alternativet **Avancerade avstämningsvillkor** . Du kan sedan skapa ett eget avstämningsvillkor med frågemodelleraren. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md).

1. Du kan filtrera data för avstämning med knappen **Skapa filter** . Detta gör att du kan skapa ett anpassat villkor med hjälp av frågemodelleraren. [Lär dig arbeta med frågemodelleraren](../../query/query-modeler-overview.md)

Som standard lagras ej avstämda data i den utgående övergången och är tillgängliga i arbetsboken för framtida bruk. Om du vill ta bort ej avstämda data inaktiverar du alternativet **Behåll ej avstämda data**.

## Exempel {#reconciliation-example}

I följande exempel visas ett arbetsflöde som skapar en publik med profiler direkt från en importerad fil som innehåller nya klienter.  Den består av följande verksamheter:

Arbetsflödet är då utformat så här:

![](../assets/workflow-reconciliation-sample-1.0.png)


Den har följande aktiviteter:

* En [Läs in fil](load-file.md)-aktivitet överför en fil som innehåller profildata som har extraherats från ett externt verktyg.

  Exempel:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* En **avstämningsaktivitet** som identifierar inkommande data som profiler, genom att använda fälten **email** och **Date of born** som avstämningsvillkor.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* En [Spara målgruppsaktivitet](save-audience.md) om du vill skapa en ny målgrupp baserat på dessa uppdateringar. Du kan också ersätta aktiviteten **Spara målgrupp** med en **End**-aktivitet om ingen specifik målgrupp behöver skapas eller uppdateras. Mottagarprofiler uppdateras i alla fall när du kör arbetsflödet.


## Kompatibilitet {#reconciliation-compat}

Aktiviteten **Avstämning** finns inte i klientkonsolen. Alla **berikande** aktiviteter som skapas i klientkonsolen med avstämningsalternativen aktiverade visas som **avstämningsaktiviteter** i webbgränssnittet för Campaign.
