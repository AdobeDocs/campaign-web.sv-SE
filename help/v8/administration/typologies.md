---
audience: end-user
title: Arbeta med affärsregler (typologier)
description: Lär dig hur du arbetar med typologier och typologiregler för att styra, filtrera och övervaka hur leveranser skickas.
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '1402'
ht-degree: 0%

---

# Arbeta med affärsregler (typologier) {#typologies}

>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Typologiregler och typologiregler"
>abstract="Typologier gör att ni kan standardisera affärspraxis för alla leveranser. En typologi är en samling typologiregler som gör att du kan kontrollera, filtrera och prioritera skickandet av leveranser. Profiler som matchar kriterier inom en typologiregel exkluderas från leveransgrupperna under förberedelsefasen."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_type"
>title="Filtrering"
>abstract=" Det finns två typer av typologiregler: <br/><br/>**Kontroll**-regler som säkerställer meddelandekvalitet och giltighet före sändning, till exempel teckenvisning, SMS-längd, adressformat eller URL-förkortning. <br/><br/>**Filtrera** regler som exkluderar segment för målgruppen baserat på specifika kriterier som ålder, plats, land eller telefonnummer."

## Om typologier

Typologier gör att ni kan standardisera affärspraxis för alla leveranser. En **typologi** är en samling **typologiregler** som gör att du kan kontrollera, filtrera och prioritera sändning av leveranser. Profiler som matchar kriterier inom en typologiregel exkluderas från leveransgrupperna under förberedelsefasen.

Typologier ser till att dina leveranser alltid innehåller vissa element, t.ex. en länk för att avbryta prenumerationen eller en ämnesrad, eller filtreringsregler som utesluter grupper från det avsedda målet, t.ex. prenumeranter, konkurrenter eller icke-lojalitetskunder.

Typologier är tillgängliga via menyn **[!UICONTROL Administration]** > **[!UICONTROL Business rules]**. Från den här skärmen får du tillgång till alla befintliga typologier och typologiregler, eller skapa nya baserat på dina behov.

![Lista över affärsregler i gränssnittet](assets/business-rules-list.png)

>[!NOTE]
>
>Listan **[!UICONTROL Typology rules]** visar alla befintliga regler som har skapats hittills i webbanvändargränssnittet eller klientkonsolen. Endast **Kontroll** - och **Filtrering**-regler kan skapas i webbanvändargränssnittet. Om du vill skapa andra typer av typologiregler, till exempel tryck- eller kapacitetsregler, använder du klientkonsolen Campaign v8. [Lär dig skapa typologiregler i klientkonsolen](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

De viktigaste stegen för att tillämpa typologier i meddelanden är följande:

1. [Skapa en typologi](#typology).
1. [Skapa typologiregler](#typology-rule).
1. [Referera till typologiregler i typologin](#add-rules).
1. [Använd typologin för ett meddelande](#message).

## Skapa en typologi {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Typologiegenskaper"
>abstract="Definiera typologiens egenskaper och expandera avsnittet **[!UICONTROL Additional options]** för att få åtkomst till avancerade inställningar. Använd fältet **[!UICONTROL IP affinity]** för att associera IP-tillhörigheter med typologier. På så sätt kan du bättre kontrollera utgående SMTP-trafik genom att definiera vilka specifika IP-adresser som kan användas för varje tillhörighet."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="IP-tillhörighet"
>abstract="Genom att hantera tillhörigheter med IP-adresser får du bättre kontroll över utgående SMTP-trafik genom att koppla olika IP-adresser till varje typ av trafik beroende på vilken typ av leveransåtgärd det är fråga om."

Så här skapar du en typologi:

1. Gå till menyn **[!UICONTROL Business rules]** och välj fliken **[!UICONTROL Typology]**.

1. Klicka på knappen **[!UICONTROL Create typology]** och ange **[!UICONTROL Label]** som typologi.

1. Expandera avsnittet **[!UICONTROL Additional options]** om du vill definiera avancerade inställningar, till exempel typologiens interna namn, lagringsmapp och beskrivning.

   ![Gränssnitt för att skapa typologi](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >I fältet **[!UICONTROL IP affinity]** kan du associera IP-tillhörigheter med typologier. Detta ger bättre kontroll över utgående SMTP-trafik genom att definiera vilka specifika IP-adresser som kan användas för varje tillhörighet. Du kan till exempel använda en affinitet per land eller underdomän. Du kan sedan skapa en typologi per land och länka varje tillhörighet till motsvarande typologi.

1. Klicka på **[!UICONTROL Create]** för att bekräfta att typologin har skapats.

Typologiinformationen är öppen. Från den här skärmen kan du direkt referera till befintliga typologiregler eller skapa nya typologiregler som du kan referera till senare:
* [Lär dig skapa en typologiregel](#add-rules)
* [Lär dig referera till regler i en typologi](#add-rules)

## Skapa en typologiregel {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Egenskaper för typologiregel"
>abstract="Definiera typologiregelns egenskaper. **Kontroll**-regler verifierar meddelandekvalitet och giltighet före sändning, medan **Filtrering**-regler exkluderar segment för målgruppen baserat på specifika kriterier.<br/><br/>Du kan också ändra regelns körningsordning för att hantera sekvensen i vilken typologiregler körs när flera regler av samma typ körs under samma meddelandebearbetningsfas."

Det finns två typer av typologiregler:

* **Kontroll**: Garanterar meddelandekvalitet och giltighet före sändning, t.ex. teckenvisning, SMS-längd, adressformat eller URL-förkortning. Dessa regler skapas med ett skriptgränssnitt som definierar komplex logik för innehållskontroller och ändringar.

* **Filtrering**: Utesluter segment för målgruppen baserat på specifika kriterier som ålder, plats, land eller telefonnummer. Dessa regler är kopplade till en målinriktningsdimension.

>[!NOTE]
>
>För närvarande går det bara att skapa typologireglerna **Kontroll** och **Filtering** från webbanvändargränssnittet. Om du vill skapa andra typer av regler använder du Klientkonsolen. [Lär dig skapa typologiregler i klientkonsolen](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

Så här skapar du en typologiregel:

1. Gå till menyn **[!UICONTROL Business rules]** och välj fliken **[!UICONTROL Typology rules]**.

1. Klicka på knappen **[!UICONTROL Create typology rule]** och följ sedan stegen som beskrivs nedan.

   ![Skapa typologiregel](assets/business-rules-create-typo.png)

### Definiera regelns huvudegenskaper {#properties}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtrering"
>abstract="**Filtreringsreglerna** exkluderar segment för målgruppen baserat på specifika kriterier som ålder, plats, land eller telefonnummer. Markera typologiregelns måldimension och klicka på knappen **[!UICONTROL Add rules]** för att få åtkomst till frågemodelleraren och skapa regeln."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Code"
>abstract="**Kontroll**-regler verifierar meddelandets kvalitet och giltighet innan det skickas, t.ex. teckenvisning, SMS-längd, adressformat eller URL-förkortning. Dessa regler skapas med JavaScript-kod."

Det här är de viktigaste egenskaperna som du kan definiera när du skapar en ny typologiregel:

>[!BEGINTABS]

>[!TAB Kontrollregler]

1. Ange **[!UICONTROL Label]** som regel.

   ![Skapa kontrollregel](assets/business-rules-create-typo1.png)

1. I avsnittet **[!UICONTROL Additional options]** kan du komma åt avancerade inställningar, till exempel regelns interna namn, mapplagring och beskrivning. Du kan också ange när regeln ska användas och dess varningsnivå. Expandera avsnitten nedan om du vill ha mer information.

   +++Faser

   Ange vid vilken tidpunkt i leveranscykeln regeln ska tillämpas. Välj värdet i listrutan **[!UICONTROL Phase]**:

   * **[!UICONTROL At the start of targeting]**: Förhindra att personaliseringssteget körs om fel uppstår.

   * **[!UICONTROL After targeting]**: Välj den här fasen om du behöver känna till målvolymen för att kunna använda kontrollregeln. Kontrollregeln **[!UICONTROL Check proof size]** gäller till exempel efter varje målfas. Den här regeln förhindrar meddelandepersonalisering om det finns för många korrekturmottagare.

   * **[!UICONTROL At the start of personalization]**: Välj den här fasen om kontrollen gäller godkännande av meddelandeanpassning. Anpassning av meddelanden utförs under analysfasen.

   * **[!UICONTROL At the end of the analysis]**: Tillämpa kontroller som kräver fullständig meddelandepersonalisering.

   +++

   +++Nivå

   Ange aviseringsnivån för regeln:

   * **[!UICONTROL Error]**: Stoppa meddelandeförberedelsen

   * **[!UICONTROL Warning]**: Visa en varning i förberedelseloggarna

   * **[!UICONTROL Info]**: Visningsinformation i förberedelseloggarna

   * **[!UICONTROL Verbose]**: Visningsinformation i serverloggarna

   +++

1. Om du vill skapa regelns innehåll klickar du på knappen **Redigera kod** och anger logiken för regeln med JavaScript. I exemplet nedan skapas en regel som visar en varning i loggarna om målet är tomt.

   ![Kontrollregelkodredigerare](assets/business-rules-code.png)

1. Klicka på **Skapa**.


>[!TAB Filtreringsregler]

1. Ange **[!UICONTROL Label]** som regel.

   ![Skapa filtreringsregel](assets/business-rules-create-typo2.png)

1. Expandera avsnittet **[!UICONTROL Additional options]** om du vill komma åt avancerade inställningar, till exempel regelns interna namn, mapplagring och beskrivning.

1. Om du vill skapa regelns innehåll markerar du måldimensionen och klickar på knappen **[!UICONTROL Add rules]** för att definiera filtervillkor med [regelbyggaren](../query/query-modeler-overview.md).

   ![Frågemodelleraren för filtreringsregel](assets/business-rules-query.png)

1. Klicka på **Skapa**

>[!ENDTABS]

### Definiera regelns ytterligare egenskaper {#add-properties}

Nu ska vi definiera de ytterligare parametrarna. På den här skärmen kan du fortfarande ändra de huvudegenskaper som tidigare definierats.

![Skapa ytterligare filtreringsregel](assets/business-rules-create-typo3.png)

1. Växla av alternativet **[!UICONTROL Active]** om du inte vill att regeln ska vara aktiv direkt efter att den har skapats.

1. Definiera regelns **[!UICONTROL Execution order]**.

   Som standard är typologiregelordningen inställd på 50. Anpassa det här värdet för att hantera den sekvens i vilken typologiregler ska köras när flera regler av samma typ körs under samma meddelandebearbetningsfas. En filtreringsregel med körningsordningen 20 körs till exempel före en filtreringsregel med körningsordningen 30.

1. Välj en **[!UICONTROL Channel]** som ska associeras med regeln.

Regeln är klar att refereras i en typologi för att den ska kunna tillämpas på meddelanden.

## Referera till typologiregler i en typologi {#add-rules}

Följ de här stegen för att referera till en eller flera regler i en typologi:

1. Navigera till fliken **[!UICONTROL Typology]** och öppna den typologi där du vill referera till reglerna.

1. Välj fliken **[!UICONTROL Typology rules]** och klicka på knappen **[!UICONTROL Add rules)]**.

   ![Lägg till gränssnitt för typologiregler](assets/business-rules-reference.png)

1. Välj en eller flera typologiregler som ska kopplas till typologin och bekräfta.

   ![Spara typologiregelgränssnitt](assets/business-rules-typology-save.png)

1. Klicka på **[!UICONTROL Save]**.

Du kan nu tillämpa typologin på meddelanden. När du är klar kommer alla markerade typologiregler att köras för att utföra de definierade kontrollerna.

## Tillämpa typologier på meddelanden {#message}

Om du vill tillämpa en typologi på en meddelande- eller meddelandemall väljer du typologin i meddelandeinställningarna. [Lär dig hur du konfigurerar leveransinställningar](../advanced-settings/delivery-settings.md#typology)

![Använd typologi i meddelandegränssnittet](assets/business-rules-apply.png)

När typologireglerna som ingår i typologin har tillämpats körs de för att kontrollera leveransens giltighet under meddelandeförberedelsen. Profiler som matchar villkor inom en typologiregel exkluderas från leveransgrupperna.