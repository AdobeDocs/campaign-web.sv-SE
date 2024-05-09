---
audience: end-user
title: Push-meddelanden med AI-assistenten i Campaign
description: Kom igång med AI-assistenten i Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 1%

---

# Generering av push-meddelanden med AI-assistenten {#generative-push}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* [Kom igång med AI-assistenten](generative-gs.md)
* [E-postgenerering med AI-assistenten](generative-content.md)
* [SMS-generering med AI-assistenten](generative-sms.md)
* Generering av push-meddelanden med AI-assistenten

>[!ENDSHADEBOX]

AI Assistant kan hjälpa er att optimera effekten av era leveranser genom att föreslå olika typer av innehåll som troligtvis får genklang hos er målgrupp.

>[!NOTE]
>
>Innan du börjar använda den här funktionen bör du läsa upp relaterade [Gardrutor och begränsningar](generative-gs.md#generative-guardrails).

I följande exempel kommer vi att utnyttja AI-assistenten för att skapa övertygande meddelanden för att skapa en mer engagerande kundupplevelse.

1. När du har skapat och konfigurerat leveransen av push-meddelanden klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din push-leverans finns i [den här sidan](../push/create-push.md).

1. Fyll i **[!UICONTROL Basic details]** för leverans. När du är klar klickar du **[!UICONTROL Edit content]**.

1. Anpassa push-meddelanden efter behov. [Läs mer](../push/content-push.md)

1. Öppna **[!UICONTROL Show AI Assistant]** -menyn.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. Aktivera **[!UICONTROL Use original content]** för AI Assistant för att anpassa nytt innehåll baserat på leverans, leveransnamn och vald målgrupp.

   >[!IMPORTANT]
   >
   > Din fråga måste alltid vara knuten till ditt aktuella innehåll.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. Finjustera innehållet genom att beskriva vad du vill generera i **[!UICONTROL Prompt]** fält.

   Om du behöver hjälp med att skapa din fråga kan du gå till **[!UICONTROL Prompt Library]** som ger en mängd olika tips för att förbättra leveransen.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Upload brand asset]** om du vill lägga till alla varumärkesresurser som innehåller innehåll som kan ge ytterligare kontext i AI-assistenten.

1. Välj vilket fält du vill generera: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]** eller **[!UICONTROL Message]**.

1. Skräddarsy uppmaningen med de olika alternativen:

   * **[!UICONTROL Communication strategy]**: Välj det format som passar bäst för den genererade texten.
   * **[!UICONTROL Language]**: Välj vilket språk du vill att innehållet ska skapas på.
   * **[!UICONTROL Tone]**: Tonen i e-postmeddelandet bör få genklang hos er målgrupp. Vare sig du vill låta informativ, lekfull eller övertygande kan AI-assistenten anpassa meddelandet därefter.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. När frågan är klar klickar du på **[!UICONTROL Generate]**.

1. Bläddra bland de genererade **[!UICONTROL Variations]** och klicka **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

1. Navigera till **[!UICONTROL Refine]** i **[!UICONTROL Preview]** för att få tillgång till ytterligare anpassningsfunktioner:

   * **[!UICONTROL Use as reference content]**: Den valda varianten fungerar som referensinnehåll för att generera andra resultat.

   * **[!UICONTROL Rephrase]**: AI-assistenten kan omformulera sitt budskap på olika sätt, vilket håller skrivandet aktuellt och engagerande för olika målgrupper.

   * **[!UICONTROL Use simpler language]**: Utnyttja AI-assistenten för att förenkla ditt språk och säkerställa tydlighet och tillgänglighet för en större publik.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. Klicka **[!UICONTROL Select]** när du hittat rätt innehåll.

1. Infoga anpassningsfält för att anpassa ditt e-postinnehåll baserat på profildata. Klicka sedan på **[!UICONTROL Simulate content]** för att styra återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

När ni har definierat ert innehåll, er målgrupp och ert schema är ni redo att förbereda er för att leverera push-paket. [Läs mer](../monitor/prepare-send.md)

