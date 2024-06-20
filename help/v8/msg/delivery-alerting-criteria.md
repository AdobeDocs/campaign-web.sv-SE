---
audience: end-user
title: Leveransvarningar
description: Lär dig hur du arbetar med leveransvarningar.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Villkor för leveransvarning {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Kontrollpanel för leveransaviseringskriterier"
>abstract="Campaign Web User Interface innehåller fördefinierade varningsvillkor (leveranser med låg genomströmning, leveranser vars förberedelse misslyckades ...) som du kan lägga till på din instrumentpanel. Du kan också skapa egna kriterier som passar dina behov."

Campaign Web User Interface innehåller fördefinierade varningsvillkor (leveranser med låg genomströmning, leveranser vars förberedelse misslyckades ...) som du kan lägga till på din instrumentpanel. Du kan också skapa egna kriterier som passar dina behov.

Varningsvillkoren är tillgängliga från **Leveransvarning** menyn i den vänstra navigeringsrutan, under **Kriterier** -fliken.

![](assets/alerting-criteria-list.png)

## Fördefinierade aviseringskriterier {#ootb-criteria}

Fördefinierade varningsvillkor är tillgängliga i Campaign Web User Interface. Dessa kriterier omfattar en rad olika scenarier som anges nedan:

* **Misslyckade leveranser**: Alla leveranser som schemalagts inom ett definierat intervall, med en felaktig status.
* **Det gick inte att förbereda leveranser**: Alla leveranser som har ändrats inom ett definierat intervall och för vilka förberedelsesteget (målberäkning och innehållsgenerering) har misslyckats.
* **Leverans med dåligt felförhållande för mjuka studsar**: Alla leveranser som schemalagts inom ett definierat intervall, med en status som är minst Pågående, med ett felförhållande för mjukt studs som är större än en angiven procentandel.
* **Leverans med dåligt felförhållande för hårda studsar**: Alla leveranser som är schemalagda inom ett definierat intervall, med en status som är minst Pågående, med ett felförhållande som är större än ett definierat procenttal.
* **Leveranser med lång start väntar**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Påbörja väntande längre än en definierad varaktighet, Starta väntande status, vilket innebär att meddelandena inte har beaktats av systemet än.
* **Leveranser med låg genomströmning**: Alla leveranser påbörjades under längre tid än en definierad varaktighet, med mindre än en definierad procentandel av bearbetade meddelanden, med ett dataflöde som är lägre än ett definierat värde.
* **Pågående leveranser**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Pågår.

>[!NOTE]
>
>Standardvärden används för alla parametrar för ovanstående villkor. Dessa värden kan anpassas i **Kriterieparametrar** i kontrollpanelerna för leveransvarningar där de används. [Lär dig hur du arbetar med kontrollpaneler](../msg/delivery-alerting-dashboards.md)

## Skapa ett varningsvillkor {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Skapa leveransaviseringskriterier"
>abstract="Förutom de fördefinierade varningsvillkoren från Adobe Campaign kan du skapa egna kriterier som passar dina behov."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indikatorer att lägga till i aviseringar"
>abstract="Välj de indikatorer som ska visas som kolumner i avsnittet Detaljer i e-postaviseringarna."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Aviseringstyp"
>abstract="Ange **Aviseringstyp** för kriteriet, vilket innebär den etikett och färg som ska visas bredvid leveransvillkoret i avsnittet &quot;Sammanfattning&quot; i aviseringarna."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Villkorsfrekvens"
>abstract="Kontrollera hur ofta varningar om dagen ska göras för varje leverans som uppfyller kriteriet."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Skapa ett varningsvillkor"
>abstract="Om du vill skapa egna leveransfilter skapar du ett nytt fördefinierat filter i Campaign v8-konsolen från **Administration** > **Konfiguration** > **Fördefinierade filter** nod."

Så här skapar du ett nytt villkor:

1. Navigera till **Delivery Álerting** i den vänstra navigeringsrutan och väljer **Kriterier** -fliken.
1. Klicka på **Skapa leveransaviseringskriterier** -knappen.
1. Ange en etikett för kriteriet. Det interna namnet fylls i automatiskt och är skrivskyddat.
1. The **Leveransfilter som används av det här villkoret** I kan du förfina villkorets omfång genom att använda ett fördefinierat filter på det.

   I exemplet nedan är **Pågående leveranser (critInProgressDeliflows)** filtret har valts, vilket innebär att kriteriet endast tar hänsyn till leveranser med statusen &quot;Pågår&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Om inget av de fördefinierade filtren passar dina behov kan du kontakta administratören för att skapa ett eget filter.  Detaljerad information om hur du skapar fördefinierade filter i Campaign-konsolen finns i [Adobe Campaign v8-dokumentation (konsol)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Den här åtgärden får endast utföras av avancerade användare.

1. I **Indikatorer att lägga till i aviseringar** väljer du de indikatorer som ska visas som kolumner i avsnittet Detaljer i e-postaviseringarna.

1. Ange **Aviseringstyp** för kriteriet, vilket innebär den etikett och färg som ska visas bredvid leveransvillkoret i avsnittet &quot;Sammanfattning&quot; i aviseringarna.

1. The **Villkorsfrekvens** kan du styra hur ofta varningar per dag ska visas för varje leverans som uppfyller kriteriet:

   * **Detta leveransvillkor upprepas i varje meddelande**: Visa en leverans som uppfyller villkoret i varje e-postavisering på dagen.
   * **Det här leveransvillkoret skickas endast vid den första förekomsten av dagen**: Visa en leverans som uppfyller villkoret i den första rapporten på dagen, inte upprepat i efterföljande e-postaviseringar.
