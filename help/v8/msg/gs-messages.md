---
audience: end-user
title: Kom igång med meddelanden och leveranser på Campaign v8 Web
description: Lär dig hur du arbetar med leveranser och skickar meddelanden med Campaign Web
badge: label="Beta"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 2%

---

# Kom igång med meddelanden{#gs-messages}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Leveranser"
>abstract="En leverans är en marknadsföringskommunikation som skickas till en viss målgrupp via en viss kanal: e-post, SMS eller push-meddelanden. I listan över leveranser kan du redigera befintliga leveranser och kontrollera status, kontakt- och ändringsdatum samt KPI:er. Klicka på knappen Skapa leverans för att lägga till en ny leverans. Välj en leverans för att visa dess innehåll, schema, målgrupp och detaljer."


Med Adobe Campaign kan ni skicka flerkanalskampanjer, inklusive e-post, SMS och push-meddelanden, och mäta hur effektiva de är med hjälp av olika dedikerade rapporter.

Dessa meddelanden är utformade och skickas genom leveranser och kan anpassas för varje mottagare. Dessa leveranser kan vara fristående eller ingå i en marknadsföringskampanj.

Adobe Campaign v8 har följande leveranskanaler: e-post, SMS och mobilappar.

<table style="table-layout:fixed">
    <tr style="border: 0;">
    <td>
    <a href="../email/create-email.md">
    <img alt="E-post" src="assets/do-not-localize/email.jpg">
    </a>
    <div><a href="../email/create-email.md"><strong>Skapa e-postmeddelanden</strong>
    </div>
    <p>
    </td>
    <td>
    <a href="../push/create-push.md">
      <img alt="Push" src="assets/do-not-localize/push.jpg">
    </a>
    <div>
    <a href="../push/gs-push.md"><strong>Skapa push-meddelanden</strong></a>
    </div>
    <p>
    </td>
    <td>
    <a href="../sms/create-sms.md">
      <img alt="SMS" src="assets/do-not-localize/sms.jpg">
    </a>
    <div>
    <a href="../sms/create-sms.md"><strong>Skapa SMS-meddelanden</strong></a>
    </div>
    <p>
    </td>
    </tr>
    </table>


## Skapa en leverans {#create-delivery}


Du kan skapa fristående leveranser från **[!UICONTROL Deliveries]** vänster meny eller skapa leveranser i samband med en marknadsföringskampanj från **[!UICONTROL Campaigns]** vänster meny.

Bläddra bland flikarna nedan för att lära dig hur du skapar en leverans:

>[!BEGINTABS]

>[!TAB Skapa en fristående leverans]

Så här skapar du en fristående leverans:

1. Gå till **[!UICONTROL Deliveries]** till vänster och klicka på **[!UICONTROL Create delivery]** -knappen.

   ![](assets/create-a-delivery.png)

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
1. När meddelandena har skickats går du till **Rapporter** för att komma åt nyckeltal. Läs mer om leveransrapporter i [det här avsnittet](../reporting/delivery-reports.md).

>[!TAB Skapa en leverans i en kampanj]

Så här skapar du en leverans i en kampanj:

1. Skapa en kampanj eller öppna en befintlig kampanj. Läs mer om [marknadsföringskampanjer](../campaigns/gs-campaigns.md).
1. Skapa ett arbetsflöde eller öppna ett befintligt.
1. Lägg till och konfigurera en **[!UICONTROL Build audience]** och klicka på `+`-knappen.

   ![](assets/add-delivery-in-wf.png)

   The **[!UICONTROL Build audience]** aktiviteten anges i [det här avsnittet](../workflows/activities/build-audience.md).

1. Välj en leveransaktivitet: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]** eller **[!UICONTROL Push notification (iOS)]**. Läs mer om aktiviteter i leveranskanaler i ett arbetsflöde och hur du definierar ett leveransinnehåll i det här [section](../workflows/activities/about-activities.md#channel).
1. Starta arbetsflödet och kontrollera loggarna.

Du kan också lägga till leveranser i en kampanj utan att skapa ett arbetsflöde. Bläddra till **[!UICONTROL Deliveries]** fliken med kampanjen och klicka på **[!UICONTROL Create delivery]** -knappen.

![](assets/new-campaign-delivery.png)

Konfigurationsstegen är desamma som för fristående leveranser.

Mer information om hur du konfigurerar en kampanj och hanterar leveranser som tillhör en kampanj finns i [det här avsnittet](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Lägg till personalisering{#personalization}

Meddelanden från Adobe Campaign kan personaliseras på olika sätt. [Läs mer om personaliseringsfunktioner](../personalization/gs-personalization.md).

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


## Övervaka och spåra loggar{#gs-tracking-logs}

Att övervaka era leveranser efter att de har skickats är ett viktigt steg för att se till att era marknadsföringskampanjer är effektiva och når ut till era kunder.

Du kan övervaka efter att du har skickat en leverans samt förstå hur leveransfel och karantäner hanteras.

Läs mer om övervakning och spårning i [det här avsnittet](../reporting/gs-reports.md).

## Duplicera en leverans {#delivery-duplicate}

Du kan skapa en kopia av en befintlig leverans, antingen från leveranslistan eller från kontrollpanelen för leverans.

Så här duplicerar du en leverans från listan med leveranser:

1. Klicka på knappen med tre punkter till höger bredvid namnet på den leverans som ska dupliceras.
1. Välj  **[!UICONTROL Duplicate]**.
1. Bekräfta duplicering: den nya kontrollpanelen för leverans öppnas på den centrala skärmen.

Så här duplicerar du en leverans från kontrollpanelen:

1. Öppna leveransen och klicka på  **[!UICONTROL ...More]** på skärmens övre del.
1. Välj **[!UICONTROL Duplicate]**.
1. Bekräfta duplicering: Den nya leveransen ersätter den aktuella leveransen på den centrala skärmen.

## Ta bort en leverans {#delivery-delete}

Leveranser tas bort från leveranslistan, antingen från huvudposten i det vänstra fältet eller från leveranslistan för en kampanj.

Så här tar du bort en leverans från listan över leveranser:

1. Klicka på knappen med tre punkter till höger bredvid namnet på den leverans som ska dupliceras.
1. Välj  **[!UICONTROL Delete]**.
1. Bekräfta borttagning.

![Ta bort en leverans från leveranslistan](assets/delete-delivery-from-list.png)

Alla leveranser är tillgängliga i de här listorna, men leveranser som har skapats i ett arbetsflöde kan inte tas bort därifrån. Om du vill ta bort en leverans som har skapats i ett arbetsflöde måste du ta bort leveransaktiviteten från arbetsflödet.

Så här tar du bort en leverans från ett arbetsflöde:

1. Välj leveransaktivitet.
1. Klicka på  **[!UICONTROL Delete]** på den högra panelen.
1. Bekräfta borttagning. Om leveransen har underordnade noder kan du välja att ta bort dem också eller att behålla dem.

![Ta bort en leverans i ett arbetsflöde](assets/delete-delivery-from-wf.png)
