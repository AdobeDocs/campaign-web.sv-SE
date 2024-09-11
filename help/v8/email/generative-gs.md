---
audience: end-user
title: Kom igång med AI Assistant i Adobe Campaign Web - Content Accelerator
description: Kom igång med AI Assistant i Adobe Campaign Web - Content Accelerator
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 10448255094e1be1f2c52b67d8f1f45d862f06df
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%

---

# Kom igång med AI Assistant i Adobe Campaign Web - Content Accelerator  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI Assistant"
>abstract="När du har skapat och skräddarsytt din leverans kan du använda AI-assistenten för att förbättra innehållet. Den här funktionen förenklar processen med personalisering och innehållsförbättring genom att du kan finjustera innehållet genom att beskriva vad du vill generera."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definiera kontext med AI Assistant i Campaign"
>abstract="Om du vill använda det markerade innehållet som indata för innehållsgenerering aktiverar du alternativet **Förbättra med aktuellt innehåll**. Ni kan också överföra ert varumärkesmaterial för att använda det som en källa. Om du inte använder det valda innehållet är det obligatoriskt att överföra och välja varumärkesresurser."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI terms"
>abstract="Du måste godkänna Adobe Experience Cloud Generative AI User Guidelines. Granska alla utdata från den här funktionen för att se om de är korrekta och se till att de passar ditt sätt att arbeta."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"

>[!INFO]
>
>Fördjupa dig i en praktisk upplevelse med [vår interaktiva demo](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator) som är utformad för att du ska kunna utforska dess funktioner först och till fullo förstå dess funktioner.

>[!IMPORTANT]
>
>* Innan du börjar använda den här funktionen bör du läsa upp relaterade [säkerhetsutkast och begränsningar](#generative-guardrails).
>
>* Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) innan du kan använda AI-assistenten i Adobe Campaign Web för innehållsacceleration. Kontakta din Adobe-representant om du vill veta mer.

I takt med att marknadsföringsbranschen blir mer konkurrenskraftig söker varumärkena effektiva sätt att generera slagkraftigt innehåll på ett effektivt och snabbt sätt. AI Assistant i Adobe Campaign Web for Content Acceleration, som drivs av Microsoft Azure OpenAI och Adobe Firefly, är en funktion för generering av Adobe AI-innehåll som revolutionerar sättet som marknadsförare skapar professionellt och varumärkesenhetligt innehåll i olika kanaler som e-post, SMS, Push. Med avancerade GenAI-modeller och god förståelse för varumärkesriktlinjerna genererar AI Assistant automatiskt personaliserat, engagerande och effektivt innehåll baserat på marknadsföringsmålet med innehåll som är optimerat för varumärkeskonturerade format, layouter, färgtoner och mycket annat.

Med AI Assistant kan man skapa och köra marknadsföringskampanjer i olika kanaler, som e-post, SMS och push-meddelanden, på ett intuitivt, enkelt och problemfritt sätt samtidigt som man sparar tid, förbättrar effektiviteten och får bättre resultat.

## Få åtkomst till AI Assistant Content Accelerator {#generative-access}

+++  Lär dig hur du tilldelar behörigheter för innehållsgenerering

1. **Skapa produktprofil** - Skapa en produktprofil med det specifika mönstret i [Admin Console](https://stage.adminconsole.adobe.com/): `Campaign - <instance-name> - AIAssistant`

1. **Lägg till användare** - Lägg till nödvändig användare i produktprofilen,
eller

   **Skapa användargrupp** och lägg till användargruppen i produktprofilen och lägg till användare i produktprofilen.

+++

## Skyddsritningar och begränsningar {#generative-guardrails}

Allmänna riktlinjer för hur du använder AI Assistant i Adobe Campaign Web for Content Acceleration för e-postgenerering anges nedan:

* Kvaliteten på det genererade innehållet påverkas i hög grad av det marknadsföringsmål/den uppmaning du anger. Använd en väldefinierad uppmaning för GenAI-modellen att tolka korrekt. 
* Ladda upp varumärkesresurser för att få korrekt varumärkesinnehåll. Annars baseras innehållet på offentligt tillgänglig information. Det överförda innehållet kan ha följande format: PDF, JPEG, PNG eller ZIP-filer (med filformat som stöds).
* Den maximala storleken för överförda varumärkesresurser är 50 MB. Större filer eller mycket bilder kan fungera, men bearbetningstiden ökar.
* Använd [inbyggda e-postmallar](../email/create-email-templates.md), varumärkesspecifika mallar eller anpassade mallar för att skapa e-postinnehåll med Content Accelerator. E-postmallar med upp till 8-10 bilder rekommenderas.
* Var noga med att rapportera eventuella problematiska utdata med ikonerna för tummen uppåt, tummen nedåt eller flagga när du väljer varianter.
* Din användning av AI-assistenten regleras av Adobe Experience Cloud Generative AI User Guidelines. [Läs mer](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Som en del av Adobe åtagande att främja transparens i användningen av generativa AI-verktyg för att skapa media kommer Adobe att tillämpa  när innehåll eller projekt som innehåller en Firefly-genererad mediefil hämtas eller exporteras. [Läs mer](https://helpx.adobe.com/firefly/using/content-credentials.html)

Följande begränsningar gäller för AI Assistant i Adobe Campaign Web for Content Acceleration:

* AI Assistant i Adobe Campaign Web for Content Acceleration stöds för närvarande endast på engelska. Indata som inte är engelska kan ge inkonsekventa eller felaktiga resultat. Frågor som uppstår till följd av svar som inte kommer från engelska kommer för närvarande inte att behandlas eller förbättras.
* Endast tillgängligt för e-post-, push- och SMS-kanalerna.
* GenAI-innehåll kanske inte alltid är korrekt: dela med dig av dina synpunkter så att våra tekniker kan förfina modellerna.
* Ni kan överföra flera varumärkesresurser, men ni kan bara utnyttja en för en viss generation.

## Funktioner för innehållsgenerering i AI Assistant {#generative-features}

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
