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

Varningsvillkoren är tillgängliga på menyn **Leveransvarning** i den vänstra navigeringsrutan, på fliken **Villkor**.

![](assets/alerting-criteria-list.png)

## Fördefinierade aviseringskriterier {#ootb-criteria}

Fördefinierade varningsvillkor är tillgängliga i Campaign Web User Interface. Dessa kriterier omfattar en rad olika scenarier som anges nedan:

* **Leveranser misslyckades**: Alla leveranser som har schemalagts inom ett definierat intervall, med en felaktig status.
* **Leveranser med förberedelse misslyckades**: Alla leveranser som har ändrats inom ett definierat intervall, för vilka förberedelsesteget (målberäkning och innehållsgenerering) har misslyckats.
* **Leverans med felaktig felkvot för mjuka studsar**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Pågår minst, med ett felförhållande för mjuka studsar som är större än en definierad procentandel.
* **Leverans med felaktig felkvot för hårda studsar**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Pågår minst, med ett felförhållande för hårda studsar som är större än en definierad procentandel.
* **Leveranser med lång inledande väntande**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Påbörja väntande längre än en definierad varaktighet, startar väntande status, vilket innebär att meddelanden inte har beaktats av systemet än.
* **Leveranser med lågt dataflöde**: Alla leveranser påbörjades under längre tid än en definierad varaktighet, med mindre än en definierad procentandel av bearbetade meddelanden, med ett dataflöde som är lägre än ett definierat värde.
* **Pågående leveranser**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Pågår.

>[!NOTE]
>
>Standardvärden används för alla parametrar för ovanstående villkor. Dessa värden kan anpassas i avsnittet **Villkorsparametrar** i kontrollpanelerna för leveransaviseringar där de används. [Lär dig arbeta med instrumentpaneler](../msg/delivery-alerting-dashboards.md)

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
>abstract="Ange **aviseringstypen** för villkoret, vilket innebär etiketten och färgen som ska visas bredvid leveransvillkoret i avsnittet Sammanfattning i aviseringarna."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Villkorsfrekvens"
>abstract="Kontrollera hur ofta varningar om dagen ska göras för varje leverans som uppfyller kriteriet."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Skapa ett varningsvillkor"
>abstract="Om du vill skapa egna leveransfilter skapar du ett nytt fördefinierat filter i Campaign v8-konsolen från noden **Administration** > **Konfiguration** > **Fördefinierade filter** ."

Så här skapar du ett nytt villkor:

1. Navigera till menyn **Leveransvillkor** i den vänstra navigeringsrutan och välj fliken **Villkor** .
1. Klicka på knappen **Skapa leveransvillkor**.
1. Ange en etikett för kriteriet. Det interna namnet fylls i automatiskt och är skrivskyddat.
1. Med **leveransfiltret som används av det här villkoret** kan du förfina villkorets omfång genom att använda ett fördefinierat filter på det.

   I exemplet nedan har filtret **Leveranser som bearbetas (critInProgressDeliflows)** valts, vilket innebär att villkoret endast tar hänsyn till leveranser med statusen &quot;Pågår&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Om inget av de fördefinierade filtren passar dina behov kan du kontakta administratören för att skapa ett eget filter.  Detaljerad information om hur du skapar fördefinierade filter i Campaign-konsolen finns i [Adobe Campaign v8-dokumentationen (konsolen)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Den här åtgärden får endast utföras av avancerade användare.

1. I avsnittet **Indikatorer som ska läggas till i aviseringar** väljer du de indikatorer som ska visas som kolumner i avsnittet Detaljer i e-postaviseringarna.

1. Ange **aviseringstypen** för villkoret, vilket innebär etiketten och färgen som ska visas bredvid leveransvillkoret i avsnittet Sammanfattning i aviseringarna.

1. I avsnittet **Villkorsfrekvens** kan du styra hur ofta varningar per dag ska visas för varje leverans som uppfyller villkoret:

   * **Det här leveransvillkoret upprepas i alla meddelanden**: Visa en leverans som uppfyller villkoret i varje e-postavisering på dagen.
   * **Det här leveransvillkoret skickas endast första gången dagen**: Visa en leverans som uppfyller villkoret i den första rapporten på dagen, inte upprepat i efterföljande e-postaviseringar.
