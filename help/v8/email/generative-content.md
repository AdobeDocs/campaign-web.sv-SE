---
audience: end-user
title: Text med AI-assistenten
description: Kom igång med AI-assistenten i Campaign
badge: label="Beta"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: 396f52cfdb482e5afdf43b5729ef37b5a634be3d
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 1%

---

# E-postgenerering med AI-assistenten {#generative-content}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* [Kom igång med AI-assistenten](generative-gs.md)
* **[E-postgenerering med AI-assistenten](generative-content.md)**
* [SMS-generering med AI-assistenten](generative-sms.md)
* [Generering av push-meddelanden med AI-assistenten](generative-push.md)

>[!ENDSHADEBOX]

När ni väl har skapat och personaliserat era e-postmeddelanden kan ni använda Journey Optimizer AI Assistant i Campaign, som bygger på generativ AI, för att ta innehållet till nästa nivå.

AI Assistant kan hjälpa er att optimera effekten av era leveranser genom att föreslå olika typer av innehåll som troligtvis får genklang hos er målgrupp.

>[!NOTE]
>
>Innan du börjar använda den här funktionen bör du läsa upp relaterade [Gardrutor och begränsningar](generative-gs.md#guardrails-and-limitations).

## Skapa innehåll med AI Assistant {#generative-text}

1. När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din e-postleverans finns i [den här sidan](../email/create-email-content.md).

1. Fyll i **[!UICONTROL Basic details]** för leverans. När du är klar klickar du **[!UICONTROL Edit content]**.

1. Anpassa e-postmeddelandet efter behov. [Läs mer](content-components.md)

1. Öppna **[!UICONTROL AI Assistant]** -menyn.

   Du kan också välja en **[!UICONTROL Text component]** för att endast rikta in sig på ett visst innehåll.

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. Finjustera innehållet genom att beskriva vad du vill generera i **[!UICONTROL Prompt]** fält.

   Om du behöver hjälp med att skapa din fråga kan du gå till **[!UICONTROL Prompt Library]** som ger en mängd olika tips för att förbättra leveransen.

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. Växla **[!UICONTROL Subject line]** eller **[!UICONTROL Preheader]** för att inkludera dem i variantgenereringen.

1. På snabbmenyn aktiverar du **[!UICONTROL Enhance with current context]** för AI Assistant för att anpassa nytt innehåll baserat på leverans, leveransnamn och vald målgrupp.

   >[!IMPORTANT]
   >
   > Din uppmaning måste alltid vara knuten till ett specifikt sammanhang genom att överföra en varumärkesresurs eller aktivera **[!UICONTROL Enhance current content]** alternativ.

1. Klicka **[!UICONTROL Upload brand asset]** om du vill lägga till alla varumärkesresurser som innehåller innehåll som kan ge ytterligare kontext i AI-assistenten.

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Communication strategy]** som bäst passar dina behov. Detta påverkar den genererade textens ton och format.

1. Välj **[!UICONTROL Language]** och **[!UICONTROL Tone]** som du vill att den genererade texten ska ha. På så sätt säkerställs att texten passar er målgrupp och ert syfte.

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. När frågan är klar klickar du på **[!UICONTROL Generate]**.

1. Bläddra bland de genererade **[!UICONTROL Variations]** och klicka **[!UICONTROL Apply]** när du hittat rätt innehåll.

   Klicka **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. [Läs mer om innehållspersonalisering](../personalization/personalize.md)

   ![](assets/text-genai-6.png){zoomable=&quot;yes&quot;}

1. När du har definierat meddelandeinnehållet klickar du på **[!UICONTROL Simulate content]** för att styra återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

1. När ni har definierat ert innehåll, er målgrupp och ert schema är ni redo att förbereda er för att leverera e-post. [Läs mer](../monitor/prepare-send.md)

## Bildgenerering med AI-assistenten {#generative-image}

I exemplet nedan kan du lära dig hur du använder AI-assistenten för att optimera och förbättra ditt innehåll, vilket ger en mer användarvänlig upplevelse. Följ de här stegen:

1. När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din e-postleverans finns i [den här sidan](../email/create-email-content.md).

1. Fyll i **[!UICONTROL Basic details]** för leverans. När du är klar klickar du **[!UICONTROL Edit email content]**.

1. Markera den resurs som du vill ändra med AI-assistenten.

1. Välj **[!UICONTROL AI Assistant]**.

   ![](assets/image-genai-1.png){zoomable=&quot;yes&quot;}

1. Finjustera innehållet genom att beskriva vad du vill generera i **[!UICONTROL Prompt]** fält.

   Om du behöver hjälp med att skapa din fråga kan du gå till **[!UICONTROL Prompt Library]** som ger en mängd olika tips för att förbättra leveransen.

   ![](assets/image-genai-2.png){zoomable=&quot;yes&quot;}

1. Klicka **[!UICONTROL Upload brand asset]** om du vill lägga till alla varumärkesresurser som innehåller innehåll som kan ge ytterligare kontext i AI-assistenten.

   >[!IMPORTANT]
   >
   > Din fråga måste alltid vara kopplad till ett visst sammanhang.

1. Välj **[!UICONTROL Aspect ratio]** av din mediefil. Detta avgör objektets bredd och höjd.

   Du kan välja mellan vanliga proportioner som 16:9, 4:3, 3:2 eller 1:1, eller ange en anpassad storlek.

1. Anpassa **[!UICONTROL Color & tone]**, **[!UICONTROL Content type]**, **[!UICONTROL Lighting]** och **[!UICONTROL Composition]** inställningarna så att de matchar de önskade resursegenskaperna.

   ![](assets/image-genai-3.png){zoomable=&quot;yes&quot;}

1. När du är nöjd med promptkonfigurationen klickar du på **[!UICONTROL Generate]**.

1. Sök i **[!UICONTROL Variation suggestions]** för att hitta den önskade resursen.

   Klicka **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

   ![](assets/image-genai-5.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Show Similar]** om du vill visa relaterade bilder till den här varianten.

1. Klicka **[!UICONTROL Select]** när du hittat rätt innehåll.

   ![](assets/image-genai-6.png){zoomable=&quot;yes&quot;}

1. När du har definierat meddelandeinnehållet klickar du på **[!UICONTROL Simulate content]** för att styra återgivningen och kontrollera personaliseringsinställningarna med testprofiler.  [Läs mer](../preview-test/preview-content.md)

   ![](assets/image-genai-7.png){zoomable=&quot;yes&quot;}

1. När ni har definierat ert innehåll, er målgrupp och ert schema är ni redo att förbereda er för att leverera e-post. [Läs mer](../monitor/prepare-send.md)
