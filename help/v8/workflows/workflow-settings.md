---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 60cd0ed8dcbe3e6003c1cde674fe3441d6d88869
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 2%

---

# Konfigurera arbetsflödesinställningarna {#workflow-settings}

content TBD

definiera inställningar som är tillgängliga från knappen på arbetsytan
<!--à reformuler-->

## Egenskaper för arbetsflöde {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Egenskaper för arbetsflöde"
>abstract="TBD"

(= samma som när du skapar arbetsflödet ? att kontrollera)

* Etikett
* Ytterligare alternativ
* Internt namn
* Mapp
* Länkad kampanj > kan ändra den. I så fall försvinner arbetsflödet från den aktuella kampanjen och visas i den nya länkade kampanjen
* Tidszon: Definiera en specifik tidszon som ska användas som standard i alla arbetsflödets aktiviteter. Som standard är arbetsflödets tidszon den som definieras för den aktuella Campaign-operatorn.
* Ansvarig: När ett arbetsflöde är felaktigt meddelas de operatorer som tillhör arbetsflödesövervakningsgruppen via e-post, förutsatt att deras e-postadress anges i deras profil. Den här gruppen är markerad i **[!UICONTROL Supervisor(s)]** i arbetsflödesegenskaperna.
* description

## Segmenteringsinställningar

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinställningar"
>abstract="TBD"

* målgruppsdimension:

   Vid datasegmenteringsåtgärder mappas målnyckeln till en filtreringsdimension. Med måldimensionen kan du definiera målgruppen för åtgärden: mottagare, mottagare, mottagare, operatör, abonnenter osv. Filtreringsdimensionen gör att du kan välja populationen baserat på vissa kriterier: kontraktsägare, nyhetsbrev, prenumeranter osv.

* bevara resultat: The **Behåll resultatet från mellanliggande populationer mellan två avrättningar** Alternativet håller temporära tabeller mellan två körningar av ett arbetsflöde.  Den är tillgänglig i arbetsflödesegenskapernas **[!UICONTROL General]** och kan användas för utveckling och testning för att övervaka data och kontrollera resultat. Du kan använda det här alternativet i utvecklingsmiljöer, men aldrig använda det i produktionsmiljöer. Om du behåller tillfälliga tabeller kan databasens storlek öka avsevärt och så småningom kan storleksgränsen nås. Dessutom kommer säkerhetskopieringen att bli långsammare.

   Endast arbetsregister för den senaste körningen av arbetsflödet behålls. Arbetsregister från tidigare körningar rensas av **[!UICONTROL cleanup]** arbetsflöde, som körs dagligen.

   >[!CAUTION]
   >
   >Det här alternativet måste **aldrig** checkas in i **produktion** arbetsflöde. Det här alternativet används för att analysera resultaten och är utformat endast för teständamål och ska därför endast användas i utvecklings- eller stagingmiljöer.

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
