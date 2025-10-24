---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
source-git-commit: 8ba304ef0bf922fc8057a5ee6f1e296805793735
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 1%

---

# Organisera aktiviteter {#orchestrate}

När du har [skapat ett arbetsflöde](create-workflow.md), oavsett om det är från arbetsflödesmenyn eller från en kampanj, kan du börja organisera de olika aktiviteterna som det utför. För att göra detta finns en visuell arbetsyta som gör att du kan skapa ett arbetsflödesdiagram. I det här diagrammet kan du lägga till olika aktiviteter och koppla dem i en sekventiell ordning.

## Lägg till aktiviteter {#add}

I det här skedet av konfigurationen visas diagrammet med en startikon som representerar början av arbetsflödet. Om du vill lägga till din första aktivitet klickar du på knappen **+** som är ansluten till startikonen.

En lista över aktiviteter som kan läggas till i diagrammet visas. Vilka aktiviteter som är tillgängliga beror på var du befinner dig i arbetsflödesdiagrammet. När du till exempel lägger till din första aktivitet kan du starta arbetsflödet genom att rikta in dig på en målgrupp, dela arbetsflödessökvägen eller ange en **Vänta** -aktivitet för att fördröja arbetsflödets körning. Efter en **Bygg målgruppsaktivitet** kan du förfina ditt mål med målinriktningsaktiviteter, skicka en leverans till din målgrupp med kanalaktiviteter eller ordna arbetsflödesprocessen med flödeskontrollaktiviteter.

![Ikon för att starta arbetsflöde och aktivitetsalternativ](assets/workflow-start.png){zoomable="yes"}

När en aktivitet har lagts till i diagrammet visas en höger ruta där du kan konfigurera den nyligen tillagda aktiviteten med specifika inställningar. Detaljerad information om hur du konfigurerar varje aktivitet finns i [det här avsnittet](activities/about-activities.md).

![Panelen Aktivitetskonfiguration](assets/workflow-configure-activities.png){zoomable="yes"}

Upprepa den här processen om du vill lägga till så många aktiviteter som behövs, beroende på vilka uppgifter ditt arbetsflöde utför. Du kan också infoga en ny aktivitet mellan två aktiviteter. Det gör du genom att klicka på knappen **+** för övergången mellan aktiviteterna, välja önskad aktivitet och konfigurera den i den högra rutan.

Om du vill ta bort en aktivitet markerar du den på arbetsytan och klickar på ikonen **Ta bort** i aktivitetsegenskaperna.

>[!TIP]
>
>Du kan anpassa namnet på övergångarna mellan varje aktivitet. Det gör du genom att markera övergången och ändra dess etikett i den högra rutan.

## Verktygsfältet {#toolbar}

Verktygsfältet, som finns i det övre högra hörnet av arbetsytan, innehåller alternativ för att enkelt ändra aktiviteterna och navigera på arbetsytan:

* **Flervalsläge**: Markera flera aktiviteter om du vill ta bort alla samtidigt eller kopiera och klistra in dem. Se [det här avsnittet](#copy).
* **Rotera**: Växla arbetsytan lodrätt.
* **Anpassa till skärmen**: Anpassa arbetsytans zoomnivå till skärmen.
* **Zooma ut** / **Zooma in**: Zooma ut eller in på arbetsytan.
* **Visningsschema**: Öppna en ögonblicksbild av arbetsytan som visar din plats.

![Verktygsfältsalternativ för arbetsytan &#x200B;](assets/workflow-toolbar.png){zoomable="yes"}{width="50%"}

## Hantera aktiviteter {#manage}

När du lägger till aktiviteter är åtgärdsknappar tillgängliga i egenskapsrutan, vilket gör att du kan utföra flera åtgärder.

![Aktivitetsknappar](assets/activity-action.png){zoomable="yes"}

Du kan:

* **Ta bort** aktiviteten från arbetsytan.
* **Inaktivera/aktivera** aktiviteten. När arbetsflödet körs körs inte inaktiverade aktiviteter och följande aktiviteter på samma sökväg, och arbetsflödet stoppas.
* **Pausa/återuppta** aktiviteten. När arbetsflödet körs pausas det vid den pausade aktiviteten. Motsvarande uppgift, samt alla som följer den i samma sökväg, körs inte.
* **Kopiera** aktiviteten. Se [det här avsnittet](#copy).
* **Flytta** en aktivitet och alla dess underordnade noder till en annan övergång. Se [det här avsnittet](#move).
* Få åtkomst till aktivitetens **körningsalternativ**.
* Åtkomst till aktivitetens **loggar och uppgifter**.

Flera **målaktiviteter**, till exempel **Kombinera** eller **Ta bort dubbletter**, gör att du kan bearbeta den återstående populationen och inkludera den i en ytterligare utgående övergång. Om du till exempel använder en **delad** -aktivitet består komplementet av den population som inte matchar någon av de tidigare definierade delmängderna. Aktivera alternativet **Generera komplement** om du vill använda den här funktionen.

![Delad aktivitet med komplementalternativ](assets/workflow-split-complement.png)

## Flytta eller kopiera aktiviteter {#move-copy}

### Kopiera och klistra in aktiviteter {#copy}

Du kan kopiera arbetsflödesaktiviteter och klistra in dem i vilket arbetsflöde som helst. Målarbetsflödet kan finnas på en annan webbläsarflik.

Du kan kopiera aktiviteter på två sätt:

* Kopiera en aktivitet med åtgärdsknappen.

  ![Kopiera en aktivitetsknapp](assets/workflow-copy.png){zoomable="yes"}{width="70%"}

* Kopiera flera aktiviteter med verktygsfältsknappen.

  ![Knappen Kopiera flera aktiviteter](assets/workflow-copy-2.png){zoomable="yes"}{width="70%"}

Om du vill klistra in de kopierade aktiviteterna klickar du på knappen **+** för en övergång och väljer Klistra in X-aktivitet.

![Alternativet Klistra in kopierade aktiviteter &#x200B;](assets/workflow-copy-3.png){zoomable="yes"}{width="50%"}

### Flytta aktiviteter och deras underordnade noder {#move}

Med Journey Optimizer kan du flytta en aktivitet, tillsammans med allt innehåll i dess underordnade noder (inklusive alla övergångar och aktiviteter i den), till slutet av en annan övergång i samma arbetsflöde.

Den här processen kopplar från aktiviteten och allt i den utgående övergången från den ursprungliga platsen, vilket flyttar den till den nya målövergången.

Så här flyttar du en aktivitet:

1. Markera aktiviteten som du vill flytta.
1. Klicka på knappen **Flytta** i aktivitetens egenskapspanel.
1. Markera övergången där du vill placera aktiviteten och dess utgående övergång och bekräfta sedan.

![Flytta aktivitet och underordnade noder](assets/activity-move.png)

## Körningsalternativ {#execution}

Med alla aktiviteter kan du hantera deras körningsalternativ. Markera en aktivitet och klicka på knappen **Körningsalternativ** . På så sätt kan du definiera aktivitetens körningsläge och beteende vid fel.

![Panelen Körningsalternativ](assets/workflow-execution-options.png){zoomable="yes"}{width="70%"}

### Egenskaper {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_activity_execution_options_properties"
>title="Aktivitetsegenskaper"
>abstract="I det här avsnittet kan du konfigurera körningsinställningar för en aktivitet, inklusive vilken åtgärd som ska utföras, maximal varaktighet, tidszon, datortillhörighet och asynkront beteende."

I fältet **Körning** kan du definiera åtgärden som ska utföras när aktiviteten startar.

I fältet **Maximal körningstid** kan du ange en varaktighet som t.ex. &quot;30s&quot; eller &quot;1h&quot;. Om aktiviteten inte har slutförts efter den angivna varaktigheten utlöses en varning. Detta påverkar inte arbetsflödets funktioner.

I fältet **Tidszon** kan du välja aktivitetens tidszon. Adobe Campaign hanterar tidsskillnader mellan flera länder i samma instans. Inställningen som används konfigureras när instansen skapas.

I fältet **Tillhörighet** kan du tvinga ett arbetsflöde eller en arbetsflödesaktivitet att köras på en viss dator. Om du vill göra det anger du en eller flera tillhörigheter för arbetsflödet eller aktiviteten i fråga.

I fältet **Beteende** kan du definiera proceduren som ska följas om asynkrona uppgifter används.

### Felhantering {#execution-options}

>[!CONTEXTUALHELP]
>id="acw_workflow_activity_execution_options_error"
>title="Initieringsskript"
>abstract="I det här avsnittet kan du definiera vad som ska hända om en aktivitet misslyckas. Du kan välja åtgärder som att stoppa arbetsflödet, gå till nästa aktivitet eller utlösa en anpassad felhanteringsprocess."

I fältet **I händelse av fel** kan du ange vilken åtgärd som ska utföras om aktiviteten påträffar ett fel. Se [avsnittet](workflow-settings.md#error-settings).

### Initieringsskript {#initialization-options}

>[!CONTEXTUALHELP]
>id="acw_workflow_activity_execution_options_initialization"
>title="Initieringsskript"
>abstract="I det här avsnittet kan du lägga till JavaScript som körs när aktiviteten startar. Använd det för att initiera variabler, ange parametrar eller förbereda data som är specifika för den aktivitetens körning."

Med **initieringsskriptet** kan du initiera variabler eller ändra aktivitetsegenskaper. Klicka på knappen **Redigera kod** och skriv det kodfragment som ska köras. Skriptet anropas när aktiviteten körs. Se avsnittet som rör [händelsevariabler](../workflows/event-variables.md).

## Exempel {#example}

Här följer ett exempel på ett arbetsflöde som utformats för att skicka ett e-postmeddelande till alla kunder (andra än VIP-kunder) med ett e-postmeddelande som är intresserade av kaffemaskiner.

![Exempeldiagram för arbetsflöde](assets/workflow-example.png){zoomable="yes"}

För att uppnå detta har följande verksamheter lagts till:

* En **[!UICONTROL Fork]**-aktivitet som delar upp arbetsflödet i tre sökvägar (en för varje kundgrupp),
* **[!UICONTROL Build audience]** aktiviteter för att rikta sig till de tre uppsättningarna kunder:
   * Kunder med e-post
   * Kunder som tillhör den befintliga målgruppen&quot;Intresserad av kaffemaskiner&quot;,
   * Kunder som tillhör den befintliga målgruppen VIP att belöna.
* En **[!UICONTROL Combine]**-aktivitet som grupperar kunder med ett e-postmeddelande och de som är intresserade av kaffemaskiner,
* En **[!UICONTROL Combine]**-aktivitet som utesluter VIP-kunder,
* En **[!UICONTROL Email delivery]**-aktivitet som skickar ett e-postmeddelande till de resulterande kunderna.

När du har slutfört arbetsflödet lägger du till en **[!UICONTROL End]**-aktivitet i slutet av diagrammet. Den här aktiviteten markerar slutet av ett arbetsflöde och har ingen funktionell inverkan.

När du har utformat arbetsflödesdiagrammet kan du köra arbetsflödet och spåra förloppet för de olika uppgifterna. [Lär dig hur du startar ett arbetsflöde och övervakar dess körning](start-monitor-workflows.md).