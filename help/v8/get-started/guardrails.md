---
title: Garantier och begränsningar i gränssnittet för Campaign Web
description: Garantier och begränsningar i gränssnittet för Campaign Web
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 4b50a20f2ba60017b97d49df8b3d84c44c15ea8c
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Skyddsritningar och begränsningar {#guardrails-limitations}

När du arbetar i gränssnittet för Campaign-webben med arbetsflöden som skapats eller ändrats i klientkonsolen för Campaign gäller de skyddsmekanismer och begränsningar som anges nedan.

Observera att även om den här sidan identifierar viktiga aspekter när du arbetar med arbetsflöden i konsolen och i webbanvändargränssnittet så omfattar den inte alla möjliga inkompatibiliteter mellan de två gränssnitten.

## Arbetsflödesaktiviteter {#wkf-activities}

Arbetsflödesaktiviteter som ännu inte stöds i Campaign Web är skrivskyddade och visas som inkompatibla aktiviteter. Du kan fortfarande köra arbetsflödet, skicka meddelanden, kontrollera loggarna osv. Arbetsflödesaktiviteter som är tillgängliga både i Campaign Web och i klientkonsolen går att redigera.

Arbetsflödesaktiviteter som ännu inte stöds i gränssnittet för Campaign-webben är skrivskyddade och visas som inkompatibla aktiviteter. Du kan fortfarande köra arbetsflödet, skicka meddelanden, kontrollera loggarna osv. Arbetsflödesaktiviteter som är tillgängliga både i gränssnittet för Campaign-webben och i klientkonsolen för Campaign kan redigeras.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

När en **Fråga** eller en **Berikning** -aktiviteten har konfigurerats med ytterligare data i konsolen. Anrikningsdata beaktas i Campaign Web och skickas till den utgående övergången, men kan inte redigeras.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

I konsolen **Berikning** kan utföra både avstämning och anrikning. Om du har definierat avstämningsinställningarna i klientkonsolen i **Berikning** aktivitet, visas som en **Avstämning** i Campaign Web-användargränssnittet.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){width="800px" align="left" zoomable="yes"} |

## Arbetsyta {#wkf-canvas}

När du skapar ett nytt arbetsflöde i gränssnittet för Campaign-webben har arbetsytan bara stöd för en startpunkt. Men om du skapade ett arbetsflöde i konsolen med flera startpunkter kan du öppna och redigera det i Campaign Web-gränssnittet.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

Nodernas placering uppdateras varje gång en aktivitet läggs till eller tas bort. Om du skapar ett arbetsflöde i konsolen, ändrar det med hjälp av användargränssnittet i Campaign-webben och öppnar det igen i konsolen, kan du märka att det finns mindre brister i positioneringen. Detta påverkar inte arbetsflödets processer och uppgifter.

| Inledande arbetsflöde | Positioneringsändring |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |
