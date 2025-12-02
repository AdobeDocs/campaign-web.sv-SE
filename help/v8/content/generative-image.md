---
audience: end-user
title: Generativt innehåll
description: Lär dig hur du genererar bilder med AI Assistant
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 2%

---

# Generera bilder med AI Assistant {#generative-image}

>[!IMPORTANT]
>
>Innan du börjar använda den här funktionen bör du läsa de relaterade [Guardsändningarna och begränsningarna](generative-gs.md#generative-guardrails).
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

Använd AI Assistant på Adobe Campaign Web för att skapa övertygande visuellt material som förbättrar budskapen i e-post, landningssidor och push-meddelanden. Med AI Assistant kan du generera och optimera bilder och säkerställa att innehållet är visuellt engagerande och anpassat till ert varumärke.

## För e-post- och landningssidor {#email-web-channels}

AI Assistant kan generera kompletta visuella upplevelser för e-postleveranser och landningssidor. Tack vare den här funktionen kan ni producera varumärkesanpassade och spännande bilder som får er att lyfta fram era målgrupper över alla digitala kontaktytor.

### Åtkomst och konfiguration {#access-configure}

Om du vill börja generera bilder med AI Assistant skapar du först leveransen och öppnar innehållsredigeraren. Följ stegen nedan för att förbereda arbetsytan och öppna AI Assistant-panelen.

1. Skapa och konfigurera leverans:

   * **E-post**: När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**. [Läs mer](../email/create-email-content.md)
   * **Landningssida**: När du har skapat och konfigurerat landningssidan klickar du på **[!UICONTROL Edit content]**. [Läs mer](../landing-pages/create-lp.md)

1. Markera den resurs som du vill ändra med AI Assistant och gå till menyn **[!UICONTROL AI Assistant]**.

   ![Skärmbild med textkomponentval i Adobe Campaign Web](assets/image-genai-1.png){zoomable="yes"}

### Generera innehåll {#generate-content}

1. Aktivera alternativet **[!UICONTROL Reference style]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Välj din **[!UICONTROL Brand]** för att se till att det AI-genererade innehållet följer varumärkesspecifikationerna. [Läs mer](brands.md) om varumärken.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser. [Läs mer om god praxis](ai-assistant-prompting-guide.md)

   ![Skärmbild som visar ett promptbibliotek för bildgenerering i Adobe Campaign Web](assets/image-genai-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Image settings]**:

   * **[!UICONTROL Aspect ratio]**: Bestäm resursens bredd och höjd. Välj bland vanliga proportioner som 16:9, 4:3, 3:2 eller 1:1, eller ange en anpassad storlek.
   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare utseende, medan en högre inställning (10) gör bilden mer levande.
   * **[!UICONTROL Color & tone]**: Justera det övergripande utseendet på färgerna och stämningen eller atmosfären som förmedlas.
   * **[!UICONTROL Lighting]**: Ändra ljussättningen i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

     ![Skärmbild med bildinställningsalternativ i Adobe Campaign Web](assets/image-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Reference content]** på menyn **[!UICONTROL Upload file]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext-AI Assistant eller välja en tidigare överförd.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded reference content]**. Du behöver bara växla mellan de resurser du vill ha med i din generation.

1. När du är nöjd med promptkonfigurationen klickar du på **[!UICONTROL Generate]**.

### Förfina och slutför {#refine-finalize}

När du har genererat bildvariationer kan du granska resultatet, kontrollera varumärkesjusteringen och välja det bästa alternativet för ditt innehåll.

1. Bläddra igenom den genererade **[!UICONTROL Variations]**.

1. Klicka på procentikonen för att visa din **[!UICONTROL Brand Alignment Score]** och identifiera eventuella feljusteringar av ditt varumärke.

   Läs mer om [varumärkesjusteringspoäng](../content/brands-score.md).

   ![](assets/image-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den markerade varianten eller på **[!UICONTROL Apply]** om du vill ersätta det aktuella innehållet.

1. Välj **[!UICONTROL Generate Similar]** om du vill visa relaterade bilder till den här varianten.

1. Öppna fliken **[!UICONTROL Brand Alignment]** och se hur ditt innehåll överensstämmer med [varumärkesriktlinjerna](../content/brands.md).

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. När du har definierat meddelandeinnehållet klickar du på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

1. Granska och aktivera ditt innehåll:
   * **E-post**: När du har definierat ditt innehåll, din målgrupp och ditt schema är du redo att förbereda din e-postleverans. [Läs mer](../monitor/prepare-send.md)
   * **Landningssida**: När landningssidan är klar kan du publicera den och göra den tillgänglig för användning i ett meddelande. [Läs mer](../landing-pages/create-lp.md)

## För mobila kanaler {#mobile-channels}

Med AI Assistant kan du generera engagerande bilder för push-meddelanden, vilket hjälper dig att skapa visuellt övertygande mobilkommunikation som fångar uppmärksamheten och får genklang hos publiken.

### Åtkomst och konfiguration {#mobile-access-configure}

Om du vill börja generera bilder för push-meddelanden med AI Assistant skapar du först leveransen och öppnar AI-assistenten.

1. När du har skapat och konfigurerat leveransen av push-meddelanden klickar du på **[!UICONTROL Edit content]**. [Läs mer](../push/create-push.md)

1. Öppna menyn **[!UICONTROL Show AI Assistant]**.

   ![Skärmbild som visar menyn Visa AI-assistenten](assets/push-img-1.png){zoomable="yes"}

### Generera innehåll {#mobile-generate-content}

När du har använt AI Assistant kan du justera genereringsinställningarna för att skapa bilder som är anpassade efter ditt varumärke och stöder dina mål.

1. Välj din **[!UICONTROL Brand]** för att se till att det AI-genererade innehållet följer varumärkesspecifikationerna. [Läs mer](brands.md) om varumärken.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du vill ha hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina kampanjer. [Läs mer om god praxis](ai-assistant-prompting-guide.md)

   ![AI-assistenten med snabbfält och alternativ](assets/push-img-2.png){zoomable="yes"}

1. Välj **[!UICONTROL Image]** om du bara vill generera resurser.

1. Välj din **[!UICONTROL Image settings]**:

   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare och mer begränsat utseende, medan en högre inställning (10) gör bilden mer levande och visuellt kraftfull.
   * **[!UICONTROL Lighting]**: Justera ljuset i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

     ![Skärmbild med alternativ för bildinställningar](assets/push-img-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Reference content]** på menyn **[!UICONTROL Upload file]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext-AI Assistant eller välja en tidigare överförd.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded reference content]**. Du behöver bara växla mellan de resurser du vill ha med i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

### Förfina och slutför {#mobile-refine-finalize}

När du har genererat bildvariationer för dina mobilmeddelanden kan du finjustera resultatet för att säkerställa att de uppfyller dina exakta krav.

1. Bläddra igenom **[!UICONTROL Variations]** efter generering.

1. Klicka på procentikonen för att visa din **[!UICONTROL Brand Alignment Score]** och identifiera eventuella feljusteringar av ditt varumärke.

   Läs mer om [varumärkesjusteringspoäng](../content/brands-score.md).

   ![](assets/push-img-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Preview]** för att bläddra igenom **[!UICONTROL Variations]**.

1. Öppna fliken **[!UICONTROL Brand Alignment]** och se hur ditt innehåll överensstämmer med [varumärkesriktlinjerna](brands.md).

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

När ni har definierat ert innehåll, er målgrupp och ert schema kan ni färdigställa er push-leverans. [Läs mer](../monitor/prepare-send.md)
