---
title: Garantier och begränsningar i arbetsflödena för gränssnittet i Campaign Web
description: Garantier och begränsningar när du arbetar med arbetsflöden i användargränssnittet för Campaign Web
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Garantier och begränsningar för arbetsflöden {#guardrails-limitations}

När du arbetar i gränssnittet för Campaign-webben med arbetsflöden som skapats eller ändrats i klientkonsolen för Campaign gäller de skyddsmekanismer och begränsningar som anges nedan.

Observera att även om den här sidan identifierar viktiga aspekter när du arbetar med arbetsflöden i konsolen och i webbanvändargränssnittet så omfattar den inte alla möjliga inkompatibiliteter mellan de två gränssnitten.

## Arbetsflödesaktiviteter {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Aktiviteten är inte redigerbar"
>abstract="När en **fråga** eller en **berikning**-aktivitet har konfigurerats med ytterligare data i konsolen, beaktas data för berikning på Campaign-webben och skickas till den utgående övergången, men kan inte redigeras."

Arbetsflödesaktiviteter som ännu inte stöds i gränssnittet för Campaign-webben är skrivskyddade och visas som inkompatibla aktiviteter. Du kan fortfarande köra arbetsflödet, skicka meddelanden, kontrollera loggarna osv. Arbetsflödesaktiviteter som är tillgängliga både i gränssnittet för Campaign-webben och i klientkonsolen för Campaign kan redigeras.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

När en **fråga** eller en **berikning**-aktivitet har konfigurerats med ytterligare data i konsolen, beaktas data för berikning på Campaign-webben och skickas till den utgående övergången, men kan inte redigeras.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

I konsolen kan aktiviteten **Enrichment** utföra både avstämning och anrikning. Om du har definierat avstämningsinställningar i aktiviteten **Enrichment** i klientkonsolen visas den som en **avstämningsaktivitet** i webbgränssnittet för Campaign.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Arbetsyta {#wkf-canvas}

När du skapar ett nytt arbetsflöde i gränssnittet för Campaign-webben har arbetsytan bara stöd för en startpunkt. Men om du skapade ett arbetsflöde i konsolen med flera startpunkter kan du öppna och redigera det i Campaign Web-gränssnittet.

| Konsol | Webb |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Nodernas placering uppdateras varje gång en aktivitet läggs till eller tas bort. Om du skapar ett arbetsflöde i konsolen, ändrar det med hjälp av användargränssnittet i Campaign-webben och öppnar det igen i konsolen, kan du märka att det finns mindre brister i positioneringen. Detta påverkar inte arbetsflödets processer och uppgifter.

| Inledande arbetsflöde | Positioneringsändring |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |
