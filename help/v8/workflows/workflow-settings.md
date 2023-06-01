---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 806e465b7c1df6cd26d68103c45b175371d73485
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 2%

---

# Konfigurera avancerade arbetsflödesinställningar {#workflow-settings}

När du organiserar arbetsflödesaktiviteter på arbetsytan kan du komma åt avancerade inställningar som är relaterade till arbetsflödet. Du kan till exempel ange en specifik tidszon för arbetsflödet, hantera arbetsflödets beteende om fel uppstår eller hantera den fördröjning efter vilken arbetsflödeshistoriken ska rensas.

Om du vill göra det klickar du på **[!UICONTROL Workflow settings]** -ikonen i det övre vänstra hörnet av arbetsytan, bredvid arbetsflödesetiketten.

![](assets/workflow-settings.png)

## Egenskaper för arbetsflöde {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Egenskaper för arbetsflöde"
>abstract="TBD"

Avsnittet för arbetsflödesegenskaper innehåller generiska egenskaper som också är tillgängliga när du skapar arbetsflödet.

* **[!UICONTROL Label]**: Etiketten för arbetsflödet som visas i listan.
* **[!UICONTROL Internal name]**: Arbetsflödets interna namn.
* **[!UICONTROL Folder]**: Mappen där arbetsflödet ska sparas.
* **[!UICONTROL Linked campaign]**: Det här fältet visas om arbetsflödet har skapats i en kampanj. Du kan öppna den associerade kampanjen.
* **[!UICONTROL Timezone]**: Definiera en specifik tidszon som ska användas som standard i alla arbetsflödets aktiviteter. Som standard är arbetsflödets tidszon den som definieras för den aktuella Campaign-operatorn.
* **[!UICONTROL Supervisor]**: När ett arbetsflöde är felaktigt meddelas de operatorer som tillhör arbetsflödesövervakningsgruppen via e-post, förutsatt att deras e-postadress anges i deras profil.
* **[!UICONTROL Description]**: Använd det här fältet om du vill ange en beskrivning av arbetsflödet.

## Segmenteringsinställningar

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinställningar"
>abstract="TBD"

* **[!UICONTROL Targeting dimension]**: Välj måldimensionen som ska användas för målprofiler: mottagare, mottagare, mottagare, operatör, abonnenter osv.
* **[!UICONTROL Keep the result of interim populations between two executions]**: Som standard behålls endast arbetsregister för den senaste körningen av arbetsflödet. Arbetstabeller från tidigare körningar rensas av ett tekniskt arbetsflöde, som körs dagligen.

   Om det här alternativet är aktiverat behålls arbetsregister även efter att arbetsflödet har körts. Du kan använda den i testsyfte och måste därför bara användas i utvecklings- eller staging-miljöer. Den får aldrig checkas in i ett produktionsarbetsflöde,

## Inställningar för arbetsflödeskörning

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Körningsinställningar"
>abstract="TBD"

* Historik på dagar: I arbetstabellerna i databasen finns en historik över körningar (uppgifter, händelser, loggar). Här kan du ange hur många dagar som ska arkiveras för det här arbetsflödet: rensningsprocessen tar bort de äldsta arkiven en gång om dagen. Om värdet i det här fältet är noll tas arkivet aldrig bort.

   Anger antalet dagar efter vilka historiken måste rensas. Historiken innehåller element som är relaterade till arbetsflödet: loggar, uppgifter, händelser (tekniska objekt som är länkade till arbetsflödet) samt filer som hämtats av **[!UICONTROL Transfer file]** aktivitet. Standardvärdet är 30 dagar för färdiga arbetsflödesmallar.

   Historiken rensas av det tekniska arbetsflödet för databasrensning som utförs som standard varje dag

   >[!IMPORTANT]
   >
   >Om **[!UICONTROL History in days]** fältet lämnas tomt, dess värde betraktas som&quot;1&quot;, vilket innebär att historiken rensas efter 1 dag.

* standardtillhörighet: I det här fältet kan du tvinga ett arbetsflöde eller en arbetsflödesaktivitet att köras på en viss dator.   Om installationen innehåller flera arbetsflödesservrar använder du det här fältet för att välja vilken dator arbetsflödet ska köras på. Om värdet som definieras i det här fältet inte finns på någon server, kommer arbetsflödet att förbli väntande.

* spara sql-frågor i loggen: Med kan du spara SQL-frågor från arbetsflödet i loggarna. (var kommer du åt SQL-loggar?)

   Den här funktionen är reserverad för avancerade användare. Det gäller arbetsflöden som innehåller riktade aktiviteter (fråga, union, skärning osv.). När det här alternativet är markerat visas de SQL-frågor som skickas till databasen under arbetsflödeskörningen i Adobe Campaign: Detta innebär att du kan analysera dem för att optimera frågor eller diagnostisera problem.

   Frågor visas i en **[!UICONTROL SQL logs]** som läggs till i arbetsflödet (utom kampanjarbetsflöden) och i **[!UICONTROL Properties]** när alternativet är aktiverat. The **[!UICONTROL Audit]** -fliken innehåller även SQL-frågor.

## Inställningar för felhantering

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Inställningar för felhantering"
>abstract="TBD"

* I det här fältet kan du definiera de åtgärder som ska vidtas om en arbetsflödesuppgift innehåller fel. Det finns två möjliga alternativ:

   Stoppa processen: arbetsflödet pausas automatiskt. arbetsflödets status ändras till Misslyckades. När problemet är löst startar du om arbetsflödet med hjälp av knapparna Start eller Starta om.

   Ignorera: status för den uppgift som utlöste felet ändras till Misslyckades, men arbetsflödet behåller statusen Started. Den här konfigurationen är relevant för återkommande uppgifter: om grenen innehåller en schemaläggare startar den normalt nästa gång arbetsflödet körs.

* Flera sekventiella fel: Det här fältet blir tillgängligt när Ignorera-värdet är markerat i fältet Vid fel. Du kan ange antalet fel som kan ignoreras innan processen stoppas. När det här numret har nåtts ändras arbetsflödets status till Misslyckad. Om värdet för det här fältet är 0 stoppas aldrig arbetsflödet oavsett antalet fel.
