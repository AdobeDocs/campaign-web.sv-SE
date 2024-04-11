---
audience: end-user
title: Push-meddelanden med AI-assistenten i Campaign
description: Kom igång med AI-assistenten i Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: f249a73e25857e65e200f3cbd9516206aab918f9
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 1%

---

# Generering av push-meddelanden med AI-assistenten {#generative-push}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* [Kom igång med AI-assistenten](generative-gs.md)
* [E-postgenerering med AI-assistenten](generative-content.md)
* [SMS-generering med AI-assistenten](generative-sms.md)
* **[Generering av push-meddelanden med AI-assistenten](generative-push.md)**

>[!ENDSHADEBOX]


AI Assistant kan hjälpa er att optimera effekten av era leveranser genom att föreslå olika typer av innehåll som troligtvis får genklang hos er målgrupp.

Med AI Assistant kan materialet höjas till nya höjder. Den kan till exempel användas för att:

* **Sammanfatta**: Sammanfoga långt innehåll i koncisa sammanfattningar för push-meddelanden. Gå rakt på sak och se till att mottagarna direkt förstår huvudbudskapet.
* **Samarbeta**: Expandera ämnen i push-meddelanden och ge mer information och sammanhang för att få bättre förståelse.
* **Förenkla språk**: Gör dina push-meddelanden tillgängliga för en större publik med hjälp av ett tydligt och koncist språk.
* **Återfras**: Undvik upprepningar genom att låta AI Assistant omformulera ditt meddelande på olika sätt
* **Ändra ton**: Ändra den känslomässiga tonen i dina push-meddelanden. Vare sig du vill låta informativ, lekfull eller brådskande kan AI-assistenten anpassa meddelandet efter det.

>[!NOTE]
>
>Innan du börjar använda den här funktionen bör du läsa upp relaterade [Gardrutor och begränsningar](generative-gs.md#guardrails-and-limitations).

I följande exempel kommer vi att utnyttja AI-assistenten för att skapa övertygande meddelanden för att skapa en mer engagerande kundupplevelse.

1. När du har skapat och konfigurerat leveransen av push-meddelanden klickar du på **[!UICONTROL Edit content]**.

   Mer information om hur du konfigurerar din push-leverans finns i [den här sidan](../push/create-push.md).

1. Fyll i **[!UICONTROL Basic details]** för leverans. När du är klar klickar du **[!UICONTROL Edit content]**.

1. Anpassa push-meddelanden efter behov. [Läs mer](../push/content-push.md)

1. Öppna **[!UICONTROL Show AI Assistant]** -menyn.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. Finjustera innehållet genom att beskriva vad du vill generera i **[!UICONTROL Prompt]** fält.

   Om du behöver hjälp med att skapa din fråga kan du gå till **[!UICONTROL Prompt Library]** som ger en mängd olika tips för att förbättra leveransen.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. Aktivera **[!UICONTROL Enhance with current context]** för AI Assistant för att anpassa nytt innehåll baserat på leverans, leveransnamn och vald målgrupp.

   >[!IMPORTANT]
   >
   > Din uppmaning måste alltid vara knuten till ett specifikt sammanhang genom att överföra en varumärkesresurs eller aktivera **[!UICONTROL Enhance current content]** alternativ.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. Välj **[!UICONTROL Upload brand asset]** om du vill lägga till alla varumärkesresurser som innehåller innehåll som kan ge ytterligare kontext i AI-assistenten.

1. Välj vilket fält du vill generera: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]** eller **[!UICONTROL Message]**.

1. Välj **[!UICONTROL Communication strategy]** som bäst passar dina behov. Detta påverkar den genererade textens ton och format.

1. Välj **[!UICONTROL Language]** och **[!UICONTROL Tone]** som du vill att den genererade texten ska ha. På så sätt säkerställs att texten passar er målgrupp och ert syfte.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. När frågan är klar klickar du på **[!UICONTROL Generate]**.

1. Bläddra bland de genererade **[!UICONTROL Variations]** och klicka **[!UICONTROL Apply]** när du hittat rätt innehåll.

   Klicka **[!UICONTROL Preview]** om du vill visa en fullskärmsversion av den valda varianten.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. Infoga personaliseringsfält för att anpassa push-innehåll baserat på profildata. [Läs mer om innehållspersonalisering](../personalization/personalize.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. När du har definierat meddelandeinnehållet klickar du på **[!UICONTROL Simulate content]** för att styra återgivningen och kontrollera personaliseringsinställningarna med testprofiler. [Läs mer](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. När ni har definierat ert innehåll, er målgrupp och ert schema är ni redo att förbereda er för att leverera push-paket. [Läs mer](../monitor/prepare-send.md)

