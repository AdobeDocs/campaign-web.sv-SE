---
audience: end-user
title: SMS med AI-assistenten i Campaign
description: Kom igång med AI-assistenten i Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 1%

---

# SMS-generering med AI-assistenten {#generative-sms}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* [Kom igång med AI-assistenten](generative-gs.md)
* [E-postgenerering med AI-assistenten](generative-content.md)
* SMS-generering med AI-assistenten
* [Generering av push-meddelanden med AI-assistenten](generative-push.md)

>[!ENDSHADEBOX]

När ni väl har utformat och personaliserat era SMS-meddelanden så att de passar er målgrupp ska ni ta er kommunikation till nästa nivå med hjälp av AI Assistant i Campaign, som bygger på innovativ AI-teknik.

Det här praktiska verktyget ger intelligenta förslag för att förfina ert innehåll och säkerställa att era meddelanden får effekt och maximerar engagemanget.

>[!NOTE]
>
>Innan du börjar använda den här funktionen bör du läsa upp relaterade [säkerhetsutkast och begränsningar](generative-gs.md#generative-guardrails).

1. När du har skapat och konfigurerat SMS-leveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din SMS-leverans finns på [den här sidan](../sms/create-sms.md).

1. Fyll i **[!UICONTROL Basic details]** för leveransen. Klicka på **[!UICONTROL Edit content]** när du är klar.

1. Anpassa SMS-meddelandet efter behov. [Läs mer](../sms/content-sms.md)

1. Öppna menyn **[!UICONTROL Show AI Assistant]**.

   ![](assets/sms-genai-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI-assistenten för att anpassa nytt innehåll baserat på din leverans, leveransnamn och vald målgrupp.

   >[!IMPORTANT]
   >
   > Din fråga måste alltid vara knuten till ditt aktuella innehåll.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du vill ha hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser.

   ![](assets/sms-genai-2.png){zoomable="yes"}

1. Välj **[!UICONTROL Upload brand asset]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext till AI-assistenten.

1. Skräddarsy uppmaningen med de olika alternativen:

   * **[!UICONTROL Communication strategy]**: Välj önskad kommunikationsmetod för den genererade texten.
   * **[!UICONTROL Language]**: Välj språk för variantens innehåll.
   * **[!UICONTROL Tone]**: Se till att texten passar din målgrupp och ditt syfte.
   * **[!UICONTROL Length]**: Välj längden på ditt innehåll med intervallreglaget.

   ![](assets/sms-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner och finjustera variationerna efter dina inställningar:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.

   * **[!UICONTROL Use simpler language]**: AI-assistenten hjälper dig att skriva tydliga, koncisa meddelanden som alla kan förstå.

   * **[!UICONTROL Rephrase]**: AI-assistenten omformulerar ditt meddelande för att hålla saker och ting engagerande för olika målgrupper.

   ![](assets/sms-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt SMS-innehåll baserat på profildata. [Läs mer om innehållspersonalisering](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable="yes"}

1. När du har definierat meddelandeinnehållet klickar du på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollerar personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable="yes"}

När du har definierat innehåll, målgrupp och schema är du redo att förbereda din SMS-leverans. [Läs mer](../monitor/prepare-send.md)
