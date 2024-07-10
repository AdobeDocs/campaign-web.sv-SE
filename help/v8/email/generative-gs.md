---
audience: end-user
title: Kom igång med AI-assistenten
description: Kom igång med AI-assistenten
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 27e97731ebd2987cc6f653f90a515473caa175d6
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Kom igång med AI-assistenten {#generative-gs}

>[!BEGINSHADEBOX]

**Innehållsförteckning**

* Kom igång med AI-assistenten
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

I takt med att marknadsföringsbranschen blir mer konkurrenskraftig söker varumärkena effektiva sätt att generera slagkraftigt innehåll på ett effektivt och snabbt sätt. AI Assistant i Campaign, som bygger på Azure OpenAI och Azure-vision, är innehållsgenereringsfunktionen i Adobe AI som revolutionerar det sätt som marknadsförare skapar professionellt och varumärkesenhetligt innehåll i olika kanaler som e-post, SMS, Push. Med avancerade GenAI-modeller och god förståelse för varumärkesriktlinjerna genererar AI Assistant automatiskt personaliserat, engagerande och effektivt innehåll baserat på marknadsföringsmålet med innehåll som är optimerat för varumärkeskonturerade format, layouter, färgtoner och mycket annat.

Med AI Assistant kan man skapa och köra marknadsföringskampanjer i olika kanaler, som e-post, SMS och push-meddelanden, på ett intuitivt, enkelt och problemfritt sätt samtidigt som man sparar tid, förbättrar effektiviteten och får bättre resultat.

>[!NOTE]
>
>Funktionen finns i Beta-versionen och kan ändras utan föregående meddelande.

## Skyddsritningar och begränsningar {#generative-guardrails}

Allmänna riktlinjer för hur du använder AI Assistant i Campaign för att generera e-post anges nedan:

* Kvaliteten på det genererade innehållet påverkas i hög grad av det marknadsföringsmål/den uppmaning du anger. Använd en väldefinierad uppmaning för GenAI-modellen att tolka korrekt. 
* Ladda upp varumärkesresurser för att få korrekt varumärkesinnehåll. Annars baseras innehållet på offentligt tillgänglig information. Det överförda innehållet kan ha följande format: PDF, JPEG, PNG eller ZIP-filer (med filformat som stöds).
* Den maximala storleken för överförda varumärkesresurser är 50 MB. Större filer eller mycket bilder kan fungera, men bearbetningstiden ökar.
* Använd e-postmallar som skapats av Adobe Campaign, helst [inbyggda e-postmallar](../email/create-email-templates.md), en varumärkesspecifik mall eller anpassad mall för att skapa ditt e-postinnehåll. E-postmall med upp till 8-10 bilder rekommenderas.
* Var noga med att rapportera eventuella problematiska utdata med ikonerna för tummen uppåt, tummen nedåt eller flagga när du väljer varianter.
* Din användning av AI-assistenten regleras av Adobe Experience Cloud Generative AI User Guidelines. [Läs mer](https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

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
