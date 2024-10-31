---
audience: end-user
title: Använd aktiviteten Läs in filarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten Läs in fil
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: ac22df907233000bada45ac2c382f1a247f7d21a
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 2%

---

# Ladda fil {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Läs in filaktivitet"
>abstract="Aktiviteten **Läs in fil** är en **datahanteringsaktivitet**. Använd den här aktiviteten om du vill arbeta med data som lagras i en extern fil. Profiler och data läggs inte till i databasen, men alla fält i indatafilen kan anpassas, eller för att uppdatera profiler eller någon annan tabell. "

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Avvisa utgående hanteringsövergång"
>abstract="Avvisa utgående hanteringsövergång"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Avvisa utgående hanteringsövergång för avslag"
>abstract="Avvisa utgående hanteringsövergång för avslag"


Aktiviteten **Läs in fil** är en **datahanteringsaktivitet**. Använd den här aktiviteten om du vill arbeta med profiler och data som lagras i en extern fil. Profiler och data läggs inte till i databasen, men alla fält i indatafilen är tillgängliga för [anpassning](../../personalization/gs-personalization.md), för att uppdatera profiler eller någon annan tabell.

>[!NOTE]
>Filformat som stöds är: text (TXT) och kommaavgränsade värden (CSV). Du kan läsa in filer med en maximal storlek på 50 MB.

Den här aktiviteten kan användas med en [avstämningsaktivitet](reconciliation.md) för att länka oidentifierade data till befintliga resurser. Aktiviteten **Läs in fil** kan till exempel placeras före en **avstämningsaktivitet** om du importerar data som inte är standard till databasen.

## Konfigurera aktiviteten Läs in fil {#load-configuration}

Aktivitetskonfigurationen för **Läs in fil** omfattar två steg. Först måste du definiera den förväntade filstrukturen genom att överföra en exempelfil.  När du är klar kan du ange ursprunget för filen vars data ska importeras. Följ stegen nedan för att konfigurera aktiviteten.

![](../assets/workflow-load-file.png)

### Konfigurera exempelfilen {#sample}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Exempelfil"
>abstract="Välj den förväntade filstrukturen genom att ladda upp en exempelfil."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formatering för inläsning av filaktivitet"
>abstract="Ange i avsnittet **Formatering** hur filen ska formateras för att säkerställa att data importeras korrekt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Värdeommappning för aktiviteten Läs in fil"
>abstract="Använd det här alternativet om du vill mappa specifika värden från de inlästa filerna med nya värden. Om kolumnen till exempel innehåller värdena &quot;Sant&quot;/&quot;Falskt&quot; kan du lägga till en mappning som automatiskt ersätter dessa värden med tecknen &quot;0&quot;/&quot;1&quot;."

Följ de här stegen för att konfigurera exempelfilen som används för att definiera den förväntade filstrukturen:

1. Lägg till en **Läs in fil**-aktivitet i ditt arbetsflöde.

1. Markera exempelfilen som ska användas för att definiera den förväntade filstrukturen. Om du vill göra det klickar du på knappen **Välj fil** i avsnittet **[!UICONTROL Sample file]** och väljer den lokala fil som ska användas.

   >[!NOTE]
   >
   >Data i exempelfilen används för att konfigurera aktiviteten men importeras inte.  Vi rekommenderar att du använder en exempelfil som innehåller lite data. Filformatet måste justeras mot denna [exempelfil](../../audience/file-audience.md#sample-file).

1. En förhandsvisning av exempelfilen visas med högst 30 rader.

1. Ange om filen använder avgränsade kolumner eller kolumner med fast bredd i listrutan **[!UICONTROL File type]**.

   ![](../assets/workflow-load-file-sample.png)

1. För filtyper med avgränsade kolumner använder du avsnittet **Kolumner** för att konfigurera egenskaperna för varje kolumn.

   +++Tillgängliga alternativ för filkolumner

   * **[!UICONTROL Label]**: Etikett som ska visas för kolumnen.
   * **[!UICONTROL Data type]**: Typ av data i kolumnen.
   * **[!UICONTROL Width]** (strängdatatyp): Maximalt antal tecken som ska visas i kolumnen.
   * **[!UICONTROL Data Transformation]** (strängdatatyp): Använd omformning på värdena i kolumnen.
   * **[!UICONTROL White space management]** (strängdatatyp): Ange hur blanksteg i kolumnen ska hanteras.
   * **[!UICONTROL Separators]** (datatyperna date, time, integer och number)*: Ange vilka tecken som ska användas som avgränsare.
   * **[!UICONTROL Allow NULLs]**: Ange hur tomma värden i kolumnen ska hanteras. Alternativet &quot;Adobe Campaign-standard&quot; ger ett felmeddelande om det finns något tomt värde.
   * **[!UICONTROL Error processing]** (strängdatatyp): Ange beteendet om fel uppstår på någon av raderna.
   * **[!UICONTROL Value remapping]**: Med det här alternativet kan du mappa specifika värden med nya. Om kolumnen till exempel innehåller värdena &quot;Sant&quot;/&quot;Falskt&quot; kan du lägga till en mappning som automatiskt ersätter dessa värden med tecknen &quot;0&quot;/&quot;1&quot;.

+++

1. I avsnittet **Formatering** anger du hur filen ska formateras för att säkerställa att data importeras på rätt sätt.

### Definiera målfilen som ska överföras {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Målfil för aktiviteten Läs in fil"
>abstract="Ange hur filen ska hämtas till servern i avsnittet **[!UICONTROL Target file]**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Filens namn"
>abstract="Ange namnet på fältet som ska överföras till servern. Klicka på ikonen **[!UICONTROL Open personalization dialog]** för att använda uttrycksredigeraren, inklusive händelsevariabler, för att beräkna filnamnet."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Måldatabas"
>abstract="Om du använder en **[!UICONTROL Load file]**-aktivitet som redan har konfigurerats i klientkonsolen, finns ytterligare ett **[!UICONTROL Target database]**-avsnitt tillgängligt om du har konfigurerat aktiviteten att överföra filen till en extern databas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Kommandot Läs in fil"
>abstract="Att tillåta godtyckligt kommando för förbehandling är ett säkerhetsproblem, inaktivera säkerhetsalternativet XtkSecurity_Disable_Preproc för att tvinga fram användning av en fördefinierad lista med kommandon."

>[!CAUTION]
>
>Innan du läser in målfilen bör du kontrollera att den följer exempelfilformatet. Eventuella skillnader i filformat, kolumnstruktur eller antal kolumner kan leda till fel under arbetsflödeskörningen.

Gör så här för att definiera vilken målfil som ska överföras:

1. Ange i avsnittet **[!UICONTROL Target file]** vilken åtgärd som ska utföras när filen hämtas och laddas upp till servern.

   * **[!UICONTROL Upload file from local machine]**: Välj filen som du vill överföra från datorn.

   * **[!UICONTROL Specified in the transition]**: Överför den angivna filen i den inkommande övergången som kommer från en tidigare aktivitet som **[!UICONTROL Transfer file]**.

   * **[!UICONTROL Pre-process the file]**: Överför filen som angavs i föregående övergång och använd ett förbehandlingskommando på den, till exempel **[!UICONTROL Decompression]** eller **[!UICONTROL Decrypt]**.

   * **[!UICONTROL Calculated]**: Överför filen vars namn anges i fältet **[!UICONTROL File name]**. Klicka på ikonen **[!UICONTROL Open personalization dialog]** om du vill använda uttrycksredigeraren, inklusive händelsevariabler, för att beräkna filnamnet.

   ![](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >Om du använder en **[!UICONTROL Load file]**-aktivitet som redan har konfigurerats i klientkonsolen visas ytterligare ett **[!UICONTROL Target database]**-avsnitt om du har konfigurerat aktiviteten att överföra filen till en extern databas. Du kan ange om du vill överföra filen på Campaign-servern eller i den externa databasen.

### Ytterligare alternativ {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Avvisa hantering för inläsning av filaktivitet"
>abstract="Ange hur aktiviteten ska fungera vid fel i avsnittet **Avvisa hantering**. Du kan definiera det maximala antalet fel som tillåts och växla alternativet **[!UICONTROL Keep rejects in a file]** för att hämta en fil som innehåller de fel som inträffade under importen till servern."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Ta bort fil efter import"
>abstract="Växla **Ta bort fil efter import** om du vill ta bort originalfilen från servern när filen har importerats."


1. Ange hur aktiviteten ska fungera vid fel i avsnittet **Avvisa hantering**:

   * I fältet **[!UICONTROL Number of errors allowed]** anger du det maximala antalet fel som tillåts när filen ska läsas in. Om värdet till exempel är 20 misslyckas arbetsflödeskörningen om det finns mer än 20 fel när filen läses in.

   * Om du vill behålla felen som uppstod när filen lästes in aktiverar du alternativet **[!UICONTROL Keep rejects in a file]** och anger önskat namn för filen i fältet **[!UICONTROL Rejection File]**.

     När du har aktiverat det här alternativet läggs ytterligare en utdataövergång till som heter &quot;Komplettera&quot; efter aktiviteten. Alla fel som inträffar under importen lagras i den angivna filen på servern.

1. Om du vill ta bort den överförda filen från servern när arbetsflödet har körts växlar du till alternativet **[!UICONTROL Delete file after import]**.

   ![](../assets/workflow-load-file-options.png)

1. Klicka på **Bekräfta** när inställningarna är korrekta.

## Exempel {#load-example}

Ett exempel på en extern fil som läses in och som används med aktiviteten **Avstämning** finns i [det här avsnittet](reconciliation.md#reconciliation-example).
