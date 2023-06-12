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
source-git-commit: bf5ff77b695a5a8584bad7784597bf1521bcb23e
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Kom igång med dynamiskt innehåll

Att leverera relevant innehåll till era kunder är avgörande för att ni ska kunna tilltala en mängd olika kunder och ni ska kunna spela deras intresse så att ert marknadsföringsmaterial blir läst.

För att få ut så mycket som möjligt av alla marknadsföringskampanjer ger Adobe Campaign er ett sätt att skapa en anpassad upplevelse för olika grupper och individer genom att leverera anpassat dynamiskt innehåll som talar till kunderna på deras nivå genom att utnyttja den information ni har samlat in om dem.

* **Anpassa era meddelanden** till varje enskild mottagare genom att utnyttja profildata som förnamn, intressen, var de bor, vad de köpt och mycket annat.

  Du kan välja vilket fält som helst tillgängligt i databasen från den anpassade redigeraren som är relaterad till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten. Följande syntax infogar mottagarens ort i ditt innehåll: &lt;%= mottagare.location.city %>.

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **Skapa villkorsstyrt innehåll** för att anpassa era leveranser till varje mottagare och endast visa det innehåll som är relevant för en viss kund baserat på den information ni har om dem. På så sätt kan du visa specifika textblock och/eller bilder baserat på villkor. Anpassa t.ex. en e-postbanderoll som baseras på mottagarnas prenumeration till en viss tjänst.

  ![](assets/condition-sample.png){width="800" align="center"}

* **Använd personaliseringsblock** för att spara tid och enkelt kunna återanvända personaliserat innehåll i era meddelanden. Campaign innehåller en uppsättning personaliseringsblock som innehåller en specifik återgivning som du kan infoga i dina leveranser. Du kan till exempel lägga till en logotyp, ett gratulationsmeddelande eller en länk till spegelsidan för ett e-postmeddelande. Innehållsblock är tillgängliga från ett dedikerat tävlingsbidrag i personaliseringsredigeraren.

  ![](assets/content-blocks.png){width="800" align="center"}

## Öppna uttrycksredigeraren {#access}

Adobe Campaign V8 Web är en uttrycksredigerare där du kan välja, ordna, anpassa och validera alla data för att skapa en anpassad upplevelse av ditt innehåll. Uttrycksredigeraren är tillgänglig för alla kanaler, i alla fält med **[!UICONTROL Open personalization dialog]** ikon, t.ex. ämnesradfältet, eller e-postlänkar och text-/knappinnehållskomponenter.

Här är några exempel på hur du får åtkomst till uttrycksredigeraren beroende på vilket innehåll du vill göra dynamiskt:

* *Åtkomst till uttrycksredigeraren från fältet Avsändarens namn*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *Åtkomst till uttrycksredigeraren från en e-posttextkomponent*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *Åtkomst till uttrycksredigeraren från en länk i ett e-postmeddelande*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>Förutom uttrycksredigeraren kan du även använda en dedikerad villkorsstyrd innehållsbyggare när du utformar ett e-postmeddelande. [Lär dig hur du skapar villkorsstyrt innehåll i e-postmeddelanden](conditions.md)

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
