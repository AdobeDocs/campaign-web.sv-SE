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
source-git-commit: e40c0b04ab985133de2d2d40e5fcb6a734ff42e9
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Kom igång med dynamiskt innehåll

För att få ut mesta möjliga av alla marknadsföringskampanjer ger Adobe Campaign er ett sätt att leverera anpassat dynamiskt innehåll som talar till kunderna på deras nivå. Använd personaliseringsfunktioner baserat på profildata för att skapa en anpassad upplevelse för olika grupper och individer: kan ni anpassa era meddelanden till varje specifik mottagare genom att utnyttja de data och den information ni har om dem. Det kan vara deras förnamn, intressen, var de bor, vad de har köpt och mycket annat.

Använd Campaign för att skapa dynamiskt innehåll och skicka personaliserade meddelanden. Personaliseringsfunktionerna kan kombineras för att förbättra budskapen och skapa en anpassad användarupplevelse.

## Hur gör man ert innehåll dynamiskt?

Du kan göra meddelandeinnehållet dynamiskt genom att infoga:

* **Anpassningsfält**: Anpassningsfält används för personalisering på första nivån av dina meddelanden. Du kan välja vilket fält som helst tillgängligt i databasen från personaliseringsredigeraren. För en leverans kan du välja vilket fält som helst som är relaterat till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten.

   Följande syntax infogar mottagarens ort i ditt innehåll: &lt;%= mottagare.location.city %>.

   ![](assets/perso-subject-line.png)

* **Villkorligt innehåll**: Konfigurera villkorligt innehåll för att lägga till innehåll baserat på mottagarens profil. Textblock och/eller bilder infogas när ett visst villkor är true. Du kan definiera den alternativa versionen av innehållet när villkoret inte är sant.

* **Inbyggda innehållsblock**: Campaign innehåller en uppsättning personaliseringsblock som innehåller en specifik återgivning som du kan infoga i dina leveranser. Du kan till exempel lägga till en logotyp, ett gratulationsmeddelande eller en länk till spegelsidan för ett e-postmeddelande. Innehållsblock är tillgängliga från ett dedikerat tävlingsbidrag i personaliseringsredigeraren.

   ![](assets/perso-content-blocks.png)

## Öppna uttrycksredigeraren {#access}

Adobe Campaign V8 Web är en uttrycksredigerare där du kan välja, ordna, anpassa och validera alla data för att skapa en anpassad upplevelse av ditt innehåll. Uttrycksredigeraren är tillgänglig för alla kanaler, i alla fält med **[!UICONTROL Open personalization dialog]** ikon, t.ex. ämnesradfältet, eller e-postlänkar och text-/knappinnehållskomponenter.

>[!NOTE]
>
>Förutom uttrycksredigeraren kan du även använda en dedikerad villkorsstyrd innehållsbyggare när du utformar ett e-postmeddelande. [Lär dig hur du skapar villkorsstyrt innehåll i e-postmeddelanden](conditions.md)

*Åtkomst till uttrycksredigeraren från fältet Avsändarens namn*

![](assets/expression-editor-access.png)

*Åtkomst till uttrycksredigeraren från en e-posttextkomponent*

![](assets/expression-editor-access-email.png)

*Åtkomst till uttrycksredigeraren från en länk i ett e-postmeddelande*

![](assets/perso-link-insert-icon.png){width="500" align="center"}


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
