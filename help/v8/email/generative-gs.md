---
audience: end-user
title: Kom igång med AI Assistant
description: Kom igång med AI Assistant
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 1%

---

# Arbeta med AI Assistant {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI Assistant"
>abstract="När du har skapat och personaliserat materialet kan du använda AI Assistant för att förbättra innehållet. Den här funktionen förenklar personalisering och innehållsförbättring genom att du kan finjustera innehållet genom att beskriva vad du vill generera."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definiera kontext med AI Assistant i Campaign"
>abstract="Aktivera alternativet **Förbättra med aktuellt innehåll** om du vill använda det markerade innehållet som indata för innehållsgenerering. Ni kan också överföra ert varumärkesmaterial för att använda det som en källa. Om du inte använder det valda innehållet är det obligatoriskt att överföra och välja varumärkesresurser."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI terms"
>abstract="Du måste godkänna Adobe Experience Cloud Generative AI User Guidelines. Granska alla utdata från den här funktionen för att se om de är korrekta och se till att de passar ditt sätt att arbeta."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"

>[!INFO]
>
>Fördjupa dig i en praktisk upplevelse med [vår förhandsvisning av aktiva funktioner](https://experienceleague.adobe.com/sv/apps/journey-optimizer/ai-assistant-content-accelerator), som är utformad för att du ska kunna utforska dess funktioner först och till fullo förstå dess funktioner.

I takt med att marknadsföringsbranschen blir mer konkurrenskraftig söker varumärkena effektiva sätt att snabbt generera slagkraftigt innehåll. AI Assistant på Adobe Campaign Web, som drivs av Microsoft Azure OpenAI och Adobe Firefly, är Adobe funktioner för generering av AI-innehåll som förändrar hur marknadsförare skapar professionellt och varumärkesenhetligt innehåll i olika kanaler som e-post, SMS och push-meddelanden. Med avancerade GenAI-modeller och en god förståelse för varumärkesriktlinjerna genererar AI Assistant automatiskt personaliserat, engagerande och effektivt innehåll baserat på marknadsföringsmålet, optimerat innehåll för varumärkeskonturerade format, layouter, färgton och mycket annat.

AI Assistant förenklar framtagning och körning av marknadsföringskampanjer i flera kanaler, som e-post, SMS och push-meddelanden, vilket sparar tid, förbättrar effektiviteten och ger bättre resultat.

>[!IMPORTANT]
>
>* Granska de relaterade [Guardrutorna och begränsningarna](#generative-guardrails) innan du använder den här funktionen.
>
>* Du måste godkänna ett [användaravtal](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) innan du kan använda AI Assistant på Adobe Campaign Web. Kontakta din Adobe-representant om du vill veta mer.

## Access AI Assistant {#generative-access}

AI Assistant för e-post, push-meddelanden och SMS är nu i General Availability (GA) och tillgängligt för alla användare. Nödvändiga behörigheter och steg för att bevilja åtkomst till användare beskrivs nedan.

+++ Lär dig hur du tilldelar behörigheter för innehållsgenerering

1. **Skapa produktprofil** - Skapa en produktprofil med följande specifika mönster i [Admin Console](https://stage.adminconsole.adobe.com/):
   `Campaign - <instance-name> - AIAssistant`

1. **Lägg till användare** - Lägg till den användare som krävs i produktprofilen,\
   eller\
   **Skapa användargrupp** och lägg till användargruppen i produktprofilen. Lägg sedan till användare i produktprofilen.

Lär dig definiera behörigheter i Campaign i [det här avsnittet](../get-started/permissions.md).

+++

## Skyddsritningar och begränsningar {#generative-guardrails}

Allmänna riktlinjer för hur du använder AI Assistant på Adobe Campaign Web för att skapa e-post anges nedan:

* Kvaliteten på det genererade innehållet beror till stor del på det marknadsföringsmål eller den fråga du anger. Använd en väldefinierad uppmaning för GenAI-modellen att tolka korrekt.
* Överför varumärkesresurser för att säkerställa korrekt varumärkesanpassat innehåll. Annars baseras innehållet på offentligt tillgänglig information. Det överförda innehållet kan ha följande format: PDF-, JPEG-, PNG- eller ZIP-filer (med filformat som stöds).
* Den maximala storleken för överförda varumärkesresurser är 50 MB. Större filer eller många bilder kan öka bearbetningstiden.
* Använd [inbyggda e-postmallar](../content/create-email-templates.md), varumärkesspecifika mallar eller anpassade mallar för att skapa ditt e-postinnehåll med hjälp av AI Assistant. E-postmallar med upp till 8-10 bilder rekommenderas.
* Rapportera eventuella problematiska utdata med upp- och nedpilarna eller flaggikonerna när du väljer varianter.
* Din användning av AI Assistant regleras av Adobe Experience Cloud Generative AI User Guidelines. [Läs mer](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Som en del av Adobe strävan efter transparens i användningen av generativa AI-verktyg för att skapa media använder Adobe Content Credentials när innehåll eller projekt som innehåller en Firefly-genererad mediefil hämtas eller exporteras. [Läs mer](https://helpx.adobe.com/se/firefly/using/content-credentials.html).

Följande begränsningar gäller för AI Assistant på Adobe Campaign Web:

* AI Assistant på Adobe Campaign Web stöds för närvarande endast på engelska. Indata som inte är engelska kan ge inkonsekventa eller felaktiga resultat. Frågor som uppstår till följd av svar från andra språk än engelska kommer för närvarande inte att behandlas eller förbättras.
* Endast tillgängligt för e-post-, push- och SMS-kanalerna.
* GenAI-innehåll kanske inte alltid är korrekt. Dela med dig av dina synpunkter så att teknikerna kan förfina modellerna.
* Ni kan överföra flera varumärkesresurser, men ni kan bara utnyttja en för en viss generation.

## Funktioner för innehållsgenerering i AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[E-postgenerering med AI Assistant]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>E-postgenerering med AI-assistenten</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[SMS-generering med AI Assistant]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>SMS-generering med AI Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Generering av push-meddelanden med AI Assistant]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generering av push-meddelanden med AI-assistenten</strong></a>
</div>
<p></td>
</tr></table>