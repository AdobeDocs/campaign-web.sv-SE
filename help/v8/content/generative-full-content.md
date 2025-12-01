---
audience: end-user
title: Generativt innehåll
description: Lär dig generera kompletta innehållsupplevelser med AI Assistant i Journey Optimizer.
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 1%

---

# Generera allt innehåll med AI Assistant {#generative-full-content}

>[!IMPORTANT]
>
>Innan du börjar använda den här funktionen bör du läsa de relaterade [Guardsändningarna och begränsningarna](generative-gs.md#generative-guardrails).
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

Använd AI Assistant på Adobe Campaign Web för att generera kompletta innehållsupplevelser i alla era e-postkanaler, landningssidor och push-meddelandekanaler. AI Assistant hjälper er att optimera effekten av era leveranser genom att skapa omfattande innehåll som får genklang hos er målgrupp.

## För e-post och landningssida {#email-web-channels}

AI Assistant kan producera kompletta innehållsupplevelser för e-postleveranser och landningssidor och både generera text och bilder. Denna robusta funktionalitet hjälper er att skapa övertygande varumärkesanpassat innehåll som kan kopplas till er målgrupp via alla digitala kontaktytor.

### Åtkomst och konfiguration {#access-configure}

Innan du börjar skapa innehåll med AI Assistant måste du konfigurera leveransen och öppna innehållsredigeraren. Följ stegen nedan för att förbereda arbetsytan och öppna AI Assistant-panelen.

1. Skapa och konfigurera leverans:

   * **E-post**: När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**. [Läs mer](../email/create-email-content.md)
   * **Landningssida**: När du har skapat och konfigurerat landningssidan klickar du på **[!UICONTROL Edit content]**. [Läs mer](../landing-pages/create-lp.md)

1. Anpassa layouten efter behov och öppna menyn **[!UICONTROL AI Assistant]**.

   ![AI Assistant-panelen visar varumärkesval och frågefält](assets/full-email-1.png){zoomable="yes"}

### Generera innehåll {#generate-content}

Med AI Assistant öppen kan du nu konfigurera genereringsinställningarna för att skapa innehåll som matchar ert varumärke och era kampanjmål. Anpassa text- och bildparametrar, lägg till varumärkesresurser och ge tips om hur AI kan generera relevanta variationer för er målgrupp.

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Välj din **[!UICONTROL Brand]** för att se till att det AI-genererade innehållet följer varumärkesspecifikationerna. [Läs mer](brands.md) om varumärken.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser. [Läs mer om god praxis](ai-assistant-prompting-guide.md)

   ![Skärmbild som visar frågebiblioteket i Adobe Campaign Web](assets/full-email-2.png){zoomable="yes"}

1. **För e-postmeddelanden** kan du växla mellan alternativen **[!UICONTROL Subject line]** och **[!UICONTROL Preheader]** för att inkludera dem i variantgenereringen.

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Se till att tonen i din e-postadress får genklang hos din publik. Vare sig du vill ljuda informativt, lekfullt eller övertygande anpassar AI Assistant budskapet därefter.

     ![Skärmbild med alternativ för textinställningar i Adobe Campaign Web](assets/full-email-4.png){zoomable="yes"}

1. Välj din **[!UICONTROL Image settings]**:

   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare utseende, medan en högre inställning (10) gör bilden mer levande.
   * **[!UICONTROL Color & tone]**: Justera det övergripande utseendet på färgerna och stämningen eller atmosfären som förmedlas.
   * **[!UICONTROL Lighting]**: Ändra ljussättningen i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

1. Klicka på **[!UICONTROL Reference content]** på menyn **[!UICONTROL Upload file]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext-AI Assistant eller välja en tidigare överförd.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded reference content]**. Du behöver bara växla mellan de resurser du vill ha med i din generation.

   ![Skärmbild med alternativ för varumärkesinställningar i Adobe Campaign Web](assets/full-email-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

### Förfina och slutför {#refine-finalize}

När du har genererat innehållsvariationer kan du finjustera resultatet för att säkerställa att det uppfyller dina exakta krav. Granska varumärkesjusteringen, justera ton och språk och förbered innehållet för aktivering i leveransen.

1. Bläddra igenom **[!UICONTROL Variations]** efter generering.

1. Klicka på procentikonen för att visa din **[!UICONTROL Brand Alignment Score]** och identifiera eventuella feljusteringar av ditt varumärke.

   Läs mer om [varumärkesjusteringspoäng](brands-score.md).

   ![](assets/full-email-7.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den markerade varianten eller på **[!UICONTROL Apply]** om du vill ersätta det aktuella innehållet.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Rephrase]**: Skriv om meddelandet med bibehållen betydelse. Med det här alternativet kan du generera alternativa ordalydelser, förbättra flödet eller justera fraser utan att ändra huvudbudskapet.

   * **[!UICONTROL Use simpler language]**: Använd AI Assistant för att förenkla ditt språk och säkerställa tydlighet och tillgänglighet för en större publik.

   * **[!UICONTROL Translate]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   * **[!UICONTROL Change tone]**: Justera tonen i meddelandet så att det bättre matchar din kommunikationsstil, dvs. gör det mer användarvänligt, professionellt, brådskande eller inspirerande.

   * **[!UICONTROL Change Communication strategy]**: Ändra meddelandetillvägagångssättet baserat på dina mål, till exempel skapa en tränglighet eller framhäva en spännande tilltalande upplevelse.

   ![Förfina meny med visningsalternativ](assets/full-email-5.png){zoomable="yes"}

1. Öppna fliken **[!UICONTROL Brand Alignment]** och se hur ditt innehåll överensstämmer med [varumärkesriktlinjerna](brands.md).

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa innehållet baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

1. Granska och aktivera ditt innehåll:
   * **E-post**: När du har definierat ditt innehåll, din målgrupp och ditt schema är du redo att förbereda din e-postkampanj. [Läs mer](../monitor/prepare-send.md)
   * **Landningssida**: När landningssidan är klar kan du publicera den och göra den tillgänglig för användning i ett meddelande. [Läs mer](../landing-pages/create-lp.md)

## För mobila kanaler {#mobile-channels}

AI Assistant har även stöd för innehållsgenerering för mobila push-meddelanden, vilket gör att du kan skapa engagerande titlar, meddelanden och bilder för dina mobilappar. På så sätt kan ni upprätthålla en enhetlig och högkvalitativ kommunikation över alla kundkontaktytor, inklusive mobiler.

### Åtkomst och konfiguration {#mobile-access-configure}

Om du vill använda AI Assistant för push-meddelanden måste du först konfigurera din push-leverans och öppna innehållsredigeraren. Stegen nedan vägleder dig genom att förbereda leveransen och använda AI Assistant-verktygen.

1. När du har skapat och konfigurerat leveransen av push-meddelanden klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din push-leverans finns på [den här sidan](../push/create-push.md).

1. Anpassa push-meddelanden efter behov. [Läs mer](../push/content-push.md)

1. Öppna menyn **[!UICONTROL Show AI Assistant]**.

   ![Skärmbild som visar menyn Visa AI-assistenten](assets/push-genai-1.png){zoomable="yes"}

### Generera innehåll {#mobile-generate-content}

När du har använt AI Assistant för push-meddelanden kan du konfigurera genereringsinställningarna för att skapa övertygande mobilt innehåll. Definiera text- och bildinställningar, välj varumärkesresurser och använd uppmaningar för att generera varianter av push-meddelanden som engagerar mobilanvändarna.

1. Välj din **[!UICONTROL Brand]** för att se till att det AI-genererade innehållet följer varumärkesspecifikationerna. [Läs mer](brands.md) om varumärken.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du vill ha hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra leveransen. [Läs mer om god praxis](ai-assistant-prompting-guide.md)

   ![AI-assistenten med snabbfält och alternativ](assets/push-genai-2.png){zoomable="yes"}

1. Välj vilket fält du vill generera: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]**, **[!UICONTROL Message]** och/eller **[!UICONTROL Image]**.

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Languages]**: Välj språk för det genererade innehållet.
   * **[!UICONTROL Tone]**: Tonen på dina push-meddelanden ska matcha din publik. Vare sig du vill låta informativ, lekfull eller övertygande kan AI Assistant anpassa budskapet därefter.

     ![Panelen Textinställningar för push-meddelanden](assets/push-genai-3.png){zoomable="yes"}

1. Välj din **[!UICONTROL Image settings]**:

   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare och mer begränsat utseende, medan en högre inställning (10) gör bilden mer levande och visuellt kraftfull.
   * **[!UICONTROL Lighting]**: Justera ljuset i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

     ![Bildinställningar för push-meddelanden](assets/push-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Reference content]** på menyn **[!UICONTROL Upload file]** om du vill lägga till en varumärkesresurs som innehåller innehåll som kan ge ytterligare kontext-AI Assistant eller välja en tidigare överförd.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded reference content]**. Du behöver bara växla mellan de resurser du vill ha med i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

### Förfina och slutför {#mobile-refine-finalize}

När du har granskat dina genererade varianter av push-meddelanden kan du finjustera innehållet så att det blir perfekt. Använd finjusteringsverktygen för att justera språk och ton, verifiera varumärkesanpassningen och anpassa innehållet innan ni aktiverar er push-kampanj.

1. Bläddra igenom den genererade **[!UICONTROL Variations]**.

1. Klicka på procentikonen för att visa din **[!UICONTROL Brand Alignment Score]** och identifiera eventuella feljusteringar av ditt varumärke.

   Läs mer om [varumärkesjusteringspoäng](brands-score.md).

   ![Genererade variationer för push-meddelanden med poäng för varumärkesjustering](assets/push-genai-6.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den markerade varianten eller klicka på **[!UICONTROL Apply]** om du vill ersätta det aktuella innehållet.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Använd den valda varianten som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Rephrase]**: Rätta till ditt meddelande på olika sätt för att hålla skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.
   * **[!UICONTROL Translate]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.
Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Förfina alternativ för push-meddelanden](assets/push-genai-5.png){zoomable="yes"}

1. Öppna fliken **[!UICONTROL Brand Alignment]** och se hur ditt innehåll överensstämmer med [varumärkesriktlinjerna](brands.md).

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

När ni definierar innehåll, målgrupp och tidsplan förbereder ni er push-leverans. [Läs mer](../monitor/prepare-send.md)

## Instruktionsvideo {#video}

Lär dig hur du använder AI Assistant för att generera fullständigt e-postinnehåll, text och bilder.

>[!VIDEO](https://video.tv.adobe.com/v/3428984)