---
audience: end-user
title: Leveransavisering
description: Lär dig arbeta med leveransaviseringar.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Kriterier för leveransavisering {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Kontrollpanel för leveransvarningsvillkor"
>abstract="Campaign Web User Interface innehåller fördefinierade varningsvillkor (leveranser med låg genomströmning, leveranser vars förberedelse misslyckades ...) som du kan lägga till på din instrumentpanel. Du kan också skapa egna kriterier som passar dina behov."

Campaign Web User Interface innehåller fördefinierade varningsvillkor (leveranser med låg genomströmning, leveranser vars förberedelse misslyckades ...) som du kan lägga till på din instrumentpanel. Du kan också skapa egna kriterier som passar dina behov.

Varningsvillkoren är tillgängliga på menyn **Leveransvarning** i den vänstra navigeringsrutan, på fliken **Villkor**.

![](assets/alerting-criteria-list.png)

## Fördefinierade aviseringskriterier {#ootb-criteria}

Fördefinierade varningsvillkor är tillgängliga i Campaign Web User Interface. Dessa kriterier omfattar en rad scenarier, som anges nedan:

* **Leveranser misslyckades**: En leverans har schemalagts inom ett angivet intervall med en felaktig status.
* **Leveranser med förberedelse misslyckades**: Alla leveranser som har ändrats inom ett definierat intervall, för vilka förberedelsesteget (målberäkning och innehållsgenerering) har misslyckats.
* **Leverans med felaktig felkvot för mjuka studsar**: Alla leveranser som har schemalagts inom ett definierat intervall, med en status som minst Pågår, med en felkvot för mjuk studs som är större än en angiven procentandel.
* **Leverans med felaktig felkvot för hårda studsar**: Alla leveranser som har schemalagts inom ett definierat intervall, med en status som minst Pågår, med en felkvot för hård studs som är större än en angiven procentandel.
* **Leveranser med lång inledande väntande**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Påbörja väntande längre än en definierad varaktighet, startar väntande status, vilket innebär att meddelanden inte har beaktats av systemet än.
* **Leveranser med lågt dataflöde**: Alla leveranser påbörjades under längre tid än en definierad varaktighet, med mindre än en definierad procentandel av bearbetade meddelanden, med ett dataflöde som är lägre än ett definierat värde.
* **Pågående leveranser**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen Pågår.

>[!NOTE]
>
>Standardvärden används för alla parametrar för ovanstående villkor. Dessa värden kan anpassas i avsnittet **Villkorsparametrar** i kontrollpanelerna för leveransaviseringar där de används. [Lär dig arbeta med instrumentpaneler](../msg/delivery-alerting-dashboards.md)

## Skapa ett varningsvillkor {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Skapa leveransvarningskriterier"
>abstract="Förutom de fördefinierade varningskriterierna från Adobe Campaign kan du skapa egna kriterier som passar dina behov."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indikatorer som ska läggas till i aviseringar"
>abstract="Välj de indikatorer som ska visas som kolumner i avsnittet Information i e-postmeddelandena."

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

1. Gå till menyn **Leverans Àlerting** i det vänstra navigeringsfönstret och välj fliken **Kriterier**.
1. Klicka på knappen **Skapa leveransaviseringsvillkor**.
1. Ange en etikett för kriteriet. Det interna namnet fylls i automatiskt och är skrivskyddat.
1. Med **leveransfiltret som tillämpas av det här kriteriet** kan du förfina kriteriets omfattning genom att tillämpa ett fördefinierat filter på det.

   I exemplet nedan har filtret **Pågående leveranser (critInProgressDelivery)** valts, vilket innebär att kriteriet endast tar hänsyn till leveranser med statusen Pågående.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Om inget av de fördefinierade filtren passar dina behov kan du kontakta administratören för att skapa ett eget filter.  Detaljerad information om hur du skapar fördefinierade filter i Campaign-konsolen finns i [Adobe Campaign v8-dokumentationen (konsolen)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Den här åtgärden får endast utföras av avancerade användare.

1. I avsnittet **Indikatorer som ska läggas till i aviseringar** väljer du de indikatorer som ska visas som kolumner i avsnittet Detaljer i e-postaviseringarna.

1. Ange **aviseringstypen** för villkoret, vilket innebär etiketten och färgen som ska visas bredvid leveransvillkoret i avsnittet Sammanfattning i aviseringarna.

1. I avsnittet **Villkorsfrekvens** kan du styra hur ofta varningar per dag ska visas för varje leverans som uppfyller villkoret:

   * **Detta leveranskriterium kommer att upprepas i varje meddelande**: Visa en leverans som uppfyller kriteriet i varje e-postavisering under dagen.
   * **Det här leveranskriteriet skickas endast den första förekomsten av dagen**: Visa en leverans som uppfyller kriteriet endast i dagens första rapport, inte upprepat i efterföljande e-postaviseringar.
