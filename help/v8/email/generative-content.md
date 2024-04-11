---
audience: end-user
title: Text med AI-assistenten
description: Kom igång med AI-assistenten i Campaign
badge: label="Beta"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: 23c43fad6076fc1dd1eaec2aee1664773ac7ce09
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

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

Så här kan din AI-assistent hjälpa dig att skriva övertygande e-postmeddelanden:

* **Sammanfatta**: Lång information kan överlagra e-postmottagare. Använd AI Assistant för att dra ihop viktiga punkter till tydliga, kortfattade sammanfattningar som får dem att läsa mer.

* **Samarbeta**: AI-assistenten kan hjälpa er att utöka kring specifika ämnen, med ytterligare information för bättre förståelse och engagemang.

* **Förenkla språk**: Utnyttja AI-assistenten för att förenkla ditt språk och säkerställa tydlighet och tillgänglighet för en större publik.

* **Återfras**:AI-assistenten kan omformulera sitt budskap på olika sätt, vilket håller skrivandet aktuellt och engagerande för olika målgrupper.

* **Ändra ton**: Tonen i e-postmeddelandet bör få genklang hos er målgrupp. Vare sig du vill låta informativ, lekfull eller övertygande kan AI-assistenten anpassa meddelandet därefter.

I följande exempel använder vi AI-assistenten för att förbättra innehållet i vår e-postinbjudan till vårt kommande evenemang.

1. När du har skapat och konfigurerat e-postleveransen klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din e-postleverans finns i [den här sidan](../email/create-email-content.md).

1. Anpassa din e-post efter behov och få tillgång till **[!UICONTROL AI Assistant]** -menyn.

   Du kan också välja en **[!UICONTROL Text component]** för att endast rikta in sig på ett visst innehåll.

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. Aktivera **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på leverans, leveransnamn och vald målgrupp.

   >[!IMPORTANT]
   >
   > Din uppmaning måste alltid vara knuten till ett specifikt sammanhang genom att överföra en varumärkesresurs eller aktivera **[!UICONTROL Enhance current content]** alternativ.

1. Finjustera innehållet genom att beskriva vad du vill generera i **[!UICONTROL Prompt]** fält.

   Om du behöver hjälp med att skapa din fråga kan du gå till **[!UICONTROL Prompt Library]** som ger en mängd olika tips för att förbättra leveransen.

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. Du kan växla **[!UICONTROL Subject line]** eller **[!UICONTROL Preheader]** för att inkludera dem i variantgenereringen.

   Observera att det här alternativet är tillgängligt om du inte har valt någon specifik textkomponent.

1. Klicka **[!UICONTROL Upload brand asset]** om du vill lägga till alla varumärkesresurser som innehåller innehåll som kan ge ytterligare kontext i AI-assistenten.

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. Skräddarsy uppmaningen med de olika alternativen:

   * **[!UICONTROL Communication strategy]**: Välj önskat kommunikationssätt för den genererade texten.
   * **[!UICONTROL Language]**: Välj språk för variantens innehåll.
   * **[!UICONTROL Tone]**: Se till att texten är lämplig för din målgrupp och ditt syfte.
   * **[!UICONTROL Lenght]**: Välj längden på innehållet med intervallreglaget. Endast tillgängligt om du har markerat en viss textkomponent.

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. När frågan är klar klickar du på **[!UICONTROL Generate]**.

1. Bläddra bland de genererade **[!UICONTROL Variations]** och klicka **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

1. Navigera till **[!UICONTROL Refine]** i **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner och finjustera variationerna efter dina önskemål.

   Klicka **[!UICONTROL Select]** när du hittat rätt innehåll.

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. Klicka sedan på **[!UICONTROL Simulate content]** för att styra återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

När ni har definierat ert innehåll, er målgrupp och ert schema är ni redo att förbereda er för att leverera e-post. [Läs mer](../monitor/prepare-send.md)

## Bildgenerering med AI-assistenten {#generative-image}

Använd AI Assistant för att generera olika och skräddarsydda bilder för era e-postkampanjer. Den kan till exempel användas för att:

* **Generera**: Generera en mängd övertygande bilder som är särskilt utformade för e-postkampanjer. Detaljerad kontroll över inställningar som färgpalett, blixt och komposition gör att ni kan agera med distinkta målgruppssegment och uppnå era unika kampanjmål.

* **Generera liknande**: Använd AI-assistenten för att generera bilder som liknar dem för en vald variant.

* **Varumärkesresurs**: Optimera bildurvalet för e-postkampanjer genom att utnyttja både interna varumärkesresurser och externa källor som Adobe Firefly.

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

1. Skräddarsy uppmaningen med de olika alternativen:

   * **[!UICONTROL Aspect ratio]**: Detta avgör objektets bredd och höjd. Du kan välja mellan vanliga proportioner som 16:9, 4:3, 3:2 eller 1:1, eller ange en anpassad storlek.
   * **[!UICONTROL Color & tone]**: Det övergripande utseendet på färgerna i en bild och stämningen eller atmosfären som bilden förmedlar.
   * **[!UICONTROL Content type]**: Detta kategoriserar det visuella elementets karaktär och skiljer mellan olika former av visuell representation, t.ex. foton, grafik eller grafik.
   * **[!UICONTROL Lighting]**: Detta avser blixten i en bild som formar atmosfären och markerar specifika element.
   * **[!UICONTROL Composition]**: Detta avser elementens placering i en bilds bildruta

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
