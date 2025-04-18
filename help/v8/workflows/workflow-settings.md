---
audience: end-user
title: Konfigurera inställningar för arbetsflöde
description: Lär dig hur du konfigurerar arbetsflödesinställningar med Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 1%

---

# Konfigurera inställningar för arbetsflöde {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Egenskaper för arbetsflöde"
>abstract="På den här skärmen väljer du den mall som ska användas för att skapa arbetsflödet och anger en etikett. Expandera avsnittet **Ytterligare alternativ** om du vill konfigurera fler inställningar, till exempel arbetsflödets interna namn, dess mapp, tidszon och övervakningsgrupp. Vi rekommenderar starkt att du väljer en grupp för ansvariga så att de får ett meddelande om ett fel inträffar."

När du skapar ett arbetsflöde eller organiserar arbetsflödesaktiviteter på arbetsytan får du tillgång till avancerade inställningar för arbetsflödet. Du kan till exempel ange en specifik tidszon för arbetsflödet, hantera arbetsflödets beteende vid fel eller hantera den fördröjning efter vilken arbetsflödeshistoriken rensas.

De här inställningarna är förkonfigurerade i mallen som valdes när arbetsflödet skapades, men kan redigeras efter behov för det aktuella arbetsflödet.

![Knappgränssnitt för arbetsflödesinställningar](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Egenskaper för arbetsflöde {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Egenskaper för arbetsflöde"
>abstract="I det här avsnittet finns allmänna arbetsflödesegenskaper som också är tillgängliga när du skapar arbetsflödet. Du kan välja vilken mall som ska användas för att skapa arbetsflödet och ange en etikett. Expandera avsnittet Ytterligare alternativ om du vill konfigurera särskilda inställningar, till exempel lagringsmapp för arbetsflöde eller tidszon."

Avsnittet **[!UICONTROL Properties]** innehåller allmänna inställningar som kan konfigureras när du skapar ett arbetsflöde. Om du vill komma åt egenskaperna för ett befintligt arbetsflöde klickar du på knappen **[!UICONTROL Settings]** i åtgärdsfältet ovanför arbetsytan.

![Gränssnitt för arbetsflödesinställningar](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

Egenskaperna är:

* **[!UICONTROL Label]** för arbetsflödet som visas i listan.
* Arbetsflödets **[!UICONTROL Internal name]**.
* **[!UICONTROL Folder]** där arbetsflödet ska sparas.
* Standardvärdet **[!UICONTROL Timezone]** som ska användas i alla arbetsflödets aktiviteter. Som standard är arbetsflödets tidszon den som definieras för den aktuella Campaign-operatorn.
Möjliga värden är:
   * **Serverns tidszon** om du vill använda tidszonen för Adobe Campaign-programservern.
   * **Operatörens tidszon** används för att använda tidszonen för den Adobe Campaign-operator som kör arbetsflödet, enligt definitionen i operatorns profil i klientkonsolen.
   * **Tidszon för databasen** som använder tidszonen för databasservern.
   * En specifik tidszon.
* När ett arbetsflöde misslyckas meddelas de operatorer som tillhör den operatörsgrupp som valts i fältet **[!UICONTROL Supervisor(s)]** via e-post.
* Ange **[!UICONTROL Description]** i arbetsflödet.

När arbetsflödet är [associerat med en kampanj](create-workflow.md) visas det i fältet **[!UICONTROL Linked campaign]**. Öppna den associerade kampanjen från det fältet.

## Segmenteringsinställningar {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinställningar"
>abstract="I det här avsnittet kan du välja måldimension för målprofiler i arbetsflödet och välja att behålla arbetsflödesresultaten mellan två körningar. Det här alternativet bör endast användas för testning och får aldrig aktiveras i ett produktionsarbetsflöde."

* **[!UICONTROL Targeting dimension]**: Välj den måldimension som ska användas för målprofiler, till exempel mottagare, mottagare, operatorer, prenumeranter och andra. [Läs mer om måldimensioner](../audience/targeting-dimensions.md).

* **[!UICONTROL Keep the result of interim populations between two executions]**: Som standard behålls endast arbetsregister för den senaste körningen av arbetsflödet. Arbetstabeller från tidigare körningar rensas av ett tekniskt arbetsflöde, som körs dagligen.

  Om det här alternativet är aktiverat behålls arbetsregister även efter att arbetsflödet har körts. Använd det för testning och kontrollera att det används **endast** i utvecklings- eller staging-miljöer. Den får aldrig checkas in i ett produktionsarbetsflöde.

## Körningsinställningar {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Körningsinställningar"
>abstract="I det här avsnittet kan du konfigurera inställningar för arbetsflödets körning, t.ex. antalet dagar som arbetsflödeshistoriken sparas."

* **[!UICONTROL History in days]**: Anger efter hur många dagar som historiken måste rensas. Historiken innehåller element som är relaterade till arbetsflödet, till exempel loggar, uppgifter och händelser (tekniska objekt som är kopplade till arbetsflödesåtgärden). Standardvärdet är 30 dagar för färdiga arbetsflödesmallar. Historiken rensas av det tekniska arbetsflödet för databasrensning som utförs varje dag.

  >[!IMPORTANT]
  >
  >Om fältet **[!UICONTROL History in days]** lämnas tomt betraktas dess värde som &quot;1&quot;, vilket innebär att historiken rensas efter 1 dag.

* **[!UICONTROL Default affinity]**: Om din installation innehåller flera arbetsflödesservrar använder du det här fältet för att ange på vilken server arbetsflödet ska köras. Detta framtvingar körning av det arbetsflödet på en viss server. Välj ett befintligt tillhörighetsnamn, men se till att du inte använder blanksteg eller skiljetecken. Om du använder olika servrar anger du olika namn avgränsade med kommatecken.

  >[!IMPORTANT]
  >
  >Om värdet som definieras i det här fältet inte finns på någon server, kommer arbetsflödet att förbli väntande.

* **[!UICONTROL Save SQL queries in log]**: Markera det här alternativet om du vill spara SQL-frågorna från arbetsflödet i loggarna. Den här funktionen är reserverad för avancerade användare. Det gäller arbetsflöden som innehåller riktade aktiviteter, till exempel **[!UICONTROL Build audience]**. När det här alternativet är aktiverat visas de SQL-frågor som skickas till databasen under arbetsflödeskörningen i arbetsflödets loggar, så att du kan analysera dem för att optimera frågor eller diagnostisera problem.

## Inställningar för felhantering {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Inställningar för felhantering"
>abstract="I det här avsnittet kan du definiera hur arbetsflödet ska hantera fel under körningen. Du kan välja att pausa processen, ignorera ett visst antal fel eller avbryta arbetsflödets körning."

* **[!UICONTROL Error management]**: I det här fältet kan du definiera de åtgärder som ska vidtas om en arbetsflödesuppgift innehåller fel. Det finns tre möjliga alternativ:

   * **[!UICONTROL Suspend the process]**: Arbetsflödet pausas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst kan du återuppta arbetsflödet med **[!UICONTROL Resume]**-knapparna.
   * **[!UICONTROL Ignore]**: Statusen för den uppgift som utlöste felet ändras till **[!UICONTROL Failed]**, men arbetsflödet behåller statusen **[!UICONTROL Started]**. <!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abort the process]**: Arbetsflödet stoppas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst startar du om arbetsflödet med **[!UICONTROL Start]**-knapparna.

* **[!UICONTROL Consecutive errors]**: Det här fältet blir tillgängligt när värdet **[!UICONTROL Ignore]** har valts i fältet **[!UICONTROL In case of errors]**. Ange antalet fel som kan ignoreras innan processen stoppas. När det här numret har nåtts ändras arbetsflödets status till **[!UICONTROL Failed]**. Om värdet för det här fältet är 0 stoppas aldrig arbetsflödet oavsett antalet fel.

## Initieringsskript {#initialization-script}

Med **initieringsskriptet** kan du initiera variabler eller ändra aktivitetsegenskaper. Klicka på knappen **Redigera kod** och skriv det kodfragment som ska köras. Skriptet anropas när arbetsflödet körs. Se avsnittet som rör [händelsevariabler](../workflows/event-variables.md).