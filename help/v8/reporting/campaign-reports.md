---
audience: end-user
title: Kampanjrapporter
description: Lär dig hur du får tillgång till och använder kampanjrapporter
badge: label="Alpha" type="Positive"
source-git-commit: 535ab4238c9937d716a20ac8019b44da091bdd6c
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 1%

---

# Kampanjrapporter {#campaign-reports}

Campaign-rapporten är uppdelad i olika widgetar som detaljerar kampanjens framgångar och fel.

Kampanjrapportsidan visas med följande flikar:

* [E-postkanal](#email-channel)
* [SMS-kanal](#sms-channel)
* [Push-kanal](#push-channel)

Klicka på Rapporter från kampanjens kontrollpanel för att få tillgång till din Campaign-rapport.

![](assets/campaign_report_email_13.png)

## E-postkanal {#email-channel}

### Leveranssammanfattning {#delivery-summary-email}

* **[!UICONTROL Delivery Overview]** innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med e-postleveransen.

  ![](assets/campaign_report_email_1.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Total sent]**: Totalt antal meddelanden som bearbetats under leveransanalysen.

   * **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

   * **[!UICONTROL Bounces]**: Totalt antal fel som sammanställts under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

   * **[!UICONTROL Distinct opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

* **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till dina mottagare:

  ![](assets/campaign_report_email_2.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

   * **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransanalys.

   * **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress saknas, sätts i karantän, på blockeringslista osv.

+++

* **[!UICONTROL Execution statistics]** tabellen visar hur bra leveransen är.

  ![](assets/campaign_report_email_3.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransanalys.

   * **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

* **[!UICONTROL Reaction statistics]** tabellen innehåller tillgängliga data för mottagaraktivitet för leveransen.

  ![](assets/campaign_report_email_4.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Distinct opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

   * **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

   * **[!UICONTROL Unsubscriptions]**: Antal mottagare som klickat på att avbryta prenumerationen för den aktuella perioden.

   * **[!UICONTROL Mirror page]**: Antal mottagare som klickade på länken för spegelsidan.

   * **[!UICONTROL Forwards]**: Antal mottagare som klickade och som vidarebefordrade e-postmeddelandet.
+++

* **[!UICONTROL Generated click streams]** tabellen visar data som är relativa till hur mottagarna interagerade med leveransen.

  ![](assets/campaign_report_email_5.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat på en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

+++

### Ej levererbara {#non-deliverables-email}

* **[!UICONTROL Breakdown of errors per type]** och **[!UICONTROL Breakdown of errors per domain]** tabeller och diagram innehåller tillgängliga data för eventuella fel som påträffas i varje domän.

  ![](assets/campaign_report_email_6.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återbindning, i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL Contribution]**:

   * **[!UICONTROL Breakdown]**:

+++

### Spårningsindikatorer {#tracking-indicators-email}

* **[!UICONTROL Delivery statistics]** innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om data som är tillgängliga för skickade e-postmeddelanden.

  ![](assets/campaign_report_email_7.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL Distinct opens]**: Totalt antal målmottagare som öppnat ett meddelande minst en gång.

   * **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

   * **[!UICONTROL Clicks on the opt-out link]**: Antal klick på länken för att avbryta prenumerationen.

   * **[!UICONTROL Clicks on the mirror link]**: Antal klick på länken till spegelsidan.

   * **[!UICONTROL Estimation of forwards]**: Uppskattning av antalet e-postmeddelanden som vidarebefordrats av målmottagarna.
+++

* **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till mottagarna.

  ![](assets/campaign_report_email_8.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Sent]**: Totalt antal skickade meddelanden.

   * **[!UICONTROL Complaints]**: Antal meddelanden för den här domänen som har rapporterats som oönskade av mottagaren.

   * **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

   * **[!UICONTROL Clicks]**: Antal distinkta mottagare som klickat på samma leverans minst en gång.

   * **[!UICONTROL Raw reactivity]**: Procentandel av antalet mottagare som klickade på en leverans minst en gång jämfört med antalet mottagare som öppnade en leverans minst en gång.
+++

### URL:er och klickströmmar {#url-email}

* **[!UICONTROL URLs and click streams]** innehåller nyckeltal (KPI:er) som ger detaljerad information om de URL:er som du klickade mest på under en leverans.

  ![](assets/campaign_report_email_9.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat på en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

+++

* **[!UICONTROL Top 10 most visited links]** diagram och tabell innehåller tillgängliga data för mottagarnas beteende per länk.

  ![](assets/campaign_report_email_10.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Percentage]**: Procentandel användare som interagerade med leveransen.

+++

* **[!UICONTROL Breakdown of clicks over time]** diagrammet innehåller tillgängliga data för mottagarnas beteende per länk.

  ![](assets/campaign_report_email_11.png)

### Användaraktiviteter {#user-activities-email}

* **[!UICONTROL User activities]** visar hur öppningar och klickningar delas upp i ett diagram.

  ![](assets/campaign_report_email_12.png)

  +++Läs mer om rapportstatistik för e-postkampanjer.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Opens]**: Antal distinkta målmottagare för den här domänen som har öppnat ett meddelande minst en gång.

+++

## SMS-kanal {#sms-channel}

### Leveranssammanfattning {#delivery-summary-sms}

* **[!UICONTROL Delivery Overview]** innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med SMS-leveransen.

  +++Läs mer om mätvärden för SMS-kampanjrapporter.

   * **[!UICONTROL Total sent]**: Totalt antal meddelanden som bearbetats under leveransanalysen.

   * **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

   * **[!UICONTROL Errors]**: Totalt antal fel som sammanställts under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

* **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till dina mottagare:

  +++Läs mer om mätvärden för SMS-kampanjrapporter.

   * **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

   * **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransanalys.

   * **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress saknas, sätts i karantän, på blockeringslista osv.

+++

* **[!UICONTROL Execution statistics]** tabellen visar hur framgångsrik leveransen är:

  +++Läs mer om mätvärden för SMS-kampanjrapporter.

   * **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransanalys.

   * **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

* **[!UICONTROL Generated click streams]** tabellen visar data i relation till hur mottagarna interagerade med leveransen:

  +++Läs mer om mätvärden för SMS-kampanjrapporter.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat på en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

+++

## Push-kanal {#push-channel}

### Leveranssammanfattning {#delivery-summary-push}

* **[!UICONTROL Delivery Overview]** innehåller nyckeltal för nyckeltal (KPI) som ger detaljerad information om hur besökarna interagerar med leverans av push-meddelanden.

  +++Läs mer om mätvärden för push-kampanjrapporter.

   * **[!UICONTROL Total sent]**: Totalt antal meddelanden som bearbetats under leveransanalysen.

   * **[!UICONTROL Delivered]**: Antal meddelanden som har skickats, i relation till det totala antalet skickade meddelanden.

   * **[!UICONTROL Errors]**: Totalt antal fel som sammanställts under leverans och automatisk returbehandling i relation till totalt antal skickade meddelanden.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

+++

* **[!UICONTROL Initial target audience statistics]** tabellen visar data som är relativa till dina mottagare:

  +++Läs mer om mätvärden för push-kampanjrapporter.

   * **[!UICONTROL Initial audience]**: Totalt antal målmottagare.

   * **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransanalys.

   * **[!UICONTROL Rejected by rules]**: Totalt antal adresser som ignoreras under analysen när regler tillämpas: adress saknas, sätts i karantän, på blockeringslista osv.

+++

* **[!UICONTROL Execution statistics]** tabellen visar hur framgångsrik leveransen är:

  +++Läs mer om mätvärden för push-kampanjrapporter.

   * **[!UICONTROL Message to deliver]**: Totalt antal meddelanden som ska levereras efter leveransanalys.

   * **[!UICONTROL Success]**: Antal meddelanden som har bearbetats i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL Errors]**: Totalt antal fel som har ackumulerats under leveranser och automatisk återinläsning i relation till antalet meddelanden som ska levereras.

   * **[!UICONTROL New quarantines]**: Totalt antal adresser i karantän efter misslyckad leverans (okänd användare, ogiltig domän) i relation till antalet meddelanden som ska levereras.

+++

* **[!UICONTROL Generated click streams]** tabellen visar data i relation till hur mottagarna interagerade med leveransen:

  +++Läs mer om mätvärden för push-kampanjrapporter.

   * **[!UICONTROL Distinct clicks]**: Totalt antal distinkta mottagare som klickat på en leverans minst en gång.

   * **[!UICONTROL Clicks]**: Totalt antal klick på länkar i leveranser.

   * **[!UICONTROL Reactivity]**: Förhållandet mellan antalet målmottagare som klickat på en leverans, i förhållande till det uppskattade antalet målmottagare som öppnat en leverans.

+++
