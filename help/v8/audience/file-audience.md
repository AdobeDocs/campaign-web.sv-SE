---
audience: end-user
title: Läsa in en e-postmålgrupp från en fil
description: Lär dig hur du läser in profiler från en extern fil för att skapa e-postmålgrupper
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: b166d06215e06d6426ab9ce9a757fcc041810df9
workflow-type: tm+mt
source-wordcount: '640'
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
>abstract="Kontrollera kolumnformatet i den externa filen."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formateringsparametrar"
>abstract="Ange hur den externa filen ska formateras för att säkerställa att data importeras på rätt sätt."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Förhandsgranska filen"
>abstract="Kontrollera förhandsgranskningen av kolumnerna i den externa filen. Den här skärmen visar endast upp till 30 poster."

Med Adobe Campaign webbanvändargränssnitt kan du rikta profiler som lagras i en extern fil. När profilerna har lästs in är alla fält från indatafilen tillgängliga för användning för att anpassa leveransen [Lär dig anpassa ditt innehåll](../personalization/personalize.md).

Profiler från indatafilen läggs inte till i databasen. De har lästs in och är endast tillgängliga för den här specifika fristående e-postleveransen.

>[!NOTE]
>
>Den här sidan beskriver hur du läser in externa profiler från en fil när du skapar en fristående e-postleverans. Information om hur du läser in data från en fil i ett arbetsflödes sammanhang finns i [den här sidan](../workflows/activities/load-file.md).

## Måste läsas {#must-read}

* Den här funktionen är tillgänglig för **e-postleveranser** endast.
* Filformat som stöds är: text (TXT) och kommaavgränsade värden (CSV).
* Du kan inte använda [kontrollgrupper](control-group.md) när målpopulationen läses in från en extern fil.

## Markera och konfigurera indatafilen {#upload}

Följ de här stegen om du vill skapa målprofiler från en fil i dina e-postmeddelanden:

1. Öppna en befintlig e-postleverans, eller [skapa en ny e-postleverans](../email/create-email.md).
1. I **Målgrupp** klickar du på **Välj målgrupp** knapp och sedan välja **Välj från fil**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. Välj den lokala fil som ska läsas in. Filformatet måste justeras mot [exempelfil](#sample-file).
1. Förhandsgranska och kontrollera hur data mappas i skärmens centrala del.

   ![](assets/select-from-file-map.png)

1. Ange den kolumn som innehåller e-postadressen från **Adressfält** listruta. Du kan också markera blockeringslista-kolumnen om du har sådan information i indatafilen.
1. Justera kolumninställningarna och formatera data från de tillgängliga alternativen.
1. Klicka **Bekräfta** när inställningarna är korrekta.

När du skapar meddelandeinnehållet kan du lägga till personalisering genom att använda fält från indatafilen. [Lär dig anpassa innehåll](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## Exempelfil {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Läsa in en målgrupp från en fil"
>abstract="Filformat som stöds är TXT och CSV. Använd den första raden som kolumnrubrik. Justera filformatet med exempelfilen som finns på länken nedan."

När du läser in en extern fil till målprofiler i leveranserna, kontrollerar du att indatafilen matchar rekommendationerna nedan:

* Format som stöds är TXT och CSV.
* Den första raden i filen är kolumnrubriken.
* Justera filformatet med exempelfilen nedan:

  ```javascript
  {
  lastname,firstname,city,birthdate,email,denylist
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
  }
  ```

## Förhandsgranska och testa din e-post {#test}

Med Campaign Web kan ni förhandsgranska och skicka korrektur när ni använder en målgrupp som överförts från en fil. Följ dessa steg för att göra detta:

1. Klicka på **[!UICONTROL Simulate content button]** på skärmen där du redigerar leveransinnehåll och klickar på **[!UICONTROL Add test profile(s)]** -knappen.

1. Profilerna som finns i den överförda filen visas. Markera den eller de profiler som du vill använda för att förhandsgranska innehållet och klicka på **[!UICONTROL Select]**.

1. En förhandsgranskning av leveransinnehållet visas i den högra rutan på skärmen. Personaliserade element ersätts med data från den profil som valts i den vänstra rutan. [Läs mer om förhandsgranskning av leveransinnehåll](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. Om du vill skicka korrektur klickar du på **[!UICONTROL Send proof]** -knappen.

1. Klicka på **[!UICONTROL Upload proof profiles]** och markera den TXT- eller CSV-fil som innehåller korrekturmottagarna.

   >[!CAUTION]
   >
   >Se till att filformatet matchar det som används för att överföra målgruppen. Alla formatfel visar en varning.

1. När korrekturprofilerna har lagts till och du är redo att skicka korrekturet klickar du på **[!UICONTROL Send proof]** och bekräfta sändningen.

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. Du kan övervaka sändningen av korrekturet med **[!UICONTROL View proofs]** när som helst. [Läs mer om korrekturövervakning](../preview-test/test-deliveries.md#access-test-deliveries)
