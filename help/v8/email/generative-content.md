---
audience: end-user
title: Generativt innehåll
description: Kom igång med AI Assistant
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 1%

---

# E-postgenerering med AI Assistant {#generative-content}

>[!IMPORTANT]
>
>Innan du börjar använda den här funktionen bör du läsa de relaterade [Guardsändningarna och begränsningarna](generative-gs.md#generative-guardrails).
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

När du har skapat och anpassat dina e-postmeddelanden kan du använda AI Assistant på Adobe Campaign Web för att förbättra innehållet.

AI Assistant på Adobe Campaign Web hjälper dig att optimera effekten av dina leveranser genom att generera hela e-postmeddelanden, riktat textinnehåll och bilder som är skräddarsydda för att passa er målgrupp. Detta förbättrar era e-postkampanjer för bättre engagemang.

Använd AI Assistant för att generera fullständig e-post, text eller bilder med era e-postkampanjer. Gå igenom flikarna nedan och lär dig hur du använder AI Assistant på Adobe Campaign Web.

>[!BEGINTABS]

>[!TAB Fullständig e-postgenerering]

I följande exempel kan du använda AI Assistant på Adobe Campaign Web för att förfina ett befintligt e-postmeddelande och anpassa det för en speciell händelse.

1. När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din e-postleverans finns på [den här sidan](../email/create-email-content.md).

1. Anpassa layouten efter behov och öppna menyn **[!UICONTROL AI Assistant]**.

   ![Skärmbild med AI Assistant-menyn i Adobe Campaign Web](assets/full-email-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser.

   ![Skärmbild som visar frågebiblioteket i Adobe Campaign Web](assets/full-email-2.png){zoomable="yes"}

1. Växla **[!UICONTROL Subject line]** eller **[!UICONTROL Preheader]** för att inkludera dem i variantgenereringen.

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Se till att tonen i din e-postadress får genklang hos din publik. Vare sig du vill ljuda informativt, lekfullt eller övertygande anpassar AI Assistant budskapet därefter.

   ![Skärmbild med alternativ för textinställningar i Adobe Campaign Web](assets/full-email-3.png){zoomable="yes"}

1. Välj din **[!UICONTROL Image settings]**:

   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare utseende, medan en högre inställning (10) gör bilden mer levande.
   * **[!UICONTROL Color & tone]**: Justera det övergripande utseendet på färgerna och stämningen eller atmosfären som förmedlas.
   * **[!UICONTROL Lighting]**: Ändra ljussättningen i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

   ![Skärmbild med bildinställningsalternativ i Adobe Campaign Web](assets/full-email-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Rephrase]**: AI Assistant omformulerar ditt meddelande på olika sätt, vilket håller skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild med förfiningsalternativ i Adobe Campaign Web](assets/full-email-5.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![Skärmbild som visar knappen för att simulera innehåll i Adobe Campaign Web](assets/full-email-6.png){zoomable="yes"}

När ni definierar innehåll, målgrupp och tidsplan ska ni förbereda er för e-postleverans. [Läs mer](../monitor/prepare-send.md)

>[!TAB Generering av endast text]

I följande exempel använder du AI Assistant för att förbättra innehållet i din e-postinbjudan till ett kommande evenemang.

1. När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din e-postleverans finns på [den här sidan](../email/create-email-content.md).

1. Välj en **[!UICONTROL Text component]** för att ange specifikt innehåll som mål och öppna menyn **[!UICONTROL AI Assistant]**.

   ![Skärmbild med textkomponentval i Adobe Campaign Web](assets/text-genai-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser.

   ![Skärmbild med promptbibliotek i Adobe Campaign Web](assets/text-genai-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Se till att tonen i din e-postadress får genklang hos din publik. Vare sig du vill ljuda informativt, lekfullt eller övertygande anpassar AI Assistant budskapet därefter.
   * **Textlängd**: Använd reglaget för att välja önskad längd på texten.

   ![Skärmbild med alternativ för textinställningar i Adobe Campaign Web](assets/text-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Elaborate]**: Expandera specifika ämnen och ge ytterligare information för bättre förståelse och engagemang.
   * **[!UICONTROL Summarize]**: Förenkla viktiga punkter i tydliga, kortfattade sammanfattningar för att få uppmärksamhet och uppmuntra till ytterligare läsning.
   * **[!UICONTROL Rephrase]**: Gör om ditt meddelande på olika sätt så att det håller skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild med förfiningsalternativ i Adobe Campaign Web](assets/text-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

När ni definierar innehåll, målgrupp och tidsplan ska ni förbereda er för e-postleverans. [Läs mer](../monitor/prepare-send.md)

>[!TAB Bildgenerering]

I exemplet nedan kan du lära dig hur du använder AI Assistant för att optimera och förbättra dina resurser, vilket ger en mer användarvänlig upplevelse.

1. När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din e-postleverans finns på [den här sidan](../email/create-email-content.md).

1. Fyll i **[!UICONTROL Basic details]** för leveransen. Klicka på **[!UICONTROL Edit email content]** när du är klar.

1. Markera den resurs som du vill ändra med AI Assistant.

1. Välj **[!UICONTROL AI Assistant]** på den högra menyn.

   ![Skärmbild med AI Assistant-menyn för bildgenerering i Adobe Campaign Web](assets/image-genai-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Reference style]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser.

   ![Skärmbild som visar ett promptbibliotek för bildgenerering i Adobe Campaign Web](assets/image-genai-2.png){zoomable="yes"}

1. Skräddarsy din fråga med alternativet **[!UICONTROL Image settings]**:

   * **[!UICONTROL Aspect ratio]**: Bestäm resursens bredd och höjd. Välj bland vanliga proportioner som 16:9, 4:3, 3:2 eller 1:1, eller ange en anpassad storlek.
   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare utseende, medan en högre inställning (10) gör bilden mer levande.
   * **[!UICONTROL Color & tone]**: Justera det övergripande utseendet på färgerna och stämningen eller atmosfären som förmedlas.
   * **[!UICONTROL Lighting]**: Ändra ljussättningen i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

   ![Skärmbild med bildinställningsalternativ i Adobe Campaign Web](assets/image-genai-3.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. När du är nöjd med promptkonfigurationen klickar du på **[!UICONTROL Generate]**.

1. Bläddra i **[!UICONTROL Variation suggestions]** för att hitta den önskade resursen.

   Klicka på **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

   ![Skärmbild som visar variantförslag för bildgenerering i Adobe Campaign Web](assets/image-genai-5.png){zoomable="yes"}

1. Välj **[!UICONTROL Generate Similar]** om du vill visa relaterade bilder till den här varianten.

   ![Skärmbild som visar ett liknande alternativ i Adobe Campaign Web](assets/image-genai-6.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. När du har definierat meddelandeinnehållet klickar du på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

1. När ni definierar innehåll, målgrupp och tidsplan ska ni förbereda er för e-postleverans. [Läs mer](../monitor/prepare-send.md)

>[!ENDTABS]

## Instruktionsvideo {#video}

Lär dig hur du använder AI Assistant för att generera fullständigt e-postinnehåll, text och bilder.

>[!VIDEO](https://video.tv.adobe.com/v/3428984)