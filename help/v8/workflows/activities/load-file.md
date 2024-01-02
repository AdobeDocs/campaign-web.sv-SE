---
audience: end-user
title: Använda arbetsflödesaktiviteten Läs in fil
description: Lär dig hur du använder arbetsflödesaktiviteten Läs in fil
badge: label="Begränsad tillgänglighet"
source-git-commit: 6068e3695ebed22a94a75b9aded59d1e5fb6b47a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 1%

---

# Ladda fil {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Läs in filaktivitet"
>abstract="The **Läs in fil** aktiviteten är en **Datahantering** aktivitet. Använd den här aktiviteten när du vill arbeta med profiler som lagras i en extern fil."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Exempelfil"
>abstract="Exempelfil"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Filens namn"
>abstract="Filens namn"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Måldatabas"
>abstract="Måldatabas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Avvisa hantering för Läs in filaktivitet"
>abstract="Avvisa hantering för Läs in filaktivitet"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Avvisa utgående övergång för hantering"
>abstract="Avvisa utgående övergång för hantering"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Avvisa utgående övergång för hantering av avslag"
>abstract="Avvisa utgående övergång för hantering av avslag"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formatering för aktiviteten Läs in fil"
>abstract="Formatering för aktiviteten Läs in fil"


The **Läs in fil** aktiviteten är en **Datahantering** aktivitet. Använd den här aktiviteten när du vill arbeta med profiler som lagras i en extern fil. Profiler läggs inte till i databasen, men alla fält i indatafilen är tillgängliga för [personalisering](../../personalization/gs-personalization.md)eller för att uppdatera profiler.


>[!NOTE]
>Filformat som stöds är: text (TXT) och kommaavgränsade värden (CSV).


Den här aktiviteten kan användas med en [Avstämning](reconciliation.md) aktivitet för att länka oidentifierade data till befintliga resurser. Till exempel **Läs in fil** kan placeras före en **Avstämning** om du importerar data som inte är standard till databasen.


## Konfigurera aktiviteten Läs in fil {#load-configuration}

Följ de här stegen för att konfigurera **Läs in fil** aktivitet:


1. Dra och släpp en **Läs in fil** i arbetsflödet. Klicka på **Välj från fil** -knappen.
1. Markera den lokala fil som ska användas. Formatet måste justeras mot [exempelfil](../../audience/file-audience.md#sample-file).
1. Förhandsgranska och kontrollera hur data mappas i skärmens centrala del.
1. Justera kolumninställningarna och formatera data från de tillgängliga alternativen.
1. Klicka **Bekräfta** när inställningarna är korrekta.

## Exempel{#load-example}

Ett exempel på hur en extern fil läses in är tillgängligt med **Avstämning** aktivitet i [det här avsnittet](reconciliation.md#example).