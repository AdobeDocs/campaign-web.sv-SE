---
audience: end-user
title: Kom igång med meddelanden och leveranser på Campaign v8 Web
description: Lär dig hur du arbetar med leveranser och skickar meddelanden med Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Kom igång med meddelanden på Campaign Web {#gs-messages}

Med Adobe Campaign kan ni skicka flerkanalskampanjer, inklusive e-post, SMS och push-meddelanden, och mäta hur effektiva de är med hjälp av olika dedikerade rapporter. Dessa meddelanden är utformade och skickas genom leveranser och kan anpassas för varje mottagare. Dessa leveranser kan vara fristående eller ingå i en marknadsföringskampanj.

Adobe Campaign v8 har följande leveranskanaler:

* **E-postkanal**: Med e-postleveranser kan du skicka personaliserade e-postmeddelanden till målpopulationen. Lär dig hur du skapar och skickar e-postmeddelanden i [den här sidan](../email/create-email.md).

* **SMS-kanal**: leveranser i mobilkanaler gör att du kan skicka personaliserat SMS till målpopulationen.  Lär dig hur du skapar och skickar SMS i [den här sidan](../sms/create-sms.md).

* **Mobil programkanal**: mobilappsleveranser gör att du kan skicka meddelanden till iOS- och Android-system.  Lär dig hur du skapar och skickar push-meddelanden i [den här sidan](../push/gs-push.md).

## Skapa en leverans

Du kan skapa fristående leveranser från **Leverans** huvudmenyn eller skapa leveranser i samband med en marknadsföringskampanj.

>[!BEGINTABS]

>[!TAB Skapa en fristående leverans]

Så här skapar du en fristående leverans:

1. Bläddra till **[!UICONTROL Deliveries]** till vänster och klicka på **[!UICONTROL Create delivery]** -knappen.
1. Välj en kanal för leveransen. Läs mer om leveranskanaler och hur du definierar ett leveransinnehåll i dessa avsnitt:

   * [E-postkanal](../email/create-email.md)
   * [Push-meddelandekanal](../push/gs-push.md)
   * [SMS-kanal](../sms/create-sms.md)

1. Definiera målgruppen för leveransen, för huvudmålet och kontrollgruppen. Läs mer om målgrupper i [det här avsnittet](../audience/about-audiences.md).
1. Definiera meddelandeinnehållet.
1. (valfritt) Definiera leveransschema. Om inget schema är definierat skickas meddelanden direkt efter att du klickat på **[!UICONTROL Send]** -knappen.
1. Klicka på  **[!UICONTROL Review and send]** för att kontrollera inställningarna.
1. Använd  **[!UICONTROL Simulate content]** för att testa leveransinställningar och personaliseringsinställningar. Läs mer om meddelandesimulering i [det här avsnittet](../preview-test/preview-test.md).
1. Klicka på  **[!UICONTROL Prepare]** för att beräkna målpopulationen och generera meddelandena. Förberedelsesteget kan ta några minuter. När färdigställandet är klart kan meddelanden skickas. Om ett fel uppstår går du till **Loggar** för att kontrollera varningar och varningar.
1. Kontrollera resultaten och klicka på  **[!UICONTROL Send]** för att börja skicka meddelanden.
1. När meddelandena har skickats bläddrar du till avsnittet Rapporter för att få tillgång till nyckeltal. Läs mer om leveransrapporter i [det här avsnittet](../reporting/reports.md).

>[!TAB Skapa en leverans i en kampanj]

Så här skapar du en leverans i en kampanj:

1. Skapa en kampanj eller öppna en befintlig kampanj.

Mer information om hur du konfigurerar en kampanj finns i

>[!ENDTABS]


## Välj hur du vill skicka meddelanden{#gs-send-msg}

När meddelandet har skapats och dess innehåll har utformats och testats kan du välja hur du vill skicka det.

Campaign erbjuder en uppsättning funktioner för att:

* Skicka meddelanden manuellt till huvudmålet

* Skicka meddelanden som är kopplade till en [marknadsföringskampanj](../campaigns/gs-campaigns.md)

* Skicka meddelanden via [arbetsflöde](../workflows/channel-activities.md)


## Lägg till personalisering{#personalization}

Meddelanden från Adobe Campaign kan personaliseras på olika sätt


## Loggar för leverans och spårning{#gs-tracking-logs}

Att övervaka era leveranser efter att de har skickats är ett viktigt steg för att se till att era marknadsföringskampanjer är effektiva och når ut till era kunder. Du kan övervaka efter att du har skickat en leverans samt förstå hur leveransfel och karantäner hanteras.
