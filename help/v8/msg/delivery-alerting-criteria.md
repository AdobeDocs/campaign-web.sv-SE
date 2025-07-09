---
audience: end-user
title: Leveransvarningar
description: Lär dig hur du arbetar med leveransvarningar.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: 037b04475370b1a34ecec31ef2a774866278ce65
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Villkor för leveransvarning {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Kontrollpanel för leveransaviseringskriterier"
>abstract="Campaign Web User Interface innehåller fördefinierade varningsvillkor (leveranser med låg genomströmning, leveranser vars förberedelse misslyckades ...) som du kan lägga till på din instrumentpanel. Du kan också skapa egna kriterier som passar dina behov."

Campaign Web User Interface innehåller fördefinierade varningsvillkor, som leveranser med låg genomströmning eller leveranser vars förberedelse misslyckades, som du kan lägga till på instrumentpanelen. Du kan också skapa egna kriterier som passar dina behov.

Varningsvillkoren är tillgängliga på menyn **Leveransvarning** i den vänstra navigeringsrutan, på fliken **Villkor**.

![Lista med varningsvillkor som visas på menyn Leveransvarning](assets/alerting-criteria-list.png)

## Fördefinierade aviseringskriterier {#ootb-criteria}

Fördefinierade varningsvillkor är tillgängliga i Campaign Web User Interface. Dessa kriterier omfattar en rad olika scenarier som anges nedan:

* **Leveranser misslyckades**: Alla leveranser som har schemalagts inom ett definierat intervall, med en felaktig status.
* **Leveranser med förberedelse misslyckades**: Alla leveranser som har ändrats inom ett definierat intervall, för vilka förberedelsesteget (målberäkning och innehållsgenerering) har misslyckats.
* **Leverans med felaktig felkvot för mjuka studsar**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen &quot;Pågår&quot; och ett felförhållande för mjuka studsar som är större än en definierad procentandel.
* **Leverans med felaktig felkvot för hårda studsar**: Alla leveranser som är schemalagda inom ett definierat intervall, med statusen &quot;Pågår&quot; och ett felförhållande för hårda studsar som är större än en definierad procentandel.
* **Leveranser med lång inledande väntande**: Alla leveranser som har schemalagts inom ett definierat intervall, med statusen Påbörja väntande längre än en definierad varaktighet. Status &quot;Starta väntande&quot; innebär att meddelanden ännu inte har beaktats av systemet.
* **Leveranser med lågt dataflöde**: Alla leveranser har startat för längre tid än en definierad varaktighet, med mindre än en definierad procentandel av bearbetade meddelanden och ett dataflöde som är lägre än ett definierat värde.
* **Pågående leveranser**: Alla leveranser som är schemalagda inom ett definierat intervall med statusen Pågår.

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

Så här skapar du ett nytt villkor:

1. Navigera till menyn **Leveransvarning** i den vänstra navigeringsrutan och välj fliken **Villkor** .
1. Klicka på knappen **Skapa leveransvillkor**.
1. Ange en etikett för kriteriet. Det interna namnet fylls i automatiskt och är skrivskyddat.
1. Använd **Leveransfiltret som används av det här villkoret** för att förfina villkorets omfång genom att använda ett fördefinierat filter på det.

   I exemplet nedan har filtret **Leveranser som bearbetas (critInProgressDeliflows)** valts, vilket innebär att villkoret endast tar hänsyn till leveranser med statusen &quot;Pågår&quot;.

   ![Exempel på egenskaper för varningsvillkor med det valda filtret](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Om inget av de fördefinierade filtren passar dina behov kan du skapa egna filter på menyn **Kundhantering** > **Fördefinierade filter** . [Läs mer](../get-started/predefined-filters.md)
   >
   >Den här åtgärden får endast utföras av avancerade användare.

1. I avsnittet **Indikatorer som ska läggas till i aviseringar** väljer du de indikatorer som ska visas som kolumner i avsnittet Detaljer i e-postaviseringarna.

1. Ange **aviseringstypen** för villkoret, vilket innebär etiketten och färgen som ska visas bredvid leveransvillkoret i avsnittet Sammanfattning i aviseringarna.

1. Använd avsnittet **Villkorsfrekvens** om du vill kontrollera frekvensen för aviseringar per dag för varje leverans som uppfyller villkoret:

   * **Det här leveransvillkoret upprepas i alla meddelanden**: Visa en leverans som uppfyller villkoret i varje e-postavisering på dagen.
   * **Det här leveransvillkoret skickas endast den första förekomsten av dagen**: Visa en leverans som uppfyller villkoret i den första rapporten på dagen, utan att upprepa det i efterföljande e-postaviseringar.