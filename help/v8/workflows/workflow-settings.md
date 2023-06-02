---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 1a608d2042ae257d89acbd67d99a0ce05d89f382
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 3%

---

# Konfigurera inställningar för arbetsflöde {#workflow-settings}

När du organiserar arbetsflödesaktiviteter på arbetsytan kan du komma åt avancerade inställningar som är relaterade till arbetsflödet. Du kan till exempel ange en specifik tidszon för arbetsflödet, hantera arbetsflödets beteende om fel uppstår eller hantera den fördröjning efter vilken arbetsflödeshistoriken ska rensas.

De här inställningarna är förkonfigurerade i mallen som valdes när arbetsflödet skapades, men kan redigeras efter behov för det aktuella arbetsflödet.

Om du vill göra det klickar du på **[!UICONTROL Workflow settings]** -ikonen i det övre vänstra hörnet av arbetsytan, bredvid arbetsflödesetiketten.

![](assets/workflow-settings.png)

## Egenskaper för arbetsflöde {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Egenskaper för arbetsflöde"
>abstract="TBD"

The **[!UICONTROL Properties]** -avsnittet innehåller allmänna inställningar som också är tillgängliga när du skapar arbetsflödet.

* **[!UICONTROL Label]**: Etiketten för arbetsflödet som visas i listan.
* **[!UICONTROL Name]**: Arbetsflödets interna namn.
* **[!UICONTROL Folder]**: Mappen där arbetsflödet ska sparas.
* **[!UICONTROL Linked campaign]**: Det här fältet visas om arbetsflödet har skapats i en kampanj. Du kan öppna den associerade kampanjen.
* **[!UICONTROL Timezone]**: Definiera en specifik tidszon som ska användas som standard i alla arbetsflödets aktiviteter. Som standard är arbetsflödets tidszon den som definieras för den aktuella Campaign-operatorn.
* **[!UICONTROL Supervisor(s)]**: När ett arbetsflöde är felaktigt meddelas de operatorer som tillhör arbetsflödesövervakningsgruppen via e-post, förutsatt att deras e-postadress anges i deras profil.
* **[!UICONTROL Description]**: Använd det här fältet om du vill ange en beskrivning av arbetsflödet.

## Segmenteringsinställningar

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinställningar"
>abstract="TBD"

* **[!UICONTROL Targeting dimension]**: Välj måldimensionen som ska användas för målprofiler: mottagare, mottagare, mottagare, operatör, abonnenter osv.
* **[!UICONTROL Keep the result of interim populations between two executions]**: Som standard behålls endast arbetsregister för den senaste körningen av arbetsflödet. Arbetstabeller från tidigare körningar rensas av ett tekniskt arbetsflöde, som körs dagligen.

   Om det här alternativet är aktiverat behålls arbetsregister även efter att arbetsflödet har körts. Du kan använda den i testsyfte och måste därför bara användas i utvecklings- eller staging-miljöer. Den får aldrig checkas in i ett produktionsarbetsflöde.

## Körningsinställningar

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Körningsinställningar"
>abstract="TBD"

* **[!UICONTROL History in days]**: Anger efter hur många dagar som historiken måste rensas. Historiken innehåller element som är relaterade till arbetsflödet: loggar, uppgifter, händelser (tekniska objekt som är länkade till arbetsflödesåtgärden). Standardvärdet är 30 dagar för färdiga arbetsflödesmallar. Historiken rensas av det tekniska arbetsflödet för databasrensning som utförs som standard varje dag

   >[!IMPORTANT]
   >
   >Om **[!UICONTROL History in days]** fältet lämnas tomt, dess värde betraktas som&quot;1&quot;, vilket innebär att historiken rensas efter 1 dag.

* **[!UICONTROL Default affinity]**: Om installationen innehåller flera arbetsflödesservrar använder du det här fältet för att välja vilken dator arbetsflödet ska köras på. Om värdet som definieras i det här fältet inte finns på någon server, kommer arbetsflödet att förbli väntande.

* **[!UICONTROL Save SQL queries in log]**: Med kan du spara SQL-frågor från arbetsflödet i loggarna. Den här funktionen är reserverad för avancerade användare. Det gäller arbetsflöden som innehåller riktade aktiviteter som **[!UICONTROL Build audience]**. När det här alternativet är aktiverat visas de SQL-frågor som skickas till databasen under arbetsflödeskörningen i Adobe Campaign, så att du kan analysera dem för att optimera frågor eller diagnostisera problem.

   Frågor visas i en **[!UICONTROL SQL logs]** som läggs till i arbetsflödet (utom kampanjarbetsflöden) och i **[!UICONTROL Properties]** när alternativet är aktiverat. <!-- where?-->

## Inställningar för felhantering

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Inställningar för felhantering"
>abstract="TBD"

* **[!UICONTROL Error management]**: I det här fältet kan du definiera de åtgärder som ska vidtas om en arbetsflödesuppgift innehåller fel. Det finns två möjliga alternativ:

   * **[!UICONTROL Suspend the process]**: Arbetsflödet pausas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst kan du återuppta arbetsflödet med **[!UICONTROL Resume]** knappar.
   * **[!UICONTROL Ignore]**: Statusen för aktiviteten som utlöste felet ändras till **[!UICONTROL Failed]** men arbetsflödet behåller **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abord the process]**: Arbetsflödet stoppas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst startar du om arbetsflödet med **[!UICONTROL Start]** knappar.

* **[!UICONTROL Consecutive errors]**: Det här fältet blir tillgängligt när **[!UICONTROL Ignore]** värdet är markerat i **[!UICONTROL In case of errors]** fält. Du kan ange antalet fel som kan ignoreras innan processen stoppas. När det här numret har nåtts ändras arbetsflödets status till **[!UICONTROL Failed]**. Om värdet för det här fältet är 0 stoppas aldrig arbetsflödet oavsett antalet fel.
