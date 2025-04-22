---
audience: end-user
title: SMS med AI Assistant
description: Kom igång med AI Assistant
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 2%

---

# SMS-generering med AI Assistant {#generative-sms}

>[!IMPORTANT]
>
>Innan du börjar använda den här funktionen bör du läsa de relaterade [Guardsändningarna och begränsningarna](generative-gs.md#generative-guardrails).
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

När ni utformar och personaliserar era SMS-meddelanden så att de passar er målgrupp kan ni kommunicera med AI Assistant på Adobe Campaign Web, som bygger på innovativ AI-teknik.

Det här verktyget ger intelligenta förslag för att förfina ert innehåll och säkerställa att era meddelanden får effekt och maximerar engagemanget.

>[!BEGINTABS]

>[!TAB Fullständig SMS-generering]

1. När du har skapat och konfigurerat SMS-leveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din SMS-leverans finns på [den här sidan](../sms/create-sms.md).

1. Fyll i **[!UICONTROL Basic details]** för leveransen. Klicka på **[!UICONTROL Edit content]** när du är klar.

1. Öppna menyn **[!UICONTROL Show AI Assistant]**.

   ![Skärmbild som visar menyn Visa AI-assistenten](assets/sms-genai-1.png){zoomable="yes"}

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser.

   ![Skärmbild som visar frågebiblioteket](assets/sms-genai-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Se till att tonen i din e-postadress får genklang hos din publik. Vare sig du vill ljuda informativt, lekfullt eller övertygande anpassar AI Assistant budskapet därefter.
   * **Textlängd**: Använd reglaget för att välja önskad längd på texten.

   ![Skärmbild med alternativ för textinställningar](assets/sms-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som innehåller innehåll som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

   ![Skärmbild som visar genererade variationer](assets/sms-genai-4.png){zoomable="yes"}

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner och finjustera variationerna efter dina inställningar:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Use simpler language]**: AI Assistant hjälper dig att skriva tydliga, koncisa meddelanden som alla kan förstå.
   * **[!UICONTROL Rephrase]**: AI Assistant formulerar om ditt meddelande så att det alltid är engagerande för olika målgrupper.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild med förfiningsalternativ](assets/sms-genai-5.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt SMS-innehåll baserat på profildata. [Läs mer om innehållspersonalisering](../personalization/personalize.md).

   ![Skärmbild med anpassningsfält](assets/sms-genai-5.png){zoomable="yes"}

1. När du har definierat meddelandeinnehållet klickar du på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md).

   ![Skärmbild med innehållssimulering](assets/sms-genai-6.png){zoomable="yes"}

När ni definierar ert innehåll, er målgrupp och er tidsplan ska ni förbereda er för SMS-leverans. [Läs mer](../monitor/prepare-send.md).

>[!TAB Generering av endast text]

1. När du har skapat och konfigurerat SMS-leveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din SMS-leverans finns på [den här sidan](../sms/create-sms.md).

1. Fyll i **[!UICONTROL Basic details]** för leveransen. Klicka på **[!UICONTROL Edit content]** när du är klar.

1. Anpassa SMS-meddelandet efter behov. [Läs mer](../sms/content-sms.md).

1. Gå till menyn **[!UICONTROL AI Assistant]** bredvid fältet **[!UICONTROL Message]**.

   ![Skärmbild med AI Assistant-menyn](assets/sms-text-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use reference content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina kampanjer.

   ![Skärmbild med frågebiblioteket](assets/sms-text-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj önskad kommunikationsmetod för den genererade texten.
   * **[!UICONTROL Language]**: Välj språk för variantens innehåll.
   * **[!UICONTROL Tone]**: Se till att texten är lämplig för din målgrupp och ditt syfte.
   * **[!UICONTROL Length]**: Välj längden på ditt innehåll med intervallreglaget.

   ![Skärmbild med alternativ för textinställningar](assets/sms-text-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som innehåller innehåll som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner och finjustera variationerna efter dina inställningar:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Rephrase]**: AI Assistant kan omformulera ditt meddelande på olika sätt, vilket håller skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Använd AI Assistant för att förenkla ditt språk och säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild med förfiningsalternativ](assets/sms-text-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt SMS-innehåll baserat på profildata. [Läs mer om innehållspersonalisering](../personalization/personalize.md).

1. När du har definierat meddelandeinnehållet klickar du på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md).

   ![Skärmbild med innehållssimulering](assets/sms-text-5.png){zoomable="yes"}

När ni definierar ert innehåll, er målgrupp och er tidsplan ska ni förbereda er för SMS-leverans. [Läs mer](../monitor/prepare-send.md).

>[!ENDTABS]