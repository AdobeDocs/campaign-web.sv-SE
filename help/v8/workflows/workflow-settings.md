---
audience: end-user
title: Konfigurera inställningar för arbetsflöde
description: Lär dig hur du konfigurerar arbetsflödesinställningar med Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: 865978dd8083723187a90647060f8758d4d888be
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---


# Konfigurera inställningar för arbetsflöde {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Egenskaper för arbetsflöde"
>abstract="På den här skärmen väljer du den mall som ska användas för att skapa arbetsflödet och anger en etikett. Expandera avsnittet **Ytterligare alternativ** om du vill konfigurera fler inställningar, till exempel arbetsflödets interna namn, mapp, tidszon och övervakargrupp. Vi rekommenderar starkt att du väljer en grupp för ansvariga så att de får ett meddelande om ett fel inträffar."

När du skapar ett arbetsflöde eller organiserar arbetsflödesaktiviteter på arbetsytan kan du komma åt avancerade inställningar som är relaterade till arbetsflödet. Du kan till exempel ange en specifik tidszon för arbetsflödet, hantera arbetsflödets beteende om fel uppstår eller hantera den fördröjning efter vilken arbetsflödeshistoriken ska rensas.

De här inställningarna är förkonfigurerade i mallen som valdes när arbetsflödet skapades, men kan redigeras efter behov för det aktuella arbetsflödet.

![](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Egenskaper för arbetsflöde {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Egenskaper för arbetsflöde"
>abstract="Det här avsnittet innehåller allmänna arbetsflödesegenskaper som också är tillgängliga när du skapar arbetsflödet. Du kan välja den mall som ska användas för att skapa arbetsflödet och ange en etikett. Expandera avsnittet Ytterligare alternativ för att konfigurera specifika inställningar, till exempel mappen för arbetsflödets lagring eller tidszonen."

Avsnittet **[!UICONTROL Properties]** innehåller allmänna inställningar som kan konfigureras när ett arbetsflöde skapas. Om du vill få tillgång till egenskaperna för ett befintligt arbetsflöde klickar du på knappen **[!UICONTROL Settings]** som finns i åtgärdsfältet ovanför arbetsytan.


![](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}


Dessa egenskaper är:

* **[!UICONTROL Label]** för arbetsflödet som visas i listan.
* Arbetsflödets **[!UICONTROL Internal name]**.
* **[!UICONTROL Folder]** där arbetsflödet ska sparas.
* Standardvärdet **[!UICONTROL Timezone]** som ska användas i alla arbetsflödets aktiviteter. Som standard är arbetsflödets tidszon den som definieras för den aktuella Campaign-operatorn.
Möjliga värden är:
   * **Serverns tidszon** för att använda Adobe Campaign-programserverns tidszon
   * **Operatörens tidszon** använder tidszonen för den Adobe Campaign-operator som kör arbetsflödet, enligt operatorns profil, i klientkonsolen
   * **Tidszon för databasen** som använder databasserverns tidszon
   * En specifik tidszon
* När ett arbetsflöde misslyckas meddelas de operatorer som tillhör den operatorgrupp som valts i fältet **[!UICONTROL Supervisor(s)]** via e-post.
* Du kan även ange **[!UICONTROL Description]** i arbetsflödet.

När arbetsflödet är [associerat med en kampanj](create-workflow.md) visas det i fältet **[!UICONTROL Linked campaign]**. Du kan öppna den associerade kampanjen från det fältet.


## Segmenteringsinställningar  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinställningar"
>abstract="I det här avsnittet kan du välja måldimension för målprofiler i arbetsflödet och välja att behålla arbetsflödesresultaten mellan två körningar. Det här alternativet bör endast användas för testning och får aldrig aktiveras i ett produktionsarbetsflöde."

* **[!UICONTROL Targeting dimension]**: Välj måldimensionen som ska användas för målprofiler: mottagare, mottagare, operatör, prenumeranter osv. [Läs mer om måldimensioner](../audience/targeting-dimensions.md)

* **[!UICONTROL Keep the result of interim populations between two executions]**: Som standard sparas bara arbetsregistren från den senaste körningen av arbetsflödet. Arbetstabeller från tidigare körningar rensas av ett tekniskt arbetsflöde som körs dagligen.

  Om det här alternativet är aktiverat kommer arbetsregister att sparas även efter att arbetsflödet har körts. Du kan använda den i testsyfte och måste därför bara användas **i utvecklings- eller mellanlagringsmiljöer.** Det får aldrig kontrolleras i ett produktionsarbetsflöde.

## Körningsinställningar  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Körningsinställningar"
>abstract="I det här avsnittet kan du konfigurera inställningar som är relaterade till arbetsflödets körning, t.ex. antalet dagar som arbetsflödeshistoriken sparas."

* **[!UICONTROL History in days]**: Anger efter hur många dagar som historiken måste rensas. Historiken innehåller element som är relaterade till arbetsflödet: loggar, uppgifter, händelser (tekniska objekt som är kopplade till arbetsflödesåtgärden). Standardvärdet är 30 dagar för färdiga arbetsflödesmallar. Rensa historiken utförs av det tekniska arbetsflödet för databasrensning, som körs varje dag som standard

  >[!IMPORTANT]
  >
  >Om fältet **[!UICONTROL History in days]** lämnas tomt kommer dess värde att betraktas som &quot;1&quot;, vilket innebär att historiken rensas efter 1 dag.

* **[!UICONTROL Default affinity]**: Om installationen innehåller flera arbetsflödesservrar använder du det här fältet för att ange vilken server som arbetsflödet ska köras på. Detta framtvingar körning av det arbetsflödet på en viss server. Du kan välja ett befintligt tillhörighetsnamn, men se till att du inte använder blanksteg eller skiljetecken. Om du använder olika servrar anger du olika namn, avgränsade med kommatecken.

  >[!IMPORTANT]
  >
  >Om värdet som definieras i det här fältet inte finns på någon server, kommer arbetsflödet att förbli väntande.


* **[!UICONTROL Save SQL queries in log]**: Markera det här alternativet om du vill spara SQL-frågorna från arbetsflödet i loggarna. Den här funktionen är reserverad för avancerade användare. Det gäller arbetsflöden som innehåller målinriktade aktiviteter som **[!UICONTROL Build audience]**. När det här alternativet är aktiverat visas de SQL-frågor som skickas till databasen under arbetsflödeskörningen i arbetsflödets loggar, så att du kan analysera dem för att optimera frågor eller diagnostisera problem.

## Inställningar för felhantering  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Inställningar för felhantering"
>abstract="I det här avsnittet kan du ange hur arbetsflödet ska hantera fel under körningen. Du kan välja att pausa processen, ignorera ett visst antal fel eller stoppa arbetsflödeskörningen."

* **[!UICONTROL Error management]**: I det här fältet anger du vilka åtgärder som ska vidtas om en arbetsflödesuppgift innehåller fel. Det finns tre möjliga alternativ:

   * **[!UICONTROL Suspend the process]**: Arbetsflödet pausas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst kan du återuppta arbetsflödet med **[!UICONTROL Resume]**-knapparna.
   * **[!UICONTROL Ignore]**: Statusen för den uppgift som utlöste felet ändras till **[!UICONTROL Failed]**, men arbetsflödet behåller statusen **[!UICONTROL Started]**. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abort the process]**: Arbetsflödet stoppas automatiskt och dess status ändras till **[!UICONTROL Failed]**. När problemet är löst startar du om arbetsflödet med **[!UICONTROL Start]**-knapparna.

* **[!UICONTROL Consecutive errors]**: Det här fältet blir tillgängligt när värdet **[!UICONTROL Ignore]** har valts i fältet **[!UICONTROL In case of errors]**. Du kan ange antalet fel som kan ignoreras innan processen stoppas. När det här numret har nåtts ändras arbetsflödets status till **[!UICONTROL Failed]**. Om värdet för det här fältet är 0 stoppas arbetsflödet aldrig, oavsett antalet fel.

## Initieringsskript {#initialization-script}

Med **initieringsskriptet** kan du initiera variabler eller ändra aktivitetsegenskaper. Klicka på knappen **Redigera kod** och skriv det kodfragment som ska köras. Skriptet anropas när arbetsflödet körs. Se avsnittet som rör [händelsevariabler](../workflows/event-variables.md).

