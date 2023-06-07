---
title: Kom igång med dynamiskt innehåll
description: Lär dig hur du gör ditt innehåll dynamiskt med personalisering, villkorsstyrt innehåll och inbyggda innehållsblock.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---


# Kom igång med dynamiskt innehåll

För att få ut mesta möjliga av alla marknadsföringskampanjer ger Adobe Campaign er ett sätt att leverera anpassat dynamiskt innehåll som talar till kunderna på deras nivå. Använd personaliseringsfunktioner baserat på profildata för att skapa en anpassad upplevelse för olika grupper och individer: kan ni anpassa era meddelanden till varje specifik mottagare genom att utnyttja de data och den information ni har om dem. Det kan vara deras förnamn, intressen, var de bor, vad de har köpt och mycket annat.

Använd Campaign för att skapa dynamiskt innehåll och skicka personaliserade meddelanden. Personaliseringsfunktionerna kan kombineras för att förbättra budskapen och skapa en anpassad användarupplevelse.

Du kan göra meddelandeinnehållet dynamiskt genom att infoga:

* **Fält för personalisering**

   Anpassningsfält används för personalisering på första nivån av dina meddelanden. Du kan välja vilket fält som helst tillgängligt i databasen från personaliseringsredigeraren. För en leverans kan du välja vilket fält som helst som är relaterat till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten.

   ![](assets/perso-subject-line.png)

   Följande syntax infogar mottagarens ort i ditt innehåll: &lt;%= mottagare.location.city %>.

* **Villkorligt innehåll**

   Konfigurera villkorsstyrt innehåll för att lägga till dynamisk personalisering baserat på mottagarens profil till exempel. Textblock och/eller bilder infogas när ett visst villkor är true. Du kan definiera den alternativa versionen av innehållet när villkoret inte är sant.

* **Inbyggda innehållsblock**

   Campaign innehåller en uppsättning personaliseringsblock som innehåller en specifik återgivning som du kan infoga i dina leveranser. Du kan till exempel lägga till en logotyp, ett gratulationsmeddelande eller en länk till spegelsidan för ett e-postmeddelande. Innehållsblock är tillgängliga från ett dedikerat tävlingsbidrag i personaliseringsredigeraren.

   ![](assets/perso-content-blocks.png)

## Var kan jag lägga till dynamiskt innehåll?

Adobe Campaign V8 Web är en uttrycksredigerare där du kan välja, ordna, anpassa och validera alla data för att skapa en anpassad upplevelse av ditt innehåll.

Uttrycksredigeraren är tillgänglig för alla kanaler, i alla fält med ikonen Öppna personalisering, t.ex. ämnesradfältet, eller innehållskomponenter för text och knapp i e-postmeddelanden.

![](assets/expression-editor-access.png)

![](assets/expression-editor-access-email.png)

Dessutom kan du skapa ett dedikerat villkorsstyrt innehåll när du utformar ett e-postmeddelande. [Lär dig hur du skapar villkorsstyrt innehåll i e-postmeddelanden](conditions.md)

## Låt oss dyka djupare

Nu när du har en förståelse för hur du gör ditt innehåll dynamiskt är det dags att gå djupare in i dessa dokumentationsavsnitt för att börja arbeta med funktionen.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Anpassa innehåll" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Lägg till personalisering</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Lead" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Lägga till villkorligt innehåll</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Sällan" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Lägg till inbyggda innehållsblock</strong></a>
</div>
<p></td>
</tr></table>
