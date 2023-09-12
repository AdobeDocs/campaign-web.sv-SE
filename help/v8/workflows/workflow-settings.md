---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Beta"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 3e4cdd2ece8fc000bc71b366549fd63f18201ff7
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Konfigurera inställningar för arbetsflöde {#workflow-settings}

När du organiserar arbetsflödesaktiviteter på arbetsytan kan du komma åt avancerade inställningar som är relaterade till arbetsflödet. Du kan till exempel ange en specifik tidszon för arbetsflödet, hantera arbetsflödets beteende om fel uppstår eller hantera den fördröjning efter vilken arbetsflödeshistoriken ska rensas.

De här inställningarna är förkonfigurerade i mallen som valdes när arbetsflödet skapades, men kan redigeras efter behov för det aktuella arbetsflödet.

Klicka på **[!UICONTROL Workflow settings]** -ikonen i det övre vänstra hörnet av arbetsytan, bredvid arbetsflödesetiketten.

![](assets/workflow-settings.png)

## Egenskaper för arbetsflöde {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Egenskaper för arbetsflöde"
>abstract="I det här avsnittet finns allmänna arbetsflödesegenskaper som också är tillgängliga när du skapar arbetsflödet. Du kan välja vilken mall som ska användas för att skapa arbetsflödet och ange en etikett. Expandera avsnittet Ytterligare alternativ om du vill konfigurera särskilda inställningar, t.ex. mappen för arbetsflödeslagring eller tidszonen."

The **[!UICONTROL Properties]** -avsnittet innehåller allmänna inställningar som också är tillgängliga när du skapar arbetsflödet.

* **[!UICONTROL Label]**: Etiketten för arbetsflödet som visas i listan.
* **[!UICONTROL Name]**: Arbetsflödets interna namn.
* **[!UICONTROL Folder]**: Mappen där arbetsflödet ska sparas.
* **[!UICONTROL Linked campaign]**: Det här fältet visas om arbetsflödet har skapats i en kampanj. Du kan öppna den associerade kampanjen.
* **[!UICONTROL Timezone]**: Definiera en specifik tidszon som ska användas som standard i alla arbetsflödets aktiviteter. Som standard är arbetsflödets tidszon den som definieras för den aktuella Campaign-operatorn.
Andra möjliga värden är:
   * **Tidszon för server** för att använda tidszonen på Adobe Campaign-programservern
   * **Operatörens tidszon** använder tidszonen för den Adobe Campaign-operator som kör arbetsflödet, enligt definitionen i operatörens profil, i klientkonsolen
   * **Databasens tidszon** för att använda databasserverns tidszon
   * En specifik tidszon

* **[!UICONTROL Supervisor(s)]**: När ett arbetsflöde misslyckas meddelas de operatorer som tillhör den operatorgrupp som valts i det här fältet via e-post.
* **[!UICONTROL Description]**: Använd det här fältet om du vill ange en beskrivning av arbetsflödet.

## Segmenteringsinställningar

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinställningar"
>abstract="I det här avsnittet kan du välja måldimension för målprofiler i arbetsflödet och välja att behålla arbetsflödesresultaten mellan två körningar. Det här alternativet bör endast användas för testning och får aldrig aktiveras i ett produktionsarbetsflöde."

* **[!UICONTROL Targeting dimension]**: Välj måldimensionen som ska användas för målprofiler: mottagare, mottagare, operatör, prenumeranter osv.
* **[!UICONTROL Keep the result of interim populations between two executions]**: Som standard behålls endast arbetsregister för den senaste körningen av arbetsflödet. Arbetstabeller från tidigare körningar rensas av ett tekniskt arbetsflöde, som körs dagligen.

  Om det här alternativet är aktiverat behålls arbetsregister även efter att arbetsflödet har körts. Du kan använda den i testsyfte och måste därför bara användas i utvecklings- eller staging-miljöer. Den får aldrig checkas in i ett produktionsarbetsflöde.

## Körningsinställningar

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Körningsinställningar"
>abstract="I det här avsnittet kan du konfigurera inställningar som är relaterade till arbetsflödets körning, t.ex. antalet dagar som arbetsflödeshistoriken sparas."

* **[!UICONTROL History in days]**: Anger efter hur många dagar som historiken måste rensas. Historiken innehåller element som är relaterade till arbetsflödet: loggar, uppgifter, händelser (tekniska objekt som är kopplade till arbetsflödesåtgärden). Standardvärdet är 30 dagar för färdiga arbetsflödesmallar. Historiken rensas av det tekniska arbetsflödet för databasrensning som utförs som standard varje dag

  >[!IMPORTANT]
  >
  >Om **[!UICONTROL History in days]** fältet lämnas tomt, dess värde betraktas som&quot;1&quot;, vilket innebär att historiken rensas efter 1 dag.

* **[!UICONTROL Default affinity]**: Om din installation innehåller flera arbetsflödesservrar använder du det här fältet för att välja vilken dator arbetsflödet ska köras på. Om värdet som definieras i det här fältet inte finns på någon server, kommer arbetsflödet att förbli väntande.

* **[!UICONTROL Save SQL queries in log]**: låter dig spara SQL-frågorna från arbetsflödet i loggarna. Den här funktionen är reserverad för avancerade användare. Det gäller arbetsflöden som innehåller riktade aktiviteter som **[!UICONTROL Build audience]**. När det här alternativet är aktiverat visas de SQL-frågor som skickas till databasen under arbetsflödeskörningen i arbetsflödets loggar, så att du kan analysera dem för att optimera frågor eller diagnostisera problem.

## Inställningar för felhantering

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Inställningar för felhantering"
>abstract="I det här avsnittet kan du hantera hur arbetsflödet ska fungera när ett fel inträffar under körningen (pausa/stoppa körningen eller ignorera fel)."

* **[!UICONTROL Error management]**: I det här fältet kan du definiera vilka åtgärder som ska vidtas om en arbetsflödesuppgift innehåller fel. Det finns två möjliga alternativ:

   * **[!UICONTROL Suspend the process]**: Arbetsflödet pausas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst kan du återuppta arbetsflödet med **[!UICONTROL Resume]** knappar.
   * **[!UICONTROL Ignore]**: Status för den aktivitet som utlöste felet ändras till **[!UICONTROL Failed]** men arbetsflödet behåller **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abord the process]**: Arbetsflödet stoppas automatiskt och dess status ändras till **[!UICONTROL Failed]**. Starta om arbetsflödet med **[!UICONTROL Start]** knappar.

* **[!UICONTROL Consecutive errors]**: Det här fältet blir tillgängligt när **[!UICONTROL Ignore]** värdet är markerat i **[!UICONTROL In case of errors]** fält. Du kan ange antalet fel som kan ignoreras innan processen stoppas. När det här numret har nåtts ändras arbetsflödets status till **[!UICONTROL Failed]**. Om värdet för det här fältet är 0 stoppas aldrig arbetsflödet oavsett antalet fel.
