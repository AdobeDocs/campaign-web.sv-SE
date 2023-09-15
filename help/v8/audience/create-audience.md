---
audience: end-user
title: Skapa målgrupper
description: Lär dig skapa målgrupper i Adobe Campaign Web
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Skapa målgrupper {#create-audiences}


>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Målgruppsinställningar"
>abstract="Ange namnet på målgruppen och ytterligare alternativ."

Med Campaign Web kan ni skapa arbetsflöden där ni kan kombinera befintliga målgrupper till en visuell arbetsyta. Genom att införliva olika arbetsflödesaktiviteter, som **Dela** eller **Exkludera** kan ni generera nya och förfinade målgrupper.

När ni väl har skapat ert arbetsflöde lagras målgrupperna automatiskt på Campaign Web tillsammans med era befintliga. Dessa målgrupper kan sedan inrikta sig på kampanjer eller fristående leveranser.

Så här skapar du en målgrupp:

1. Navigera till **[!UICONTROL Audiences]** och klickar på **[!UICONTROL Create Audience]** i det övre högra hörnet.
1. Ange en etikett för er målgrupp.
1. Expandera **[!UICONTROL Additional options]** för att konfigurera avancerade målgruppsparametrar.

   Som standard skapas målgrupper i **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** utforskarmenyn. Du kan ändra standardlagringsplatsen med **[!UICONTROL Folder]** fält.

   ![](assets/audiences-settings.png)

1. När du har konfigurerat målgruppsinställningarna klickar du på **[!UICONTROL Create Audience]** -knappen.

1. En arbetsyta i arbetsflödet visas med två standardaktiviteter:

   * **[!UICONTROL Build audience]**: Detta är startpunkten i arbetsflödet, så att du kan skapa en målgrupp och använda den som grund för arbetsflödet.
   * **[!UICONTROL Save audience]**: Detta är det sista steget i arbetsflödet, vilket gör att du kan spara resultatet som en ny målgrupp.

1. Anpassa arbetsflödet genom att lägga till så många aktiviteter som behövs. Mer information om hur du konfigurerar arbetsflödesaktiviteter finns i [arbetsflödesdokumentation](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktiviteter är inte tillgängliga för målgruppsarbetsflöden.

   ![](assets/audience-creation-canvas.png)

1. När arbetsflödet är klart klickar du **[!UICONTROL Start]** för att genomföra det.

1. Arbetsflödet sparas i **[!UICONTROL Workflows]** -listan, medan de resulterande målgrupperna är tillgängliga i **[!UICONTROL Audiences]** lista. [Lär dig övervaka och hantera målgrupper](access-audiences.md)
