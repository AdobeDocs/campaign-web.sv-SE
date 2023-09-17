---
audience: end-user
title: Skapa målgrupper
description: Lär dig skapa målgrupper i Adobe Campaign Web
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---


# Skapa målgrupper {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Målgrupper"
>abstract="Från den här skärmen kan du skapa och kombinera målgrupper till en visuell arbetsyta. Lägg till olika arbetsflödesaktiviteter som **Dela** eller **Exkludera** för att skapa nya och förfinade målgrupper."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Målgruppsinställningar"
>abstract="Ange målgruppens namn och ytterligare alternativ och klicka sedan på **Skapa publik** -knappen."

Med Campaign Web kan ni skapa nya målgrupper i ett visuellt arbetsflöde. Förutom att börja från början och skapa en enkel målgrupp kan ni också utnyttja arbetsflödesaktiviteter för att förfina era målgrupper. Ni kan till exempel dela upp olika målgrupper i en och samma målgrupp, berika målgrupper med externa attribut eller dela upp en viss målgrupp i flera.

När ni väl har skapat ert arbetsflöde lagras målgrupperna automatiskt i Campaign-databasen tillsammans med era befintliga. Dessa målgrupper kan sedan inrikta sig på kampanjer eller fristående leveranser.

De viktigaste stegen för att skapa en målgrupp är följande:

1. Skapa ett målgruppsarbetsflöde.
1. Konfigurera en Build-målgruppsaktivitet för att fråga databasen efter dina behov.
1. Lägg till arbetsflödesaktiviteter för att förfina målgruppen (valfritt).
1. Konfigurera aktiviteten Spara målgrupp.
1. Kör arbetsflödet för att spara de resulterande målgrupperna i databasen.


## Skapa din första målgrupp {#create}

Så här skapar du en målgrupp:

1. Navigera till **[!UICONTROL Audiences]** och klickar på **[!UICONTROL Create Audience]** i det övre högra hörnet.
1. Ange en etikett för er målgrupp.
1. Expandera **[!UICONTROL Additional options]** för att konfigurera avancerade målgruppsparametrar.

   Som standard skapas målgrupper i **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** utforskarmenyn. Du kan ändra standardlagringsplatsen med **[!UICONTROL Folder]** fält.

   ![](assets/audiences-settings.png)

1. När du har konfigurerat målgruppsinställningarna klickar du på **[!UICONTROL Create Audience]** -knappen.

1. En arbetsyta i arbetsflödet visas med två standardaktiviteter:

   * **[!UICONTROL Build audience]**: Detta är startpunkten i arbetsflödet, så att du kan skapa en målgrupp och använda den som grund för arbetsflödet. [Lär dig konfigurera en målgruppsaktivitet](../workflows/activities/build-audience.md)

   * **[!UICONTROL Save audience]**: Detta är det sista steget i arbetsflödet, vilket gör att du kan spara resultatet som en ny målgrupp. [Lär dig konfigurera en Spara målgruppsaktivitet](../workflows/activities/save-audience.md)

1. Om du vill utföra ytterligare åtgärder efter **[!UICONTROL Build audience]** -aktivitet, lägg till så många aktiviteter som behövs i arbetsflödet. Mer information om hur du konfigurerar arbetsflödesaktiviteter finns i [arbetsflödesdokumentation](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktiviteter är inte tillgängliga för målgruppsarbetsflöden.

   ![](assets/audience-creation-canvas.png)

1. När arbetsflödet är klart klickar du **[!UICONTROL Start]** för att genomföra det.

1. Arbetsflödet sparas i **[!UICONTROL Workflows]** -listan, medan de resulterande målgrupperna är tillgängliga i **[!UICONTROL Audiences]** lista. [Lär dig övervaka och hantera målgrupper](access-audiences.md)

## Exempel på målgruppsarbetsflöde {#example}

I exemplet nedan visas ett målgruppsarbetsflöde som är konfigurerat för att rikta sig till kvinnliga kunder som bor i New York och skapa två nya målgrupper beroende på deras intresseområde i Yoga eller Löpande utrustning. De två målgrupperna berikas med ytterligare information om kundernas köp.

LÄGG TILL SKÄRMBILD

1. Aktiviteten för att skapa målgrupper är inriktad på alla kvinnliga profiler som bor i New York.
1. Aktiviteten Enrichment berikar målgruppen med attribut från tabellen Purchases.
1. Delningsaktiviteten delar upp arbetsflödet i två banor baserat på kundernas intressecenter.
1. Med Spara målgruppsaktiviteter i slutet av varje bana sparar du varje målgrupp i databasen.
