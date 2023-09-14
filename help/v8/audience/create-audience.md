---
audience: end-user
title: Skapa målgrupper
description: Lär dig skapa målgrupper i Adobe Campaign Web
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Skapa målgrupper {#create-audiences}

Med Campaign Web kan ni skapa arbetsflöden där ni kan kombinera befintliga målgrupper till en visuell arbetsyta och utnyttja olika aktiviteter (dela, exkludera..) för att skapa nya målgrupper.

När det är klart sparas de resulterande målgrupperna i Campaign Web tillsammans med befintliga målgrupper och kan utnyttjas i fristående leveranser eller kampanjer för att nå ut till individer.

## Skapa din första målgrupp {#create}

Så här skapar du en målgrupp:

1. Navigera till **[!UICONTROL Audiences]** meny och klicka **[!UICONTROL Create Audience]** längst upp till höger.
1. Ange en etikett för målgruppen.
1. Expandera avsnittet Ytterligare alternativ för att konfigurera avancerade parametrar för målgruppen.

   >[!NOTE]
   >
   >Som standard skapas målgrupper i utforskarmenyn för profiler och mål/listor. Du kan ändra standardlagringsplatsen i **[!UICONTROL Folder]** fält.

1. När målgruppsinställningarna är konfigurerade klickar du på **[!UICONTROL Create Audience]** -knappen.

1. En arbetsyta i arbetsflödet visas med två standardaktiviteter:

   * **[!UICONTROL Build audience]**: startpunkten för arbetsflödet. Med den här aktiviteten kan du välja en eller flera målgrupper som grund för ditt arbetsflöde,
   * **[!UICONTROL Save audience]**: det sista steget i arbetsflödet. Med den här aktiviteten kan du spara resultatet av arbetsflödet till en ny målgrupp.

1. Konfigurera arbetsflödet genom att lägga till så många aktiviteter som behövs. Mer information om hur du konfigurerar de olika aktiviteterna finns i [arbetsflödesdokumentation](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktiviteter är inte tillgängliga för målgruppsarbetsflöden.

   ![](assets/audience-creation-canvas.png)

1. När arbetsflödet är klart klickar du **[!UICONTROL Start]** för att genomföra det.

1. Arbetsflödet sparas i **[!UICONTROL Workflows]** och de slutliga målgrupperna i **[!UICONTROL Audiences]** lista. [Lär dig övervaka och hantera målgrupper](access-audiences.md)
