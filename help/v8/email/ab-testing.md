---
audience: end-user
title: Skapa innehållsexperiment
description: Lär dig skapa innehållsexperiment i Adobe Campaign Web
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# Skapa innehållsexperiment {#content-experiment}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Innehållsexperiment - A/B-tester"
>abstract="Nu kan du definiera flera leveransvarianter för att testa vilka som fungerar bäst. Variera innehåll, ämne eller avsändare i olika e-postelement för att få optimala resultat."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"

## Om innehållsexperiment {#about-content-experiment}

Med hjälp av innehållsexperiment på Adobe Campaign Web kan du definiera flera olika leveransvarianter för A/B-tester för att mäta vilka som fungerar bäst för målgruppen. Du kan variera leveransinnehåll, ämne eller avsändare för att testa olika versioner och avgöra vilken variant som ger bäst resultat.

Du kan utföra A/B-tester på olika e-postelement som:

* **Ämnesrad**: testa olika ämnesrader för e-post för att se vilken som genererar den högsta öppna frekvensen
* **Avsändarnamn**: Experimentera med olika avsändarkombinationer
* **E-postinnehåll**: skapa flera innehållsversioner för att identifiera vilka enheter som har den bästa klickfrekvensen

>[!NOTE]
>
>* Innehållsexperiment är för närvarande endast tillgängliga för e-postkanaler.
>* A/B-testning stöds inte för transaktionsmeddelanden.
>* Max 3 behandlingar (varianter) per experiment.

## Skapa ett innehållsexperiment {#create-content-experiment}

Följ de här stegen för att lägga till ett innehållsexperiment i e-postleveransen:

1. Skapa en e-postleverans eller öppna ett befintligt utkast. [Lär dig hur du skapar ett e-postmeddelande](create-email.md)

1. Klicka på knappen **[!UICONTROL Create experiment]** i avsnittet **[!UICONTROL Content]** på egenskapssidan för e-postleverans.

   ![Skärmbild som visar knappen Skapa experiment i e-postegenskaper](assets/ab-testing-1.png){zoomable="yes"}

## Konfigurera experimenteringsinställningarna {#configure-experiment}

Konfigurera ditt experiment i följande avsnitt:

![Skärmbild som visar Experimentinställningar](assets/ab-testing-2.png){zoomable="yes"}

### Målgruppsinställningar {#audience-settings}

Definiera den procentandel av målpopulationen som ska ta emot experimentella varianter.

Ange ett värde för målgruppens storlek. Detta anger andelen mottagare som kommer att få en av experimentella varianter under testfasen.

* **Minst**: 1 %
* **Maximalt**: 100 %
* **Standard**: 10 %

Den återstående publiken (90 % som standard) får den vinnande varianten när experimentet är avslutat och vinnaren bestäms.

Om målgruppen är 10 000 mottagare och målgruppen är 10 %, kommer 1 000 mottagare att väljas ut slumpmässigt för att delta i experimentet. De återstående 9 000 mottagarna får den vinnande varianten när experimentet är slut.

### Vinnarstrategi {#winning-strategy}

Välj det mätvärde som ska användas för att bestämma den vinnande varianten:

* **[!UICONTROL Best open rate]** (standard): varianten med den högsta procentandelen e-post som öppnas vinner
* **[!UICONTROL Best click-through rate]**: varianten med det högsta procenttalet av klickningar i e-postmeddelandet vinner
* **[!UICONTROL Weakest unsubscription rate]**: varianten med den lägsta procentandelen för avanmälan vinner

Systemet spårar automatiskt dessa mått under experimentet och beräknar vilken variant som fungerar bäst enligt det valda kriteriet.

### Mottagarmetod {#sending-method}

Ange hur länge experimentet ska köras och välj sändningsmetod:

1. Ange varaktighetsvärdet i timmar. Experimentet kommer att pågå under denna period innan den vinnande varianten bestäms.

   * **Minst**: 3 timmar
   * **Maximalt**: 240 timmar (10 dagar)
   * **Standard**: 24 timmar

   >[!NOTE]
   >
   >Försäkra dig om att tidsåtgången för experimentet är tillräckligt lång för att samla in meningsfulla data. En kort varaktighet kanske inte ger tillräcklig statistisk signifikans, särskilt för mått som klickfrekvens som kan ta längre tid att ackumulera.

1. Välj hur den vinnande varianten ska skickas till den återstående populationen:

   * **[!UICONTROL Automatic sending]** aktiverad: Systemet skickar automatiskt den vinnande varianten till den återstående målgruppen när experimentet är slut.
   * **[!UICONTROL Automatic sending]** inaktiverad: du måste klicka på knappen **[!UICONTROL Send]** manuellt för att skicka den vinnande varianten när du har granskat experimentresultatet.

Om ingen variant uppnår betydligt bättre resultat än de andra i slutet av försöket skickas den första varianten till den återstående populationen. Se [avsnittet](#send-deliveries).

## Definiera innehållshantering {#define-content}

När du har sparat dina experimentella inställningar skapas en första behandling som standard. Nu måste du lägga till andra behandlingar (upp till tre) och definiera deras specifika innehåll.

1. Klicka på **[!UICONTROL Edit content]** i leveransegenskaperna. Bearbetningarna visas till vänster.

   ![Skärmbild som visar panelen för innehållsexperiment](assets/ab-testing-3.png){zoomable="yes"}

1. Klicka på knappen **[!UICONTROL Add treatment]** och definiera dess namn. Upprepa den här åtgärden för alla behandlingar du behöver lägga till. Du kan sedan ändra deras namn, duplicera och ta bort dem.

1. Klicka på varje behandling och anpassa följande:

   * **Avsändarnamn**: Anpassa vem som e-postmeddelandet verkar komma från
   * **Ämnesrad**: Skriv en unik ämnesrad för varje behandling
   * **E-postbrödtext**: Designa olika innehållsversioner med e-post-Designer

   ![Skärmbild med flera behandlingar](assets/ab-testing-4.png){zoomable="yes"}

1. Förhandsgranska varje behandling genom att klicka på behandlingen och sedan på **[!UICONTROL Simulate content]**.

## Starta experimentet och övervaka resultatet {#validate-start}

När du har definierat alla dina innehållsbehandlingar kan du validera och påbörja experimentet.

1. Klicka på **[!UICONTROL Review and send]** i leveransegenskaperna och sedan på **[!UICONTROL Prepare]**.

1. Klicka sedan på **[!UICONTROL Start experimentation]** för att påbörja A/B-testet.

   ![Skärmbild som visar knappen för att börja experimentera](assets/ab-testing-5.png){zoomable="yes"}

1. När du har experimenterat kan du övervaka de olika mätvärden som visas på kontrollpanelen för leverans.

Du kan avsluta experimentet genom att klicka på **[!UICONTROL Stop sending]**. Du kan också bestämma dig för att skicka manuellt före slutet av experimentet genom att klicka på **[!UICONTROL Select and send to winner]**.

>[!NOTE]
>
>Resultaten uppdateras nästan i realtid när mottagarna interagerar med e-postmeddelandet. Tidiga resultat kanske inte har statistisk betydelse - vi rekommenderar att du väntar tills experimentet är klart innan du fattar de slutgiltiga besluten.

## Skicka leveranser {#send-deliveries}

Sändningen kan utföras automatiskt eller manuellt, enligt vad du har valt i inställningarna för **[!UICONTROL Winner sending method]**. Se [avsnittet](#sending-method).

### Automatisk sändning {#automatic-sending}

För automatisk sändning analyserar systemet resultaten baserat på din vinnande strategi och avgör vilken behandling som vinner. Den vinnande behandlingen skickas automatiskt till den återstående publiken. Om ingen tydlig vinnare kommer fram väljs den första varianten.

### Manuell sändning {#manual-sending}

Om du konfigurerade manuell sändning granskar du resultatet när experimentet avslutas och klickar på **[!UICONTROL Send]** för att skicka den vinnande behandlingen. Om ingen klar vinnare kommer fram väljs den första behandlingen som standard, men du kan välja en annan.

## Visa slutresultat {#final-results}

När experimentet är klart och leveransen är klar får du tillgång till omfattande rapporter:

1. Klicka på **[!UICONTROL Reports]** på kontrollpanelen för leverans.

1. Navigera till rapportfliken **[!UICONTROL Experiments]** om du vill visa nyckeltal för prestanda för varje behandling.

## Bästa praxis {#best-practices}

Tänk på följande när du skapar innehållsexperiment:

* **Testa ett element i taget**: Testa varianter av ett enskilt element (t.ex. enbart ämnesraden eller endast innehållet) i stället för flera element samtidigt för att få tydligare resultat.

* **Välj lämplig varaktighet**: Tillåt tillräckligt med tid för statistisk signifikans:
   * För provning med öppen hastighet: 12-24 timmar räcker vanligtvis
   * För klickfrekvens: 24-48 timmar eller mer behövs
   * Större målgrupper kan behöva mindre tid, mindre målgrupper kan behöva längre

* **Anpassa målgruppens storlek**:
   * Se till att din experimentella målgrupp (den procentandel som tilldelas till testning) är tillräckligt stor för att skapa meningsfulla resultat
   * Allmänna riktlinjer: Minst 1 000 mottagare per behandling för tillförlitliga resultat

* **Testa regelbundet men inte överdrivet**: Utför experiment med viktiga kampanjer, men undvik att testa varje enskild sändning för att fokusera resurser på viktiga beslut.

* **Dokumentera dina inlärningar**: Spara register över experimentresultat för att informera om framtida kampanjstrategier.

## Relaterade ämnen {#related-topics}

* [Skapa din första e-postadress](create-email.md)
* [Konfigurera e-postinnehåll](edit-content.md)
* [Förhandsgranska och skicka e-post](../monitor/prepare-send.md)
* [Leveransrapporter via e-post](../reporting/email-report.md)
