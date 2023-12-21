---
audience: end-user
title: Skapa målgrupper
description: Lär dig skapa målgrupper i Adobe Campaign Web
badge: label="Beta"
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 686bcc06591d56c2827a6826286503659ee6b26c
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Skapa målgrupper {#create-audiences}



>[!CONTEXTUALHELP]
>id="acw_homepage_rn1"
>title="Målgruppssammansättning"
>abstract="Skapa nya målgrupper i ett visuellt arbetsflöde. Förutom att börja från scratch och skapa en enkel målgrupp kan ni också utnyttja arbetsflödesaktiviteter för att förfina er målgrupp. Kombinera flera olika målgrupper till en enda, berika er målgrupp med externa attribut eller dela upp en grupp i flera målgrupper baserat på valfria regler."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Målgrupper"
>abstract="Från den här skärmen kan du komma åt listan över alla målgrupper som kan användas i dina leveranser. Klicka **Skapa** skapa nya målgrupper i en visuell arbetsyta med hjälp av olika arbetsflödesaktiviteter som **Dela** eller **Exkludera**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Målgruppsinställningar"
>abstract="Ange målgruppens namn och ytterligare alternativ och klicka sedan på **Skapa publik** -knappen."

Med Campaign Web kan ni skapa nya målgrupper i ett visuellt arbetsflöde. Förutom att börja från scratch och skapa en enkel målgrupp kan ni också utnyttja arbetsflödesaktiviteter för att förfina er målgrupp. Ni kan till exempel kombinera flera olika målgrupper till en enda, berika er målgrupp med externa attribut eller dela upp en grupp i flera målgrupper baserat på valfria regler.

När ni väl har skapat ert arbetsflöde lagras målgrupperna automatiskt i Campaign-databasen tillsammans med era befintliga. Dessa målgrupper kan sedan målgruppsanpassas i arbetsflöden eller fristående leveranser.

## Skapa din första målgrupp {#create}

Så här skapar du en målgrupp:

1. Navigera till **[!UICONTROL Audiences]** och klickar på **[!UICONTROL Create Audience]** i det övre högra hörnet.
1. Ange en etikett för er målgrupp.
1. Expandera **[!UICONTROL Additional options]** för att konfigurera avancerade målgruppsparametrar.

   Som standard skapas målgrupper i **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** utforskarmenyn. Du kan ändra standardlagringsplatsen med **[!UICONTROL Folder]** fält.

   ![](assets/audiences-settings.png)

1. När du har konfigurerat målgruppsinställningarna klickar du på **[!UICONTROL Create Audience]** -knappen. En arbetsyta i arbetsflödet visas med två standardaktiviteter:

   * **[!UICONTROL Build audience]**: Detta är startpunkten i arbetsflödet, så att du kan skapa en målgrupp och använda den som grund för arbetsflödet.

   * **[!UICONTROL Save audience]**: Detta är det sista steget i arbetsflödet, vilket gör att du kan spara arbetsflödesresultaten som en ny målgrupp.

1. Öppna **[!UICONTROL Build audience]** och använd regelbyggaren för att definiera den population som ska ingå i målgruppen genom att filtrera data i databasen. [Lär dig konfigurera en målgruppsaktivitet](../workflows/activities/build-audience.md)

1. Om du vill utföra ytterligare åtgärder för den population som är avsedd för arbetsflödet lägger du till så många aktiviteter som behövs och kopplar ihop dem. Mer information om hur du konfigurerar arbetsflödesaktiviteter finns i [arbetsflödesdokumentation](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktiviteter är inte tillgängliga för målgruppsarbetsflöden.

   ![](assets/audience-creation-canvas.png)

1. Konfigurera **[!UICONTROL Save audience]** för att ange hur du vill spara den beräknade populationen uppströms i arbetsflödet. [Lär dig konfigurera en Spara målgruppsaktivitet](../workflows/activities/save-audience.md)

1. När arbetsflödet är klart klickar du **[!UICONTROL Start]** för att genomföra det.

Arbetsflödet sparas i **[!UICONTROL Workflows]** -listan, medan de resulterande målgrupperna är tillgängliga i **[!UICONTROL Audiences]** lista. [Lär dig övervaka och hantera målgrupper](manage-audience.md)

Nu kan ni använda den här målgruppen som huvudmål för en leverans. [Läs mer](add-audience.md)

## Exempel på målgruppsarbetsflöde {#example}

I exemplet nedan visas ett målgruppsarbetsflöde som är konfigurerat för att rikta sig till kvinnliga kunder som bor i New York och skapa två nya målgrupper beroende på deras senaste köp (Yoga eller Löpande utrustning).

![](assets/audiences-example.png)

1. The **[!UICONTROL Build audience]** Aktiviteten riktar sig till alla kvinnliga profiler som bor i New York.
1. The **[!UICONTROL Enrichment]** aktiviteten berikar publiken med information från inköpstabellen för att identifiera vilken typ av produkt kunderna har köpt.
1. The **[!UICONTROL Split]** aktiviteten delar upp arbetsflödet i två banor baserat på kundens senaste köp.
1. The **[!UICONTROL Save audience]** aktiviteter i slutet av varje bana skapar två nya målgrupper i databasen, inklusive den population som beräknas i varje bana.
