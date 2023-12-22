---
audience: end-user
title: Kom igång med Content Assistant
description: Kom igång med Content Assistant
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: bc1b4186b5869d104c6b14e09160f28bf3e28f95
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Kom igång med Content Assistant {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn5"
>title="Gen AI för e-postinnehåll"
>abstract="Vår Gen AI-teknik använder avancerade algoritmer för att generera engagerande och personaliserat innehåll. Öka öppningsfrekvensen, klickfrekvensen och konverteringsgraden med Gen AI:s generering av intelligent innehåll. Ligg steget före konkurrenterna och lyft ditt marknadsföringsspel med Gen AI om e-postinnehåll."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Se versionsinformation"



>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Content Assistant"
>abstract="När du har skapat och skräddarsytt innehållet kan du använda Content Assistant för att förbättra innehållet. Den här funktionen förenklar processen med personalisering och innehållsförbättring genom att du kan finjustera innehållet genom att beskriva vad du vill generera."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definiera kontext för innehållsgenerering"
>abstract="Aktivera **Förbättra med aktuellt innehåll** växla. Ni kan också överföra ert varumärkesmaterial för att använda det som en källa. Om du inte använder det valda innehållet är det obligatoriskt att överföra och välja varumärkesresurser."

Content Assistant, som bygger på generativ AI, är ett värdefullt verktyg för att förbättra e-postinnehåll. Det förenklar personalisering och innehållsförbättring, och optimerar e-postleveransen för att få ett bättre gensvar från er målgrupp.

Den här funktionen sparar tid och ger konsekvent kvalitet genom att automatiskt generera komplett e-postinnehåll. Genom att använda generativ AI kan du enkelt skapa övertygande e-postmeddelanden och förbättra kommunikationens effektivitet och effektivitet.


Du kan använda Campaign Content Assistant i dina e-postmeddelanden för att: [generera bilder](generative-image.md), [generera textinnehåll](generative-content.md), [skapa HTML i sin helhet](generative-email.md).

>[!NOTE]
>
>Denna funktion finns i Alpha och kan ändras utan föregående meddelande. Den kommer att aktiveras i början av oktober.

## Skyddsritningar och begränsningar {#generative-guardrails}

Allmänna riktlinjer för hur du använder Content Assistant för att skapa e-post anges nedan:

* Kvaliteten på det genererade innehållet påverkas i hög grad av det marknadsföringsmål/den uppmaning du anger. Använd en väldefinierad uppmaning för GenAI-modellen att tolka korrekt. 
* Ladda upp varumärkesresurser för att få korrekt varumärkesinnehåll. Annars baseras innehållet på offentligt tillgänglig information. Det överförda innehållet kan ha följande format: PDF, JPEG, PNG eller ZIP-filer (med filformat som stöds).
* Den rekommenderade storleken för överförda varumärkesresurser är mindre än 10 MB. Större filer eller mycket bilder kan fungera, men bearbetningstiden ökar.
* Använd en e-postmall som skapats av Adobe Campaign, eller helst [inbyggda e-postmallar](../content/email-sample-templates.md) för att skapa e-postinnehåll. E-postmall med upp till 8-10 bilder rekommenderas.


Följande begränsningar gäller Campaign Content Assistant:

* Språket som stöds är endast engelska
* Endast tillgängligt för e-postkanalen
* GenAI-innehåll kanske inte alltid är korrekt: dela med dig av dina synpunkter så att våra tekniker kan förfina modellerna
* Du kan överföra flera varumärkesresurser, men du kan bara använda en för en viss generation



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Textgenerering" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Skapa text med Content Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Bildgenerering" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Bildgenerering med Content Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="E-postgenerering" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>E-postgenerering med Content Assistant</strong></a>
</div>
<p></td>
</tr></table>
