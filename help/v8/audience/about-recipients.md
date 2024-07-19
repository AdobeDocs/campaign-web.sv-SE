---
title: Kom igång med profiler
description: Lär dig övervaka och hantera profiler på Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 5a4bf85a1f70a0282405aededfb31038f9db17a8
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Kom igång med profiler {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiler"
>abstract="En profil är en post som är avsedd att ta emot meddelanden som skickas av Adobe Campaign. I den här listan kan du visa profilens information utifrån dina behörigheter. Använd filteralternativen för att bläddra i den här listan. Du kan redigera och uppdatera en liten uppsättning profilattribut."

## Vad är en profil? {#what}

En **profil**, som också kallas mottagare i klientkonsolen, representerar en post som lagras i Campaign-databasen, vilket fungerar som en nyckelkomponent för att [skapa målgrupper](create-audience.md) för leveranser och [lägga till personaliseringsdata](../personalization/personalize.md) i innehållet. Med Adobe Campaign kan ni hantera profiler smidigt, från att skapa nya tävlingsbidrag till att få en heltäckande bild av alla era profilers attribut och tjänsteabonnemang, allt via webbgränssnittet i Campaign.

Dessutom kan **[!UICONTROL test profiles]**, som identifieras som &quot;dirigeringsprofiler&quot; i klientkonsolen, göra det möjligt för dig att rikta fler mottagare som inte matchar målinriktningsvillkoren för en viss leverans. Dessa profiler innehåller fiktiv kontaktinformation, eller kontaktinformation som styrs av avsändaren. Testprofiler är korrekturmottagare: de används för att testa dina meddelanden genom att skicka korrektur. [Lär dig arbeta med testprofiler](test-profiles.md)

Både profiler och testprofiler kan användas för att testa era leveranser innan de når den avsedda målgruppen. På så sätt kan du förhandsgranska meddelandets innehåll och personalisering, skicka korrektur för testning och validering, utvärdera e-poståtergivning på olika plattformar och enheter och testa landningssidorna. [Lär dig hur du förhandsgranskar och testar leveranser](../preview-test/preview-test.md)

➡️ [Upptäck den här funktionen i videon](#video)

## Öppna listan med profiler {#access}

Profiler är tillgängliga och redigerbara i Adobe Campaign Web från posten **[!UICONTROL Customer management]** > **Profiler** i den vänstra navigeringslisten. Du kan även komma åt dem i vyn **[!UICONTROL Explorer]** från noden **[!UICONTROL Profiles & Targets]** > **[!UICONTROL Recipients]**. Därifrån kan du bläddra, skapa och hantera mappar eller undermappar samt kontrollera tillhörande behörigheter. [Lär dig skapa mappar](../get-started/permissions.md#folders)

>[!NOTE]
>
>Beroende på dina behörigheter kanske du inte har tillgång till den fullständiga listan över profiler som lagras i databasen. [Läs mer om behörigheter](../get-started/permissions.md).

Du kan filtrera listan **[!UICONTROL Profiles]** med hjälp av sökfältet eller de filter som är tillgängliga från knappen **Visa filter** . Du kan begränsa resultaten till en viss [mapp](../get-started/permissions.md#folders) med hjälp av listrutan eller lägga till regler med [frågemodelleraren](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable="yes"}

Klicka på profilens namn i listan för att få tillgång till information om profilen. En detaljerad vy av profilen öppnas så att du kan utforska dess attribut och de tjänster som han/hon prenumererar på. [Lär dig utforska profilinformation](create-profile.md)

Om du vill ta bort en profil väljer du motsvarande alternativ på menyn **[!UICONTROL More actions]**.

## Instruktionsvideo {#video}

Lär dig hur du får tillgång till, hanterar och utforskar profiler med webbgränssnittet i Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
