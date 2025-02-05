---
audience: end-user
title: Arbeta med typologier
description: Lär dig hur du arbetar med typologier och typologiregler för att styra, filtrera och övervaka hur leveranser skickas.
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: c759dd72e2ca3d11b4dad0cd38410d699b651cad
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---

# Arbeta med typologier {#typologies}

>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Typologiregler och typologiregler"
>abstract="Typologier gör att ni kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel tas inte med i leveransgrupperna under beredningsfasen."

## Om typologier

Typologier gör att ni kan standardisera affärspraxis för alla leveranser. En **typologi** är en samling **typologiregler** som gör att du kan kontrollera, filtrera och prioritera sändning av leveranser. Profiler som matchar kriterier inom en typologiregel tas inte med i leveransgrupperna under beredningsfasen.

Typsnitten ser till att dina leveranser alltid innehåller vissa element (t.ex. en länk för att avbryta prenumerationen eller en ämnesrad) eller filtreringsregler som utesluter grupper från det avsedda målet (t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder).

Typologier är tillgängliga via menyn **[!UICONTROL Administration]** > **[!UICONTROL Business rules]**. Från den här skärmen kan du komma åt alla befintliga typologier och typologiregler, eller skapa nya baserat på dina behov.

![](assets/business-rules-list.png)

>[!NOTE]
>
>Listan **[!UICONTROL Typology rules]** visar alla befintliga regler som har skapats hittills i webbanvändargränssnittet eller klientkonsolen. Endast **Kontroll** - och **Filtrering**-regler kan skapas i webbanvändargränssnittet. Om du vill skapa andra typer av typologiregler, till exempel tryck- eller kapacitetsregler, använder du klientkonsolen Campaign v8. [Lär dig skapa typologiregler i klientkonsolen](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

De viktigaste stegen för att tillämpa typologier i meddelanden är följande:

1. [Skapa en typologi](#typology).
1. [Skapa typologiregler](#typology-rules).
1. [Referera till typologiregler i typologin](#add-rules).
1. [Använd typologin för ett meddelande](#message).

## Skapa en typologi {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Typologiegenskaper"
>abstract="Definiera typologiens egenskaper och expandera avsnittet **[!UICONTROL Additional options]** för att få åtkomst till avancerade inställningar. Använd fältet **[!UICONTROL IP affinity]** för att associera IP-tillhörigheter med typologier. På så sätt kan du bättre kontrollera den utgående SMTP-trafiken genom att definiera vilka specifika IP-adresser som kan användas för varje tillhörighet."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="IP-tillhörighet"
>abstract="Genom att hantera tillhörigheter med IP-adresser får du bättre kontroll över utgående SMTP-trafik genom att koppla olika IP-adresser till varje typ av trafik beroende på vilken typ av leveransåtgärd det är fråga om."

Så här skapar du en typologi:

1. Gå till **[!UICONTROL Business rules]**-menyn och välj fliken **[!UICONTROL Typology]**.

1. Klicka på knappen **[!UICONTROL Create typology]** och ange **[!UICONTROL Label]** som typologi.

1. Expandera avsnittet **[!UICONTROL Additional options]** om du vill definiera avancerade inställningar som typologiens interna namn, lagringsmapp och beskrivning.

   ![](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >I fältet **[!UICONTROL IP affinity]** kan du associera IP-tillhörigheter med typologier. På så sätt kan du bättre kontrollera den utgående SMTP-trafiken genom att definiera vilka specifika IP-adresser som kan användas för varje tillhörighet.  Du kan till exempel använda en affinitet per land eller underdomän. Du kan sedan skapa en typologi per land och länka varje tillhörighet till motsvarande typologi.

1. Klicka på **[!UICONTROL Create]** för att bekräfta att typologin har skapats.

Typologin öppnar detaljer öppna. Från den här skärmen kan du direkt referera till befintliga typologiregler. Du kan också skapa nya typologiregler och referera till dem i typologin senare:
* [Lär dig skapa en typologiregel](#add-rules)
* [Lär dig referera till regler i en typologi](#add-rules)

## Skapa en typologiregel {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Egenskaper för typologiregel"
>abstract="Definiera typologiregelns egenskaper. **Kontroll**-regler verifierar meddelandekvalitet och giltighet före sändning, medan **Filtrering**-regler exkluderar segment för målgruppen baserat på specifika kriterier.<br/><br/>Du kan också ändra regelns körningsordning för att hantera sekvensen i vilken typologiregler körs när flera regler av samma typ körs under samma meddelandebearbetningsfas."

Om du vill skapa en typologiregel går du till menyn **[!UICONTROL Business rules]** och väljer fliken **[!UICONTROL Typology rules]**.

Klicka på knappen **[!UICONTROL Create typology rule]** och följ sedan stegen som beskrivs nedan.

### Definiera typologiregelns egenskaper {#properties}

Definiera typologiregelns egenskaper:

1. Ange **[!UICONTROL Label]** som regel.

   ![](assets/business-rules-control-rule.png)

1. Välj typologiregelns **[!UICONTROL Type]**:

   * **Kontroll**: Garanterar meddelandekvalitet och giltighet före sändning (t.ex. teckenvisning, SMS-längd, adressformat, URL-förkortning). De skapas med ett skriptgränssnitt som definierar komplex logik för innehållskontroller och ändringar.

   * **Filtreringsreglerna** exkluderar segment för målgruppen baserat på specifika kriterier (t.ex. ålder, plats, land, telefonnummer). Dessa regler är kopplade till en målinriktningsdimension.

   >[!NOTE]
   >
   >För närvarande går det bara att skapa typologireglerna **Kontroll** och **Filtering** från webbanvändargränssnittet. Om du vill skapa andra typer av regler använder du klientkonsolen. [Lär dig skapa typologiregler i klientkonsolen](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. Välj en **[!UICONTROL Channel]** att associera med regeln.

1. Växla av alternativet **[!UICONTROL Active]** om du inte vill att regeln ska vara aktiv direkt efter att den har skapats.

1. Definiera regeln **[!UICONTROL Execution order]**.

   Som standard är typologiregelordningen inställd på 50. Du kan anpassa det här värdet för att hantera den sekvens i vilken typologiregler ska köras när flera regler av samma typ körs under samma meddelandebearbetningsfas. En filtreringsregel med körningsordningen 20 körs till exempel före en filtreringsregel med körningsordningen 30.

1. Expandera avsnittet **[!UICONTROL Additional options]** om du vill komma åt avancerade inställningar som regelns interna namn, mapplagring och beskrivning.

1. För kontrollregler finns ytterligare två regler i de extra alternativen. De gör att du kan ange när regeln ska tillämpas och dess varningsnivå:

   * **[!UICONTROL Phase]**: I det här fältet kan du ange vid vilken tidpunkt i leveranscykeln regeln ska tillämpas. Välj det värde som ska användas i listrutan **[!UICONTROL Phase]**. Expandera avsnittet nedan om du vill ha mer information om möjliga värden.

   +++Reglerfaser för kontroll:

   **[!UICONTROL At the start of targeting]**: Om du vill förhindra att personaliseringssteget körs om fel uppstår kan du tillämpa kontrollregeln här.

   **[!UICONTROL After targeting]**: Välj den här fasen om du behöver känna till målvolymen för att kunna använda kontrollregeln. Kontrollregeln Kontrollera korrekturstorlek gäller till exempel efter varje målfas: den här regeln förhindrar meddelandepersonalisering om det finns för många korrekturmottagare.

   **[!UICONTROL At the start of personalization]**: Den här fasen måste väljas om kontrollen gäller godkännande av meddelandeanpassning. Anpassning av meddelanden utförs under analysfasen.

   **[!UICONTROL At the end of the analysis]**:Välj den här fasen när en kontroll kräver att meddelandepersonalisering ska vara slutförd.

+++

   * **[!UICONTROL Level]**: Med det här alternativet kan du ange regelns varningsnivå. Expandera avsnittet nedan om du vill ha mer information.

   +++Ctrl-linjenivåer:

   **[!UICONTROL Error]**: Stoppa meddelandeförberedelsen.

   **[!UICONTROL Warning]**: Visa en varning i förberedelseloggarna.

   **[!UICONTROL Info]**: Visa information i förberedelseloggarna.

   <!--**[!UICONTROL Status]**:-->

   **[!UICONTROL Verbose]**: Visa information i serverloggarna.

+++

### Bygg regelinnehållet {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtrering"
>abstract="**Filtreringsreglerna** exkluderar segment för målgruppen baserat på specifika kriterier (t.ex. ålder, plats, land, telefonnummer). Markera typologiregelns måldimension och klicka på knappen **[!UICONTROL Add rules]** för att få åtkomst till frågemodelleraren och skapa regeln."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Code"
>abstract="**Kontroll**-regler verifierar meddelandekvalitet och giltighet före sändning (t.ex. teckenvisning, SMS-längd, adressformat, URL-förkortning). De skapas med JavaScript-kod."

När typologiregelns egenskaper har definierats kan du skapa regelns innehåll.

* För **kontrollregler** klickar du på knappen **Redigera kod** och anger logiken för regeln med JavaScript. I exemplet nedan skapar vi en regel som visar en varning i loggarna om målet är tomt.

  ![](assets/business-rules-code.png)

* För **filtreringsregler** väljer du måldimensionen och klickar på knappen **[!UICONTROL Add rules]** för att definiera filtreringsvillkor med [frågemodelleraren](../query/query-modeler-overview.md).

  ![](assets/business-rules-query.png)

När regeln är klar klickar du på knappen **[!UICONTROL Create]** för att skapa typologiregeln. Du kan nu referera regeln till en typologi för att använda den på meddelanden.

## Referera till typologiregler i en typologi {#add-rules}

Följ de här stegen för att referera till en eller flera regel(er) i en typologi:

1. Navigera till fliken **[!UICONTROL Typology]** och öppna den typologi där du vill referera till reglerna.

1. Välj fliken **[!UICONTROL Typology rules]** och klicka på knappen **[!UICONTROL Add typology rule'(s)]**.

   ![](assets/business-rules-reference.png)

1. Markera en eller flera typologiregler som ska kopplas till typologin och bekräfta.

   ![](assets/business-rules-typology-save.png)

1. Klicka på **[!UICONTROL Save]**.

Du kan nu tillämpa typologin på meddelanden. När du är klar kommer alla markerade typologiregler att köras för att utföra de definierade kontrollerna.

## Tillämpa typologier på meddelanden {#message}

Om du vill använda en typologi i en meddelande- eller meddelandemall måste du välja en typologi i meddelandeinställningarna. [Lär dig hur du konfigurerar leveransinställningar](../advanced-settings/delivery-settings.md#typology)

![](assets/business-rules-apply.png)

När du är klar utförs de typologiregler som ingår i typologin för att kontrollera leveransens giltighet under meddelandeförberedelsen. Profiler som matchar kriterier inom en typologiregel exkluderas sedan från leveransgrupperna.
