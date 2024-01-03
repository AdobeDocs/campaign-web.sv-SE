---
title: Övervaka och hantera profiler
description: Lär dig övervaka och hantera profiler på Campaign Web.
source-git-commit: 543f8b2de616f63f747fbb622053f5edd492d90d
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Övervaka och hantera profiler {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360-vy av dina profiler"
>abstract="Skapa nya profiler och övervaka dem med hjälp av kraftfulla rapporter och verktyg. Få åtkomst till attribut, interaktioner och loggar för dina profiler. Använd filtreringsalternativen för att bläddra i profillistan, redigera och uppdatera deras profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Se versionsinformation"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiler"
>abstract="En profil är en individ som ska ta emot meddelanden från Adobe Campaign. I den här listan kan du visa profilens information utifrån dina behörigheter. Använd filteralternativen för att bläddra i den här listan. Du kan redigera och uppdatera en liten uppsättning profilattribut."

## Kom igång med profiler {#gs}

En profil på Adobe Campaign Web är en individ som lagras i databasen och som en nyckelkomponent för att skapa målgrupper för leveranser och lägga till personaliseringsdata i innehållet. Olika typer av profiler lagras i databasen, till exempel Testprofiler, som är utformade för att testa dina leveranser innan de skickas till slutanvändarna. [Lär dig hur du arbetar med testprofiler](test-profiles.md)

Profiler är tillgängliga från **Profiler** inträde i det vänstra navigeringsfältet. Du kan även komma åt dem från **Explorer** där du kan bläddra, skapa mappar, undermappar och kontrollera behörigheter.

Du kan filtrera profillistan med hjälp av sökfältet eller de filter som finns i **Visa filter** -knappen.

![](assets/profiles-list.png)

>[!NOTE]
>
>Beroende på dina behörigheter kanske du inte har tillgång till den fullständiga listan över profiler som lagras i databasen. Läs mer om behörigheter i [det här avsnittet](../get-started/permissions.md).

## Få åtkomst till och redigera profilattribut {#access}

Om du vill få tillgång till information om en profil klickar du på dess namn i profillistan.

![](assets/profiles-details.png)

På den här skärmen kan du få tillgång till detaljerad information om profilen:

* The **[!UICONTROL Details]** kan du bläddra igenom profilens attribut. Om du vill redigera ett attribut gör du ändringarna i det önskade fältet och klickar på knappen **[!UICONTROL Save]** -knappen.
* The **[!UICONTROL Subscriptions]** -fliken innehåller information om de tjänster som profilen prenumererar på. [Lär dig arbeta med prenumerationstjänster](manage-services.md)
* The **[!UICONTROL Logs]** i skärmens övre högra hörn kan du visa en historik över profilens interaktioner genom att skicka, exkludera och spåra loggar samt de förslag som presenteras för profilen.
