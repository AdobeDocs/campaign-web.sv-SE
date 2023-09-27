---
audience: end-user
title: Kom igång med Content Assistant
description: Kom igång med Content Assistant
badge: label="Beta"
source-git-commit: 8c9c74423d1b034271c96239322dd369336d0df6
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---


# Kom igång med Content Assistant {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Content Assistant"
>abstract="När du har skapat och skräddarsytt innehållet kan du använda Content Assistant för att förbättra innehållet. Den här funktionen förenklar processen med personalisering och innehållsförbättring genom att du kan finjustera innehållet genom att beskriva vad du vill generera."

Content Assistant, som bygger på generativ AI, är ett värdefullt verktyg för att förbättra e-postinnehåll. Det förenklar personalisering och innehållsförbättring, och optimerar e-postleveransen för att få ett bättre gensvar från er målgrupp.

Den här funktionen sparar tid och ger konsekvent kvalitet genom att automatiskt generera komplett e-postinnehåll. Genom att använda generativ AI kan du enkelt skapa övertygande e-postmeddelanden och förbättra kommunikationens effektivitet och effektivitet.

Du kan använda Campaign Content Assistant i dina e-postmeddelanden för att: [generera bilder](generative-image.md), [generera textinnehåll](generative-content.md), [skapa HTML i sin helhet](generative-email.md).


## Skyddsritningar och begränsningar {#generative-guardrails}

Allmänna riktlinjer för hur du använder Content Assistant för att skapa e-post anges nedan:

* Kvaliteten på det genererade innehållet påverkas i hög grad av det marknadsföringsmål/den uppmaning du anger. Använd en väldefinierad uppmaning för GenAI-modellen att tolka korrekt. 
* Ladda upp varumärkesresurser för att få korrekt varumärkesinnehåll. Annars baseras innehållet på offentligt tillgänglig information. Det överförda innehållet kan vara PDF-filer, Microsoft Word-dokument, JPEG, PNG eller ZIP-filer (med filformat som stöds).
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

