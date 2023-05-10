---
audience: end-user
title: Importera mottagare från en fil
description: Lär dig hur du importerar mottagare från en extern fil
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Importera mottagare från en fil {#audience-from-file}

Du kan lägga till eller uppdatera kontakter från leveransgränssnittet genom att överföra en textfil (TXT) eller en kommaseparerad värdefil (CSV). De läggs sedan till i databasen.

>[!NOTE]
>
>Du kan också skapa ett importarbetsflöde för att lägga till eller uppdatera flera profiler.


Så här lägger du till profiler från en lokal fil direkt från gränssnittet:

1. I fönstret för leveransskapande klickar du på **Välj målgrupp** och väljer **Välj från fil** alternativ.
1. Välj den lokala fil som ska överföras.
1. Definiera kolumninställningarna och formatera data. Du kan hoppa över en kolumn med **Ignorera kolumn** växla.
1. Förhandsgranska hur data mappas i skärmens centrala del.
1. Klicka **Bekräfta** när inställningarna är korrekta.

När du skapar och anpassar meddelandeinnehållet kan du välja fält från indatafilen i personaliseringsredigeraren.

## Exempelfil {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Exempelfil"
>abstract="Filformat som stöds: txt, csv. Använd den första raden som kolumnrubrik."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
