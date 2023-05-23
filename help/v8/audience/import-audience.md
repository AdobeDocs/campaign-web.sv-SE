---
audience: end-user
title: Målmottagare från en fil
description: Lär dig hur du använder mottagare från en extern fil för att skapa e-postmålgrupper
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# Målmottagare från en fil {#audience-from-file}

Du kan överföra kontakter från en extern fil. Den här funktionen är bara tillgänglig för e-postleveranser.Format som stöds är: textfil (TXT) eller en kommaavgränsad värdefil (CSV). De läggs sedan till i databasen.

>[!NOTE]
>
>Du kan skapa ett importarbetsflöde för att lägga till eller uppdatera flera profiler.  Läs mer


Följ de här stegen för att ange profiler från en lokal fil direkt från gränssnittet:

1. I fönstret för att skapa e-postleverans klickar du på **Välj målgrupp** och väljer **Välj från fil** alternativ.

   ![](assets/select-from-file.png)

1. Välj den lokala fil som ska överföras.
1. Förhandsgranska hur data mappas i skärmens centrala del.
1. Välj den kolumn som innehåller e-postadressen i dialogrutan **Adressfält** nedrullningsbar meny.
1. Justera kolumninställningarna och formatera data från de tillgängliga alternativen.
1. Klicka **Bekräfta** när inställningarna är korrekta.

När du skapar och anpassar meddelandeinnehållet kan du välja fält från indatafilen i personaliseringsredigeraren.

![](assets/select-external-perso.png)

## Exempelfil {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Exempelfil"
>abstract="Filformat som stöds: txt, csv. Använd den första raden som kolumnrubrik."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
