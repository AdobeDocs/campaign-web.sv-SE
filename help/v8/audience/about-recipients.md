---
title: Övervaka och hantera profiler
description: Lär dig övervaka och hantera profiler på Campaign Web.
badge: label="Begränsad tillgänglighet"
source-git-commit: e61878f325575377865186fb9cb63b831ac843fd
workflow-type: tm+mt
source-wordcount: '658'
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

Profiler kan bara läggas till från Campaign-klientkonsolen. De kan dock nås via Adobe Campaign Web från **Profiler** inträde i det vänstra navigeringsfältet. Du kan även komma åt dem från **Explorer** där du kan bläddra, skapa mappar, undermappar och kontrollera behörigheter.

Du kan filtrera profillistan med hjälp av sökfältet eller de filter som finns i **Visa filter** -knappen.

![](assets/profiles-list.png)

>[!NOTE]
>
>Beroende på dina behörigheter kanske du inte har tillgång till den fullständiga listan över profiler som lagras i databasen. Läs mer om behörigheter i [det här avsnittet](../get-started/permissions.md).

## Få åtkomst till och redigera profilattribut {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Grundläggande information"
>abstract="I det här avsnittet finns information om de grundläggande detaljerna i profilen. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Kontaktinformation"
>abstract="I det här avsnittet finns information om profilens kontaktinformation. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title= "Address"
>abstract="I det här avsnittet finns information om profilens postadress och adresskvalitet. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Kontoinformation"
>abstract="I det här avsnittet finns information om profilens kontoinformation. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Mottagarna kontaktar inte längre"
>abstract="I det här avsnittet finns information om kontaktinställningarna för profilen. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Anpassade fält"
>abstract="Anpassade fält är specifika attribut som är anpassade efter dina behov och som har konfigurerats för din instans. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Övriga"
>abstract="I det här avsnittet finns ytterligare inbyggda attribut. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Mottagarens prenumerationslista"
>abstract="På den här fliken visas alla tjänster som profilen prenumererar på."

Om du vill få tillgång till information om en profil klickar du på dess namn i profillistan.

![](assets/profiles-details.png)

På den här skärmen kan du få tillgång till detaljerad information om profilen:

* The **[!UICONTROL Details]** kan du bläddra igenom profilens inbyggda och anpassade attribut. Om du vill redigera ett attribut gör du ändringarna i det önskade fältet och klickar på knappen **[!UICONTROL Save]** -knappen.
* The **[!UICONTROL Subscriptions]** -fliken innehåller information om de tjänster som profilen prenumererar på. [Lär dig arbeta med prenumerationstjänster](manage-services.md)
* The **[!UICONTROL Logs]** i skärmens övre högra hörn kan du visa en historik över profilens interaktioner genom att skicka, exkludera och spåra loggar samt de förslag som presenteras för profilen.
