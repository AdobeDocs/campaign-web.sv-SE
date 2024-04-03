---
audience: end-user
title: Använda arbetsflödesaktiviteten Läs in fil
description: Lär dig hur du använder arbetsflödesaktiviteten Läs in fil
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 1eaa2710e682e9038befc5d0752c064e2bb48521
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Ladda fil {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Läs in filaktivitet"
>abstract="The **Läs in fil** aktiviteten är en **Datahantering** aktivitet. Använd den här aktiviteten när du vill arbeta med data som lagras i en extern fil."

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

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Målfil för aktiviteten Läs in fil"
>abstract="Målfil för aktiviteten Läs in fil"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Värdeommappning för aktiviteten Läs in fil"
>abstract="Värdeommappning för aktiviteten Läs in fil"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Kommandot Läs in fil"
>abstract="Att tillåta godtyckligt kommando för förbehandling är ett säkerhetsproblem, inaktivera säkerhetsalternativet XtkSecurity_Disable_Preproc för att tvinga fram användning av en fördefinierad lista med kommandon."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Ta bort fil efter import"
>abstract="Växla **Ta bort fil efter import** om du vill ta bort originalfilen från servern när filen har importerats."

The **Läs in fil** aktiviteten är en **Datahantering** aktivitet. Använd den här aktiviteten när du vill arbeta med profiler och data som lagras i en extern fil. Profiler och data läggs inte till i databasen, men alla fält i indatafilen är tillgängliga för [personalisering](../../personalization/gs-personalization.md)eller för att uppdatera profiler eller andra tabeller.

>[!NOTE]
>Filformat som stöds är: text (TXT) och kommaavgränsade värden (CSV).

Den här aktiviteten kan användas med en [Avstämning](reconciliation.md) aktivitet för att länka oidentifierade data till befintliga resurser. Till exempel **Läs in fil** kan placeras före en **Avstämning** om du importerar data som inte är standard till databasen.

## Konfigurera aktiviteten Läs in fil {#load-configuration}

Följ de här stegen för att konfigurera **Läs in fil** aktivitet:

1. Dra och släpp en **Läs in fil** i arbetsflödet. Klicka på **Välj från fil** -knappen.

1. Markera den lokala fil som ska användas. Formatet måste vara justerat mot detta [exempelfil](../../audience/file-audience.md#sample-file).

1. Förhandsgranska och kontrollera hur data mappas i skärmens centrala del.

   ![](../assets/load-file.png)

1. Använd **Kolumner** i den vänstra rutan för att justera datatypen och bredden för varje kolumn.

1. I **Formatering** anger du hur den externa filen ska formateras för att säkerställa att data importeras på rätt sätt.

1. Klicka **Bekräfta** när inställningarna är korrekta.

## Exempel{#load-example}

Ett exempel på en extern inläsning av filer som används med **Avstämning** aktivitet är tillgänglig i [det här avsnittet](reconciliation.md#reconciliation-example).
