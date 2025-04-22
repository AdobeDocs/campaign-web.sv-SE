---
audience: end-user
title: Push-meddelande med AI Assistant
description: Kom igång med AI Assistant
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 2%

---

# Generering av push-meddelanden med AI Assistant {#generative-push}

>[!IMPORTANT]
>
>Innan du börjar använda den här funktionen bör du läsa de relaterade [Guardsändningarna och begränsningarna](generative-gs.md#generative-guardrails).
></br>
>
>Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

AI Assistant hjälper er att optimera effekten av era leveranser genom att föreslå olika innehåll som får genklang hos er målgrupp.

I följande exempel används AI Assistant för att skapa övertygande meddelanden för att skapa en mer engagerande kundupplevelse.

1. När du har skapat och konfigurerat leveransen av push-meddelanden klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din push-leverans finns på [den här sidan](../push/create-push.md).

1. Öppna menyn **[!UICONTROL Show AI Assistant]**.

   ![Skärmbild som visar menyn Visa AI-assistenten](assets/push-genai-1.png){zoomable="yes"}

1. Aktivera alternativet **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på det valda innehållet.

1. Finjustera innehållet genom att beskriva vad du vill generera i fältet **[!UICONTROL Prompt]**.

   Om du behöver hjälp med att skapa din fråga kan du få tillgång till **[!UICONTROL Prompt Library]**, som innehåller en mängd olika tips för att förbättra dina leveranser.

   ![Skärmbild som visar gränssnittet för promptbiblioteket](assets/push-genai-2.png){zoomable="yes"}

1. Välj det fält som du vill generera: **[!UICONTROL Title]**, **[!UICONTROL Message]** och/eller **[!UICONTROL Image]**.

1. Skräddarsy din fråga med alternativet **[!UICONTROL Text settings]**:

   * **[!UICONTROL Communication strategy]**: Välj den lämpligaste kommunikationsstilen för den genererade texten.
   * **[!UICONTROL Tone]**: Justera tonen i e-postmeddelandet så att det får genklang hos målgruppen. Vare sig du vill ljuda informativt, lekfullt eller övertygande anpassar AI Assistant budskapet därefter.

   ![Skärmbild med alternativ för textinställningar](assets/push-genai-3.png){zoomable="yes"}

1. Välj din **[!UICONTROL Image settings]**:

   * **[!UICONTROL Content type]**: Kategorisera det visuella elementets karaktär och skilja mellan olika former av visuell representation, till exempel foton, grafik eller grafik.
   * **[!UICONTROL Visual intensity]**: Kontrollera bildens påverkan genom att justera dess intensitet. En lägre inställning (2) ger ett mjukare och mer begränsat utseende, medan en högre inställning (10) gör bilden mer levande och visuellt kraftfull.
   * **[!UICONTROL Lighting]**: Justera ljuset i bilden för att forma atmosfären och framhäva specifika element.
   * **[!UICONTROL Composition]**: Ordna elementen i bildens ram.

   ![Skärmbild med alternativ för bildinställningar](assets/push-genai-4.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Upload brand asset]** på menyn **[!UICONTROL Brand assets]** om du vill lägga till en varumärkesresurs som innehåller innehåll som ger ytterligare kontext till AI Assistant, eller välj en som har överförts tidigare.

   Tidigare överförda filer är tillgängliga i listrutan **[!UICONTROL Uploaded brand assets]**. Växla de resurser du vill inkludera i din generation.

1. Klicka på **[!UICONTROL Generate]** när din fråga är klar.

1. Bläddra igenom den genererade **[!UICONTROL Variations]** och klicka på **[!UICONTROL Preview]** för att visa en fullskärmsversion av den valda varianten.

1. Navigera till alternativet **[!UICONTROL Refine]** i fönstret **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Använd den valda varianten som referensinnehåll för att generera andra resultat.
   * **[!UICONTROL Rephrase]**: Rätta till ditt meddelande på olika sätt för att hålla skrivandet aktuellt och engagerande för olika målgrupper.
   * **[!UICONTROL Use simpler language]**: Förenkla ditt språk för att säkerställa tydlighet och tillgänglighet för en större publik.

   Du kan också ändra **[!UICONTROL Tone]** och **[!UICONTROL Communication strategy]** för texten.

   ![Skärmbild med alternativen Förfina ](assets/push-genai-5.png){zoomable="yes"}

1. Klicka på **[!UICONTROL Select]** när du har hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. Klicka sedan på knappen **[!UICONTROL Simulate content]** för att kontrollera återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![Skärmbild med knappen Simulera innehåll](assets/push-genai-6.png){zoomable="yes"}

När ni definierar innehåll, målgrupp och tidsplan förbereder ni er push-leverans. [Läs mer](../monitor/prepare-send.md)