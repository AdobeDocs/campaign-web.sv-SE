---
audience: end-user
title: SMS med AI-assistenten i Campaign
description: Kom igång med AI-assistenten i Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: 2e084aeb27b6a866bf1f3aa82ab361da3b238901
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 1%

---

# SMS-generering med AI-assistenten {#generative-sms}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* [Kom igång med AI-assistenten](generative-gs.md)
* [E-postgenerering med AI-assistenten](generative-content.md)
* **[SMS-generering med AI-assistenten](generative-sms.md)**
* [Generering av push-meddelanden med AI-assistenten](generative-push.md)

>[!ENDSHADEBOX]

När ni väl har utformat och personaliserat era SMS-meddelanden så att de passar er målgrupp ska ni ta er kommunikation till nästa nivå med hjälp av AI Assistant i Campaign, som bygger på innovativ AI-teknik.

Det här praktiska verktyget ger intelligenta förslag för att förfina ert innehåll och säkerställa att era meddelanden får effekt och maximerar engagemanget.

>[!NOTE]
>
>Innan du börjar använda den här funktionen bör du läsa upp relaterade [Gardrutor och begränsningar](generative-gs.md#guardrails-and-limitations).

1. När du har skapat och konfigurerat SMS-leveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din SMS-leverans finns i [den här sidan](../sms/create-sms.md).

1. Fyll i **[!UICONTROL Basic details]** för leverans. När du är klar klickar du **[!UICONTROL Edit content]**.

1. Anpassa SMS-meddelandet efter behov. [Läs mer](../sms/content-sms.md)

1. Öppna **[!UICONTROL Show AI Assistant]** -menyn.

   ![](assets/sms-genai-1.png){zoomable=&quot;yes&quot;}

1. Aktivera **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på leverans, leveransnamn och vald målgrupp.

   >[!IMPORTANT]
   >
   > Din fråga måste alltid vara knuten till ditt aktuella innehåll.

1. Finjustera innehållet genom att beskriva vad du vill generera i **[!UICONTROL Prompt]** fält.

   Om du behöver hjälp med att skapa din fråga kan du gå till **[!UICONTROL Prompt Library]** som ger en mängd olika tips för att förbättra leveransen.

   ![](assets/sms-genai-2.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Upload brand asset]** om du vill lägga till alla varumärkesresurser som innehåller innehåll som kan ge ytterligare kontext i AI-assistenten.

1. Skräddarsy uppmaningen med de olika alternativen:

   * **[!UICONTROL Communication strategy]**: Välj önskat kommunikationssätt för den genererade texten.
   * **[!UICONTROL Language]**: Välj språk för variantens innehåll.
   * **[!UICONTROL Tone]**: Se till att texten är lämplig för din målgrupp och ditt syfte.
   * **[!UICONTROL Length]**: Välj längden på innehållet med intervallreglaget.

   ![](assets/sms-genai-3.png){zoomable=&quot;yes&quot;}

1. När frågan är klar klickar du på **[!UICONTROL Generate]**.

1. Bläddra bland de genererade **[!UICONTROL Variations]** och klicka **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

1. Navigera till **[!UICONTROL Refine]** i **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner och finjustera dina varianter:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.

   * **[!UICONTROL Use simpler language]**: AI-assistenten hjälper dig att skriva tydliga, koncisa meddelanden som alla kan förstå.

   * **[!UICONTROL Rephrase]**: AI Assistant formulerar om ditt budskap för att hålla det engagerande för olika målgrupper.

   ![](assets/sms-genai-4.png){zoomable=&quot;yes&quot;}

1. Klicka **[!UICONTROL Select]** när du hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt SMS-innehåll baserat på profildata. [Läs mer om innehållspersonalisering](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable=&quot;yes&quot;}

1. När du har definierat meddelandeinnehållet klickar du på **[!UICONTROL Simulate content]** för att styra återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable=&quot;yes&quot;}

När du har definierat innehåll, målgrupp och schema är du redo att förbereda din SMS-leverans. [Läs mer](../monitor/prepare-send.md)
