---
audience: end-user
title: Generativt innehåll
description: Lär dig generera textinnehåll med AI Assistant
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 2%

---

# Generera text med AI Assistant {#generative-text}

>[!IMPORTANT]
>
>Innan du börjar använda den här funktionen bör du läsa de relaterade [Guardsändningarna och begränsningarna](generative-gs.md#generative-guardrails).
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

Använd AI Assistant på Adobe Campaign Web för att skapa engagerande text som får genklang hos läsarna. Vare sig du förbättrar e-postkopieringen, skapar övertygande innehåll på landningssidor, skriver push-meddelanden eller skriver SMS-text kan AI Assistant hjälpa dig att leverera tydlig och slagkraftig kommunikation.

## För e-post- och landningssidor {#email-web-channels}

AI Assistant kan generera högklassigt textinnehåll för e-postleveranser och landningssidor. Med den här funktionen kan ni skapa övertygande varumärkesanpassade meddelanden som kan kommunicera med er målgrupp över olika digitala kontaktytor.

### Åtkomst och konfiguration {#access-configure}

Innan du kan börja generera textinnehåll med AI Assistant måste du ställa in leveransen och öppna innehållsredigeraren. Följ de här stegen för att förbereda arbetsytan och öppna AI-assistentpanelen.

1. Skapa och konfigurera leverans:

   * **E-post**: När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**. [Läs mer](../email/create-email-content.md)
   * **Landningssida**: När du har skapat och konfigurerat landningssidan klickar du på **[!UICONTROL Edit content]**. [Läs mer](../landing-pages/create-lp.md)

1. Välj en **[!UICONTROL Text component]** för att ange specifikt innehåll som mål och öppna menyn **[!UICONTROL AI Assistant]**.

   ![Skärmbild med textkomponentval i Adobe Campaign Web](assets/text-genai-1.png){zoomable="yes"}

### Generera innehåll {#generate-content}

Lär dig skapa tydliga uppmaningar, finjustera inställningarna och generera skräddarsydd text med hjälp av AI Assistant, och se till att era meddelanden passar ert varumärke och era kommunikationsmål.

1. Välj din **[!UICONTROL Brand]** för att se till att det AI-genererade innehållet följer varumärkesspecifikationerna. [Läs mer](brands.md) om varumärken.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser. [Läs mer om god praxis](ai-assistant-prompting-guide.md)

   ![Skärmbild med promptbibliotek i Adobe Campaign Web](assets/text-genai-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Languages]**: Välj språk för det genererade innehållet.
   * **[!UICONTROL Tone]**: Se till att tonen i din e-postadress får genklang hos din publik. Vare sig du vill ljuda informativt, lekfullt eller övertygande anpassar AI Assistant budskapet därefter.
   * **Textlängd**: Använd reglaget för att välja önskad längd på texten.

     ![Skärmbild med alternativ för textinställningar i Adobe Campaign Web](assets/text-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Reference content]** på menyn **[!UICONTROL Upload file]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext-AI Assistant eller välja en tidigare överförd.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded reference content]**. Du behöver bara växla mellan de resurser du vill ha med i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

### Förfina och slutför {#refine-finalize}

Lär dig hur du granskar den genererade texten, gör förbättringar och tillämpar personalisering för att färdigställa innehållet och skapa snygga och engagerande meddelanden som är klara för leverans.

1. Bläddra igenom den genererade **[!UICONTROL Variations]**.

1. Klicka på procentikonen för att visa din **[!UICONTROL Brand Alignment Score]** och identifiera eventuella feljusteringar av ditt varumärke.

   Läs mer om [varumärkesjusteringspoäng](brands-score.md).

   ![](assets/text-genai-6.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den markerade varianten eller på **[!UICONTROL Apply]** om du vill ersätta det aktuella innehållet.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Elaborate]**: Expandera specifika ämnen och ge ytterligare information för bättre förståelse och engagemang.
   * **[!UICONTROL Summarize]**: Förenkla viktiga punkter i tydliga, kortfattade sammanfattningar för att få uppmärksamhet och uppmuntra till ytterligare läsning.
   * **[!UICONTROL Rephrase]**: Gör om ditt meddelande på olika sätt så att det håller skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.
   * **[!UICONTROL Translate]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild med förfiningsalternativ i Adobe Campaign Web](assets/text-genai-5.png){zoomable="yes"}

1. Öppna fliken **[!UICONTROL Brand Alignment]** och se hur ditt innehåll överensstämmer med [varumärkesriktlinjerna](../content/brands.md).

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa innehållet baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

1. Granska och aktivera ditt innehåll:
   * **E-post**: När du har definierat ditt innehåll, din målgrupp och ditt schema är du redo att förbereda din e-postleverans. [Läs mer](../monitor/prepare-send.md)
   * **Landningssida**: När landningssidan är klar kan du publicera den och göra den tillgänglig för användning i ett meddelande. [Läs mer](../landing-pages/create-lp.md)

## För mobila kanaler {#mobile-channels}

AI Assistant kan generera övertygande textinnehåll för push-meddelanden och SMS-meddelanden, vilket hjälper dig att skapa engagerande mobilkommunikation som kan kommunicera med publiken över alla mobilkontaktytor.

### Åtkomst och konfiguration {#mobile-access-configure}

Innan du börjar generera text med AI Assistant för mobila kanaler måste du konfigurera leveransen och få tillgång till AI Assistant.

1. Skapa och konfigurera din mobila leverans:
   * **Push-meddelanden**: När du har skapat och konfigurerat leveransen av push-meddelanden klickar du på **[!UICONTROL Edit content]**. [Läs mer](../push/create-push.md)
   * **SMS**: När du har skapat och konfigurerat SMS-leveransen klickar du på **[!UICONTROL Edit content]**. [Läs mer](../sms/create-sms.md)

1. Anpassa meddelandet efter behov:
   * **Push-meddelanden**: [Läs mer](../push/content-push.md)
   * **SMS**: [Läs mer](../sms/content-sms.md)

1. Öppna menyn **[!UICONTROL Show AI Assistant]**.

   ![Skärmbild som visar menyn Visa AI-assistenten](assets/sms-genai-1.png){zoomable="yes"}

### Generera innehåll {#mobile-generate-content}

När du har använt AI Assistant kan du konfigurera genereringsinställningarna för att skapa mobilt innehåll som matchar ert varumärke och era leveransmål. Anpassa textparametrar, lägg till varumärkesresurser och ge anvisningar om hur AI genererar relevanta variationer.

1. Välj din **[!UICONTROL Brand]** för att se till att det AI-genererade innehållet följer varumärkesspecifikationerna. [Läs mer](brands.md) om varumärken.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du vill ha hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra leveransen. [Läs mer om god praxis](ai-assistant-prompting-guide.md)

   ![AI-assistenten med snabbfält och alternativ](assets/sms-genai-2.png){zoomable="yes"}

1. **För push-meddelanden** väljer du textfältet som du vill generera: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]** och/eller **[!UICONTROL Message]**.

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Languages]**: Välj språk för det genererade innehållet.
   * **[!UICONTROL Tone]**: Tonen bör återges med din målgrupp. Vare sig du vill låta informativ, lekfull eller övertygande kan AI Assistant anpassa budskapet därefter.
   * **[!UICONTROL Length]**: Välj längden på ditt innehåll med intervallreglaget.

     ![Panelen Textinställningar](assets/sms-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Reference content]** på menyn **[!UICONTROL Upload file]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext-AI Assistant eller välja en tidigare överförd.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded reference content]**. Du behöver bara växla mellan de resurser du vill ha med i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

### Förfina och slutför {#mobile-refine-finalize}

När du har genererat textvarianter för dina mobilmeddelanden kan du finjustera resultatet för att säkerställa att de uppfyller dina exakta krav. Granska varumärkesjusteringen, justera ton och språk och förbered innehållet för aktivering.

1. Bläddra igenom **[!UICONTROL Variations]** efter generering.

1. Klicka på procentikonen för att visa din **[!UICONTROL Brand Alignment Score]** och identifiera eventuella feljusteringar av ditt varumärke.

   Läs mer om [varumärkesjusteringspoäng](brands-score.md).

   ![Förfina meny](assets/sms-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den markerade varianten eller klicka på **[!UICONTROL Apply]** om du vill ersätta det aktuella innehållet.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.

   * **[!UICONTROL Rephrase]**: Skriv om meddelandet med bibehållen betydelse. Med det här alternativet kan du generera alternativa ordalydelser, förbättra flödet eller justera fraser utan att ändra huvudbudskapet.

   * **[!UICONTROL Use simpler language]**: Använd AI Assistant för att förenkla ditt språk och säkerställa tydlighet och tillgänglighet för en större publik.

   * **[!UICONTROL Translate]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   * **[!UICONTROL Change tone]**: Justera tonen i meddelandet så att det bättre matchar din kommunikationsstil, dvs. gör det mer användarvänligt, professionellt, brådskande eller inspirerande.

   * **[!UICONTROL Change Communication strategy]**: Ändra meddelandetillvägagångssättet baserat på dina mål, till exempel skapa en tränglighet eller framhäva en spännande tilltalande upplevelse.

     ![Genererade textvariationer med bakgrundsjusteringspoäng](assets/sms-genai-5.png){zoomable="yes"}

1. Öppna fliken **[!UICONTROL Brand Alignment]** och se hur ditt innehåll överensstämmer med [varumärkesriktlinjerna](brands.md).

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa innehållet baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../personalization/personalize.md)

1. Granska och aktivera ditt innehåll:
   * **Push-meddelande**: När du har definierat ditt innehåll, din målgrupp och ditt schema kan du förbereda leveransen av push-meddelanden. [Läs mer](../push/send-push.md)
   * **SMS**: När ditt SMS är klart kan du publicera det så att det blir tillgängligt för användning i ett meddelande. [Läs mer](../sms/send-sms.md)
