---
audience: end-user
title: Målmottagare från en fil
description: Lär dig hur du använder mottagare från en extern fil för att skapa e-postmålgrupper
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ed9d67c5d84826035785e9543f4ed7655aa094f1
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# Läsa in en e-postmålgrupp från en fil {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Välj fil"
>abstract="Välj den lokala fil som ska överföras. Format som stöds är TXT och CSV. Justera filformatet med exempelfilen som är länkad nedan."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Kolumndefinition"
>abstract="Kontrollera formatet för de kolumner som ska infogas från den lokala filen."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formateringsparametrar"
>abstract="Kontrollera formateringsparametrarna för filen."

Du kan överföra kontakter från en extern fil. Profiler läggs inte till i databasen, men alla fält i indatafilen är tillgängliga för [personalisering](../personalization/gs-personalization.md). Filformat som stöds är: text (TXT) och kommaavgränsade värden (CSV).

>[!CAUTION]
>
>* Den här funktionen är bara tillgänglig för **fristående e-postleveranser**. Det kan inte användas i arbetsflöden, eller med SMS- eller push-leveranser.
>
>* Du kan inte använda [kontrollgrupper](control-group.md) när målpopulationen läses in från en extern fil.

## Ladda upp filen {#upload}

Följ de här stegen för att ange profiler från en lokal fil direkt från e-postgränssnittet:

1. Öppna en befintlig e-postleverans, eller [skapa en ny e-postleverans](../email/create-email.md).
1. Fönstret för att skapa e-postleverans visas på **Målgrupp** klickar du på **Välj målgrupp** och väljer **Välj från fil** alternativ.

   ![](assets/select-from-file.png)

1. Välj den lokala fil som ska överföras. Formatet måste justeras mot [exempelfil](#sample-file).
1. Förhandsgranska och kontrollera hur data mappas i skärmens centrala del.
1. Välj den kolumn som innehåller e-postadressen i dialogrutan **Adressfält** nedrullningsbar meny. Du kan också markera blockeringslista-kolumnen om du har sådan information i indatafilen.
1. Justera kolumninställningarna och formatera data från de tillgängliga alternativen.
1. Klicka **Bekräfta** när inställningarna är korrekta.

När du skapar och anpassar meddelandeinnehållet kan du välja fält från indatafilen i [Personaliseringsredigerare](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## Förhandsgranska och testa e-postmeddelandet {#test}

Med Campaign Web kan ni förhandsgranska och skicka testmeddelanden när ni använder en målgrupp som överförts från en fil. Följ dessa steg för att göra detta:

1. Simulera innehåll
1. Öppnar förhandsvisning. Klicka på välj profil(er): välj profiler från filen som ska användas
1. om du vill skicka testmeddelande klickar du på test
1. testläge: Definiera provtryckets mål
1. Överför målet för testmeddelandet från en andra fil (eller använd samma). filformateringen följer samma som den överförda filen
1. Kontroller som utförs i filformat
1. klicka på skicka

+ länk till avsnittet för förhandsgranskning och test

**frågor:**
* ingen ersättning från fil tillgänglig?

## Exempelfil {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Läsa in en målgrupp från en fil"
>abstract="Filformat som stöds är TXT och CSV. Använd den första raden som kolumnrubrik. Justera filformatet med exempelfilen som finns på länken nedan."

Format som stöds är TXT och CSV. Den första raden är kolumnrubriken.

Justera filformatet med exempelfilen nedan:

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
