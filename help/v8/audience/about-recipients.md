---
title: Kom igång med profiler
description: Lär dig övervaka och hantera profiler på Campaign Web.
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Kom igång med profiler {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="360-vy av dina profiler"
>abstract="Skapa nya profiler och övervaka dem med hjälp av kraftfulla rapporter och verktyg. Få åtkomst till attribut, interaktioner och loggar för dina profiler. Använd filtreringsalternativen för att bläddra i profillistan, redigera och uppdatera deras profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Se versionsinformation"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360-vy av dina profiler"
>abstract="Skapa nya profiler och övervaka dem med hjälp av kraftfulla rapporter och verktyg. Få åtkomst till attribut, interaktioner och loggar för dina profiler. Använd filtreringsalternativen för att bläddra i profillistan, redigera och uppdatera deras profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Se versionsinformation"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiler"
>abstract="En profil är en individ som är avsedd att ta emot meddelanden som skickas av Adobe Campaign. I den här listan kan du visa profilens information utifrån dina behörigheter. Använd filteralternativen för att bläddra i den här listan. Du kan redigera och uppdatera en liten uppsättning profilattribut."

## Vad är en profil? {#what}

A **profil**, som också kallas &quot;mottagare&quot; i klientkonsolen, representerar en person som lagras i Campaign-databasen och fungerar som en nyckelkomponent för att [skapa målgrupper](create-audience.md) för leveranser och [lägg till personalisering](../personalization/personalize.md) data till ert innehåll. Med Adobe Campaign kan ni hantera profiler smidigt, från att skapa nya tävlingsbidrag till att få en heltäckande bild av alla era profilers attribut och tjänsteabonnemang, allt via webbgränssnittet i Campaign.

Dessutom **[!UICONTROL test profiles]**, som identifieras som&quot;dirigerade profiler&quot; i klientkonsolen, gör att du kan rikta dig till fler mottagare som inte matchar målinriktningsvillkoren för en viss leverans. Dessa profiler innehåller fiktiv kontaktinformation, eller kontaktinformation som styrs av avsändaren. De kan läggas in i målgruppen för ett meddelande för att upptäcka om mottagardatabasen används på ett bedrägligt sätt eller för att säkerställa att e-postmeddelandena kommer in i inkorgen. [Lär dig hur du arbetar med testprofiler](test-profiles.md)

Både profiler och testprofiler kan användas för att testa era leveranser innan de når den avsedda målgruppen. På så sätt kan du förhandsgranska meddelandets innehåll och personalisering, skicka korrektur för testning och validering, utvärdera e-poståtergivning på olika plattformar och enheter och testa landningssidorna. [Lär dig hur du förhandsgranskar och testar leveranser](../preview-test/preview-test.md)

## Öppna listan med profiler {#access}

Profilerna är tillgängliga och redigerbara i Adobe Campaign Web från **[!UICONTROL Customer management]** > **Profiler** inträde i det vänstra navigeringsfältet. Du kan även komma åt dem i **[!UICONTROL Explorer]** visa, från **[!UICONTROL Profiles & Targets]** > **[!UICONTROL Recipients]** nod. Därifrån kan du bläddra, skapa och hantera mappar eller undermappar samt kontrollera tillhörande behörigheter. [Lär dig hur du skapar mappar](../get-started/permissions.md#folders)

>[!NOTE]
>
>Beroende på dina behörigheter kanske du inte har tillgång till den fullständiga listan över profiler som lagras i databasen. [Läs mer om behörigheter](../get-started/permissions.md).

Du kan filtrera **[!UICONTROL Profiles]** med sökfältet eller de filter som finns i **Visa filter** -knappen. Du kan begränsa resultatet till en viss [mapp](../get-started/permissions.md#folders) använda listrutan eller lägga till regler med [frågemodellerare](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable=&quot;yes&quot;}

Klicka på profilens namn i listan för att få tillgång till information om profilen. En detaljerad vy av profilen öppnas så att du kan utforska dess attribut och de tjänster som han/hon prenumererar på. [Lär dig hur du utforskar profildetaljer](create-profile.md)

Om du vill ta bort en profil väljer du motsvarande alternativ i dialogrutan **[!UICONTROL More actions]** -menyn.
