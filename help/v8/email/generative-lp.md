---
audience: end-user
title: Landningssida med AI Assistant
description: Kom igång med AI Assistant
exl-id: f4baa23f-f289-4837-b5b3-c479eaeff86c
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '1362'
ht-degree: 1%

---

# Skapa landningssidor med AI Assistant{#generative-lp}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Generera landningssidor med AI"
>abstract="Nu kan du använda AI Assistant för att skapa leveranser av landningssidor, så att du kan generera text, bilder eller hela sidlayouter."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"

>[!IMPORTANT]
>
>Läs de relaterade [Guardscheman och Begränsningar](generative-gs.md#generative-guardrails) innan du börjar använda den här funktionen.
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

Omvandla landningssidorna med AI Assistant på Adobe Campaign Web, som bygger på generativ AI.

Skapa enkelt slagkraftigt innehåll, inklusive kompletta sidor, skräddarsydda textbitar och skräddarsydda bilder som passar er målgrupp, vilket ökar engagemanget och interaktionen.

Gå igenom flikarna nedan och lär dig hur du använder AI Assistant på Adobe Campaign Web.

>[!BEGINTABS]

>[!TAB Generering av hela landningssidor]

I följande exempel får du lära dig hur du använder AI Assistant för att förfina en befintlig landningssidmall.

1. När du har skapat och konfigurerat landningssidan klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din landningssida finns på [den här sidan](../landing-pages/create-lp.md).

1. Anpassa layouten efter behov och öppna menyn **[!UICONTROL AI Assistant]**.

   ![Skärmbild med AI Assistant-menyn i landningssidans redigerare.](assets/lp_full_gen_1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra din landningssida.

   ![Skärmbild som visar gränssnittet Prompt Library.](assets/lp_full_gen_2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Tonen på din landningssida ska tolkas som målgruppen. Vare sig du vill låta informativ, lekfull eller övertygande kan AI Assistant anpassa budskapet därefter.

   ![Skärmbild med alternativ för textinställningar.](assets/lp_full_gen_3.png){zoomable="yes"}

1. Välj din **[!UICONTROL Image settings]**:

   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare utseende, medan en högre inställning (10) gör bilden mer levande.
   * **[!UICONTROL Color & tone]**: Justera det övergripande utseendet på färgerna i en bild och stämningen eller atmosfären som den förmedlar.
   * **[!UICONTROL Lighting]**: Ändra ljuset i en bild för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna element inom en bilds bildruta.

   ![Skärmbild med alternativ för bildinställningar.](assets/lp_full_gen_4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

   ![Skärmbild som visar menyn varumärkesresurser.](assets/lp_full_gen_5.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Rephrase]**: AI Assistant kan omformulera ditt meddelande på olika sätt, vilket håller skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild som visar förfiningsalternativen.](assets/lp_full_gen_6.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa innehållet på landningssidan baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../landing-pages/create-lp.md#test-landing-page).

När landningssidan är klar publicerar du den så att den blir tillgänglig för användning i ett meddelande. [Läs mer](../landing-pages/create-lp.md#publish-landing-page).

>[!TAB Generering av endast text]

I följande exempel får du lära dig hur du använder AI Assistant för att förbättra innehållet på din landningssida.

1. När du har skapat och konfigurerat landningssidan klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din landningssida finns på [den här sidan](../landing-pages/create-lp.md).

1. Välj en **[!UICONTROL Text component]** för att ange specifikt innehåll som mål och öppna menyn **[!UICONTROL AI Assistant]**.

   ![Skärmbild med AI Assistant-menyn för textkomponenter.](assets/lp-text-genai-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina landningssidor.

   ![Skärmbild som visar gränssnittet Prompt Library.](assets/lp-text-genai-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Tonen på din landningssida ska tolkas som målgruppen. Vare sig du vill låta informativ, lekfull eller övertygande kan AI Assistant anpassa budskapet därefter.
   * **Textlängd**: Använd reglaget för att välja önskad längd på texten.

   ![Skärmbild med alternativ för textinställningar.](assets/lp-text-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

   ![Skärmbild som visar menyn varumärkesresurser.](assets/lp-text-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Elaborate]**: Expandera specifika ämnen och ge ytterligare information för bättre förståelse och engagemang.
   * **[!UICONTROL Summarize]**: Komprimera lång information till tydliga, kortfattade sammanfattningar som fångar uppmärksamheten och uppmuntrar till ytterligare läsning.
   * **[!UICONTROL Rephrase]**: Gör om ditt meddelande på olika sätt så att det håller skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild som visar förfiningsalternativen.](assets/lp-text-genai-5.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa innehållet på landningssidan baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../landing-pages/create-lp.md#test-landing-page).

När landningssidan är klar publicerar du den så att den blir tillgänglig för användning i ett meddelande. [Läs mer](../landing-pages/create-lp.md#publish-landing-page).

>[!TAB Generering av endast bild]

I exemplet nedan kan du lära dig hur du använder AI Assistant för att optimera och förbättra dina resurser, vilket ger en mer användarvänlig upplevelse.

1. När du har skapat och konfigurerat landningssidan klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din landningssida finns på [den här sidan](../landing-pages/create-lp.md).

1. Markera den resurs som du vill ändra med AI Assistant.

1. Välj **[!UICONTROL AI Assistant]** på den högra menyn.

   ![Skärmbild med AI Assistant-menyn för bildkomponenter.](assets/lp-image-gen-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Reference style]** för AI Assistant för att anpassa nytt innehåll baserat på referensinnehållet. Du kan också överföra en bild för att lägga till kontext till variationen.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina landningssidor.

   ![Skärmbild som visar gränssnittet Prompt Library.](assets/lp-image-gen-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Image settings]**:

   * **[!UICONTROL Aspect ratio]**: Bestäm resursens bredd och höjd. Välj bland vanliga proportioner som 16:9, 4:3, 3:2 eller 1:1, eller ange en anpassad storlek.
   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare utseende, medan en högre inställning (10) gör bilden mer levande.
   * **[!UICONTROL Color & tone]**: Justera det övergripande utseendet på färgerna i en bild och stämningen eller atmosfären som den förmedlar.
   * **[!UICONTROL Lighting]**: Ändra ljuset i en bild för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna element inom en bilds bildruta.

   ![Skärmbild med alternativ för bildinställningar.](assets/lp-image-gen-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. När du är nöjd med promptkonfigurationen klickar du på **[!UICONTROL Generate]**.

1. Bläddra i **[!UICONTROL Variation suggestions]** för att hitta den önskade resursen.

   Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

1. Välj **[!UICONTROL Generate Similar]** om du vill visa relaterade bilder till den här varianten.

   ![Skärmbild som visar gränssnittet för variantförslag.](assets/lp-image-gen-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. När du har definierat meddelandeinnehållet klickar du på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../landing-pages/create-lp.md#test-landing-page).

När landningssidan är klar publicerar du den så att den blir tillgänglig för användning i ett meddelande. [Läs mer](../landing-pages/create-lp.md#publish-landing-page).

>[!ENDTABS]