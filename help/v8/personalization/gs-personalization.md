---
title: Hur gör jag ert innehåll dynamiskt?
description: Lär dig hur du gör ditt innehåll dynamiskt med hjälp av personalisering och villkorat innehåll.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Hur gör jag ert innehåll dynamiskt? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalization"
>abstract="Med personaliseringsredigeraren kan du välja, ordna, anpassa och validera alla data för att skapa en anpassad upplevelse av ditt innehåll. Ni kan personalisera era meddelanden till varje mottagare genom att utnyttja profildata och skapa villkorsstyrt innehåll för att anpassa meddelandet till varje mottagare och endast visa det innehåll som är relevant."

Som marknadsförare är det viktigt att inrikta sig på kunder som verkligen är intresserade av era erbjudanden och att engagera dem genom att tillhandahålla effektivt och relevant innehåll. Med tanke på det stora urval av mottagare som ni stöter på kan det vara tidskrävande och onödigt att skapa flera olika typer av marknadsföringsmaterial som kan tilltala olika personer. Det är här som dynamiskt innehåll blir nödvändigt.

Med Adobe Campaign funktioner för dynamiskt webbinnehåll kan du anpassa ditt innehåll baserat på den information du har samlat in om mottagarna. Genom att använda dynamiskt innehåll ser du till att era marknadsföringssatsningar blir mer relevanta och undviker att marknadsföra oönskade eller onödiga produkter eller tjänster. På så sätt blir innehållet mer tilltalande och sannolikheten för att det läses ökar. Dessutom kan ni anpassa innehållet så att mottagarna känner att de får information från en person snarare än en dator.

## Hur gör jag ert innehåll dynamiskt? {#make-content-dyn}

Du kan göra meddelandeinnehållet dynamiskt genom att infoga JavaScript-konstruktioner i redigeraren för webbuttryck i Campaign. Vid sändning av meddelanden tolkar Adobe Campaign dessa uttryck för att leverera rätt innehåll till var och en av mottagarna:

* **Anpassa dina meddelanden** till varje specifik mottagare genom att utnyttja profildata som förnamn, intressen, var de bor, vad de har köpt och mycket annat. Du kan välja vilket fält som helst tillgängligt i databasen från den anpassningsbara redigeraren som är relaterad till mottagaren, meddelandet eller leveransen. Dessa attribut kan infogas på ämnesraden eller i meddelandetexten. Följande syntax infogar mottagarens ort i ditt innehåll: `<%= recipient.location.city %>`.

  [Beskrivning: Exempel på hur du infogar mottagarens ort i ämnesraden med hjälp av anpassningsattribut.](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Skapa villkorsstyrt innehåll** för att anpassa dina leveranser till varje mottagare och visa endast det innehåll som är relevant för en viss kund baserat på den information du har om dem. På så sätt kan du visa specifika textblock och/eller bilder baserat på villkor. Anpassa t.ex. en e-postbanderoll som baseras på mottagarnas prenumeration till en viss tjänst.

  [Beskrivning: Exempel på villkorat innehåll i en e-postbanderoll baserat på mottagarens prenumeration.](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [Upptäck den här funktionen i videon](#video)

## Öppna uttrycksredigeraren {#access}

Adobe Campaign Web är en uttrycksredigerare där du kan välja, ordna, anpassa och validera alla data för att skapa en anpassad upplevelse av ditt innehåll. Uttrycksredigeraren är tillgänglig för alla kanaler, i alla fält med ikonen **[!UICONTROL Open personalization dialog]**, t.ex. ämnesradfältet, eller e-postlänkar och innehållskomponenter för text/knapp.

Här är några exempel på hur du får åtkomst till uttrycksredigeraren beroende på vilket innehåll du vill göra dynamiskt:

* *Åtkomst till uttrycksredigeraren från fältet Avsändarnamn*

  [Beskrivning: Exempel på åtkomst till uttrycksredigeraren från fältet Avsändarens namn.](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Åtkomst till uttrycksredigeraren från en e-posttextkomponent*

  [Beskrivning: Exempel på åtkomst till uttrycksredigeraren från en e-posttextkomponent.](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Åtkomst till uttrycksredigeraren från en länk i ett e-postmeddelande*

  [Beskrivning: Exempel på åtkomst till uttrycksredigeraren från en länk i ett e-postmeddelande.](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Förutom uttrycksredigeraren kan du även använda en dedikerad villkorsstyrd innehållsbyggare när du utformar ett e-postmeddelande. [Lär dig hur du skapar villkorligt innehåll i e-postmeddelanden](conditions.md)

## Instruktionsvideo {#video}

Lär dig hur du gör meddelandeinnehåll dynamiskt genom att använda uttrycksredigeraren för att anpassa meddelandet eller lägga till villkorsstyrt innehåll.

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)