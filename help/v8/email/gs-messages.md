---
audience: end-user
title: Kom igång med meddelanden och leveranser på Campaign v8 Web
description: Lär dig hur du arbetar med leveranser och skickar meddelanden med Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: c5a0103cc630e3ec44747211977988145cb75a25
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 1%

---

# Kom igång med meddelanden på Campaign Web {#gs-messages}

Med Adobe Campaign kan ni skicka flerkanalskampanjer, inklusive e-post, SMS och push-meddelanden, och mäta hur effektiva de är med hjälp av olika dedikerade rapporter. Dessa meddelanden är utformade och skickas genom leveranser och kan anpassas för varje mottagare. Dessa leveranser kan vara fristående eller ingå i en marknadsföringskampanj.

Adobe Campaign v8 har följande leveranskanaler:

* **E-postkanal**: Med e-postleveranser kan du skicka personaliserade e-postmeddelanden till målpopulationen. Lär dig hur du skapar och skickar e-postmeddelanden i [den här sidan](../email/create-email.md).

* **SMS-kanal**: leveranser i mobilkanaler gör att du kan skicka personaliserat SMS till målpopulationen.  Lär dig hur du skapar och skickar SMS i [den här sidan](../sms/create-sms.md).

* **Mobil programkanal**: mobilappsleveranser gör att du kan skicka meddelanden till iOS- och Android-system.  Lär dig hur du skapar och skickar push-meddelanden i [den här sidan](../push/gs-push.md).

## Skapa en leverans {#create-delivery}

Du kan skapa fristående leveranser från **[!UICONTROL Deliveries]** vänster meny, eller skapa leveranser i samband med en marknadsföringskampanj, från **[!UICONTROL Campaigns]** vänster meny.

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
1. När meddelandena har skickats bläddrar du till **Rapporter** för att komma åt nyckeltal. Läs mer om leveransrapporter i [det här avsnittet](../reporting/reports.md).

>[!TAB Skapa en leverans i en kampanj]

Så här skapar du en leverans i en kampanj:

1. Skapa en kampanj eller öppna en befintlig kampanj. Läs mer om [marknadsföringskampanjer](../campaigns/gs-campaigns.md).
1. Skapa ett arbetsflöde eller öppna ett befintligt arbetsflöde.
1. Lägg till och konfigurera en **[!UICONTROL Build audience]** och klicka på `+`-knappen.

   ![](assets/add-delivery-in-wf.png)

   The **[!UICONTROL Build audience]** aktiviteten anges i [det här avsnittet](../workflows/targeting-activities.md).

1. Välj en leveransaktivitet: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]** eller **[!UICONTROL Push notification (iOS)]**. Läs mer om aktiviteter i leveranskanaler i ett arbetsflöde och hur du definierar ett leveransinnehåll i det här [section](../workflows/channel-activities.md).
1. Starta arbetsflödet och kontrollera loggarna.

Du kan också lägga till leveranser i en kampanj utan att skapa ett arbetsflöde. Bläddra till **[!UICONTROL Deliveries]** fliken med kampanjen och klicka på **[!UICONTROL Create delivery]** -knappen.

![](assets/new-campaign-delivery.png)

Konfigurationsstegen är desamma som för fristående leveranser.

Mer information om hur du konfigurerar en kampanj och hanterar leveranser som tillhör en kampanj finns i [det här avsnittet](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Lägg till personalisering{#personalization}

Meddelanden från Adobe Campaign kan personaliseras på olika sätt. [Läs mer om personaliseringsfunktioner](../personalization/personalize.md).

Använd Campaign för att skapa dynamiskt innehåll och skicka personaliserade meddelanden. Personaliseringsfunktionerna kan kombineras för att förbättra budskapen och skapa en anpassad användarupplevelse.

Du kan anpassa meddelandeinnehållet genom att:

* Infoga dynamisk **personaliseringsfält**

   Anpassningsfält används för personalisering på första nivån av dina meddelanden. Du kan välja vilket fält som helst tillgängligt i databasen från personaliseringsredigeraren. För en leverans kan du välja vilket fält som helst som är relaterat till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten. [Läs mer](../personalization/personalize.md)

* Infoga fördefinierad **innehållsblock**

   Campaign innehåller en uppsättning personaliseringsblock som innehåller en specifik återgivning som du kan infoga i dina leveranser. Du kan till exempel lägga till en logotyp, ett hälsningsmeddelande eller en länk till meddelandets spegelsida. Innehållsblock är tillgängliga från ett dedikerat tävlingsbidrag via personaliseringsredigeraren. [Läs mer](../personalization/personalize.md#ootb-content-blocks)

* Skapa **villkorligt innehåll**

   Konfigurera villkorsstyrt innehåll för att lägga till dynamisk personalisering baserat på mottagarens profil till exempel. Textblock och/eller bilder infogas när ett visst villkor är true. [Läs mer](../personalization/conditions.md)

* Lägg till **personaliserade erbjudanden**

   Lägg in skräddarsydda erbjudanden i ert meddelandeinnehåll, beroende på mottagarens plats, det aktuella vädret eller den senaste inköpsordern.


## Förgranska och testa leveranserna

När meddelandeinnehållet har definierats kan du förhandsgranska det för att kontrollera återgivningen av dina meddelanden och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-test.md)


## Loggar för leverans och spårning{#gs-tracking-logs}

Att övervaka era leveranser efter att de har skickats är ett viktigt steg för att se till att era marknadsföringskampanjer är effektiva och når ut till era kunder. Du kan övervaka efter att du har skickat en leverans samt förstå hur leveransfel och karantäner hanteras.
