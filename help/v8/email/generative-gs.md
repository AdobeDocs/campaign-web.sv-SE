---
audience: end-user
title: Kom igång med AI-assistenten
description: Kom igång med AI-assistenten
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Kom igång med AI-assistenten {#generative-gs}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* **[Kom igång med AI-assistenten](generative-gs.md)**
* [E-postgenerering med AI-assistenten](generative-content.md)
* [SMS-generering med AI-assistenten](generative-sms.md)
* [Generering av push-meddelanden med AI-assistenten](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI Assistant"
>abstract="När du har skapat och skräddarsytt din leverans kan du använda AI-assistenten för att förbättra innehållet. Den här funktionen förenklar processen med personalisering och innehållsförbättring genom att du kan finjustera innehållet genom att beskriva vad du vill generera."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definiera kontext med AI Assistant i Campaign"
>abstract="Aktivera **Förbättra med aktuellt innehåll** växla. Ni kan också överföra ert varumärkesmaterial för att använda det som en källa. Om du inte använder det valda innehållet är det obligatoriskt att överföra och välja varumärkesresurser."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI terms"
>abstract="Du måste godkänna Adobe Experience Cloud Generative AI User Guidelines. Alla uppmaningar, kontext, tilläggsinformation eller andra indata som du anger för den här funktionen måste vara kopplade till ett specifikt sammanhang, som kan innehålla ditt varumärke, webbplatsinnehåll, data, scheman för sådana data, mallar eller andra pålitliga dokument och får inte innehålla någon personlig information (personlig information innehåller något som kan länkas tillbaka till en viss individ). Du bör granska alla utdata från den här funktionen för att se om de är korrekta och se till att de passar ditt användningssätt"
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"

AI-assistenten är ett värdefullt verktyg för att förbättra e-postinnehåll. Det förenklar personalisering och innehållsförbättring, och optimerar e-postleveransen för att få ett bättre gensvar från er målgrupp.

Den här funktionen sparar tid och ger konsekvent kvalitet genom att automatiskt generera komplett e-postinnehåll. Genom att använda generativ AI kan du enkelt skapa övertygande e-postmeddelanden och förbättra kommunikationens effektivitet och effektivitet.

>[!NOTE]
>
>Denna funktion finns i Alpha och kan ändras utan föregående meddelande. Den kommer att aktiveras i början av oktober.

## Skyddsritningar och begränsningar {#generative-guardrails}

Allmänna riktlinjer för hur du använder AI Assistant i Campaign för att generera e-post anges nedan:

* Kvaliteten på det genererade innehållet påverkas i hög grad av det marknadsföringsmål/den uppmaning du anger. Använd en väldefinierad uppmaning för GenAI-modellen att tolka korrekt. 
* Ladda upp varumärkesresurser för att få korrekt varumärkesinnehåll. Annars baseras innehållet på offentligt tillgänglig information. Det överförda innehållet kan ha följande format: PDF, JPEG, PNG eller ZIP-filer (med filformat som stöds).
* Den rekommenderade storleken för överförda varumärkesresurser är mindre än 50 MB. Större filer eller mycket bilder kan fungera, men bearbetningstiden ökar.
* Använd e-postmallar som skapats av Adobe Campaign, helst [inbyggda e-postmallar](../email/create-email-templates.md), en varumärkesspecifik mall eller anpassad mall för att skapa ditt e-postinnehåll. E-postmall med upp till 8-10 bilder rekommenderas.


Följande begränsningar gäller för AI Assistant i Campaign:

* Språket som stöds är endast engelska.
* Endast tillgängligt för e-post-, push- och SMS-kanalerna.
* GenAI-innehåll kanske inte alltid är korrekt: dela med dig av dina synpunkter så att våra tekniker kan förfina modellerna.
* Ni kan överföra flera varumärkesresurser, men ni kan bara utnyttja en för en viss generation.



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="E-postgenerering" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>E-postgenerering med AI-assistenten</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="SMS-generering" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>SMS-generering med AI-assistenten</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Push-generering" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generering av push-meddelanden med AI-assistenten</strong></a>
</div>
<p></td>
</tr></table>
