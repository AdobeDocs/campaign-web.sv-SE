---
audience: end-user
title: Skapa målgrupper
description: Lär dig skapa målgrupper i Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 2890e5b19cb9b668f3f429cf60dbfd98278b3649
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# Skapa målgrupper {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Målgrupper"
>abstract="Från den här skärmen kan du komma åt listan över alla målgrupper som kan användas i arbetsflöden eller fristående leveranser. Klicka på **Skapa** för att skapa en ny målgrupp på en visuell arbetsyta.<br/><br/>Förutom att börja från början och skapa en enkel målgrupp kan du också utnyttja arbetsflödesaktiviteter för att förfina målgruppen. Ni kan till exempel kombinera flera olika målgrupper till en enda, berika er målgrupp med externa attribut eller dela in den i flera målgrupper baserat på valfria regler."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

## Om målgruppsgenerering

Med Campaign Web kan ni skapa nya målgrupper i ett visuellt arbetsflöde. Förutom att börja från scratch och skapa en enkel målgrupp kan ni också utnyttja arbetsflödesaktiviteter för att förfina er målgrupp. Ni kan till exempel kombinera flera olika målgrupper till en enda, berika er målgrupp med externa attribut eller dela in den i flera målgrupper baserat på valfria regler.

När ni väl utformat ert arbetsflöde lagras de resulterande målgrupperna automatiskt i Campaign-databasen tillsammans med era befintliga. Dessa målgrupper kan sedan målgruppsanpassas i arbetsflöden eller fristående leveranser.

Kolumnen **[!UICONTROL Origin]** anger målgruppernas ursprung: **[!UICONTROL Adobe Campaign]** målgrupper skapas i Adobe Campaign v8-konsolen eller webbanvändargränssnittet, medan **[!UICONTROL Adobe Experience Platform:]** målgrupper skapas i Adobe Experience Platform och integreras i Campaign med hjälp av Adobe-integreringen Källor och Destinationer.

➡️ [Upptäck den här funktionen i en video](#video)

## Behörigheter för anpassade operatorgrupper

När du skapar en ny målgrupp skapas ett arbetsflöde automatiskt och lagras i mappen **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Jobs]** / **[!UICONTROL Targeting workflows]** .

Om du har tilldelats en anpassad operatörsgrupp och råkar ut för felet&quot;Du saknar behörighet&quot; när du skapar målgrupper, måste du se till att operatörsgruppen har de behörigheter som krävs för den här mappen.

För att lösa detta måste en administratör lägga till din anpassade operatörsgrupp i mappsäkerhetssektionen i Campaign-konsolen. [Lär dig hantera behörigheter för mappar](../get-started/permissions.md#folder-permissions)

## Skapa din första målgrupp {#create}

Så här skapar du en målgrupp:

1. Navigera till menyn **[!UICONTROL Audiences]** och klicka på knappen **[!UICONTROL Create Audience]** i det övre högra hörnet.

1. Ett nytt arbetsflöde skapas automatiskt så att du kan kombinera aktiviteter för att skapa en målgrupp. Arbetsytan innehåller som standard två huvudaktiviteter:

   * Aktiviteten Fråga **[!UICONTROL Build audience]** är startpunkten i ditt arbetsflöde. Det gör att ni kan skapa en målgrupp och använda den som grund för ert arbetsflöde.

   * Aktiviteten Ny målgrupp **[!UICONTROL Save audience]** representerar det sista steget i ditt arbetsflöde. Det gör att ni kan spara resultaten som en ny publik.

   ![En tom arbetsyta för målgruppsskapande med två standardaktiviteter: Skapa målgrupp och Spara målgrupp.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >Målgruppsarbetsflöden lagras på menyn **Arbetsflöden**, tillsammans med dina andra Campaign-arbetsflöden. De är särskilt utformade för att skapa målgrupper och kan identifieras med hjälp av deras vertikala arbetsyta.

1. För bättre läsbarhet kan du ändra arbetsflödets namn i fältet **Etikett** i arbetsflödesinställningarna. [Lär dig hur du konfigurerar arbetsflödesinställningar](../workflows/workflow-settings.md)

1. Öppna aktiviteten **[!UICONTROL Build audience]** och använd frågemodelleraren för att definiera populationen som ska inkluderas i målgruppen genom att filtrera data i databasen. [Lär dig konfigurera en målgruppsaktivitet](../workflows/activities/build-audience.md)

1. Om du vill utföra ytterligare åtgärder för den målgrupp som arbetsflödet är avsett för, lägger du till så många aktiviteter som behövs och kopplar ihop dem. Mer information om hur du konfigurerar arbetsflödesaktiviteter finns i [arbetsflödesdokumentationen](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktiviteter är inte tillgängliga för målgruppsarbetsflöden.

   ![En målgruppsarbetsyta med flera aktiviteter anslutna för att förfina målgruppen.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Konfigurera aktiviteten **[!UICONTROL Save audience]** för att ange hur du vill spara den beräknade populationen uppströms i arbetsflödet. [Lär dig hur du konfigurerar en Spara målgruppsaktivitet](../workflows/activities/save-audience.md)

1. När arbetsflödet är klart klickar du på **[!UICONTROL Start]** för att köra det.

Arbetsflödet sparas i listan **[!UICONTROL Workflows]**, medan målgruppen/målgrupperna är tillgängliga i listan **[!UICONTROL Audiences]** med etiketten som definierats i aktiviteten **Spara målgrupp**. Lär dig övervaka och hantera målgrupper i [det här avsnittet](manage-audience.md)

Nu kan ni använda den här målgruppen som huvudmål för en leverans. [Läs mer](add-audience.md)

## Exempel på målgruppsarbetsflöde {#example}

I exemplet nedan visas ett målgruppsarbetsflöde som är konfigurerat för att rikta sig till kvinnliga kunder som bor i New York och skapa två nya målgrupper beroende på deras senaste köp (Yoga eller Löpande utrustning).

![Ett exempel på målgruppsarbetsflöde som riktar sig till kvinnliga kunder i New York och delar upp dem baserat på deras senaste köp.](assets/audiences-example.png){zoomable="yes"}

1. Aktiviteten **[!UICONTROL Build audience]** har alla kvinnliga profiler som bor i New York som mål.
1. Aktiviteten **[!UICONTROL Enrichment]** förbättrar publiken med information från inköpstabellen för att identifiera vilken typ av produkt kunderna har köpt.
1. Aktiviteten **[!UICONTROL Split]** delar upp arbetsflödet i två sökvägar baserat på kundens senaste köp.
1. **[!UICONTROL Save audience]**-aktiviteterna i slutet av varje sökväg skapar två nya målgrupper i databasen, inklusive populationen som beräknas i varje sökväg.

## Redigera en målgrupp {#edit}

Du kan ändra en målgrupp som genererats från ett arbetsflöde när det behövs genom att köra motsvarande arbetsflöde igen. På så sätt kan ni uppdatera målgruppsdata eller förfina målgruppen genom att anpassa frågan efter era behov.

1. Navigera till menyn **Publiker** och öppna den målgrupp du vill redigera.
1. På fliken **Översikt** tillhandahåller avsnittet **Senaste arbetsflöde** en länk till arbetsflödet som används för att generera målgruppen. Klicka på den för att komma åt arbetsflödet.
1. Gör önskade ändringar och klicka på knappen **Start** för att köra arbetsflödet igen. När arbetsflödet är klart uppdateras målgruppen automatiskt med de senaste arbetsflödesresultaten.

Som standard ersätts hela målgruppens innehåll med nya data när du kör ett målgruppsarbetsflöde, vilket leder till att tidigare data går förlorade.

Om du inte vill ersätta de befintliga målgruppsresultaten konfigurerar du **Spara målgruppsaktiviteterna** så att de passar dina behov. Du kan till exempel ändra fältet **Målgruppsetikett** för att lagra de nya resultaten hos en ny målgrupp eller lägga till de nya resultaten i det befintliga målgruppsinnehållet utan att radera tidigare data. [Lär dig hur du konfigurerar en Spara målgruppsaktivitet](../workflows/activities/save-audience.md)

![Konfigurationsskärmen Spara målgruppsaktivitet med alternativ för att justera målgruppssparande.](assets/edit-audience-save.png){zoomable="yes"}

## Instruktionsvideo {#video}

Lär dig hur du bygger och hanterar målgrupper, hur du väljer målgrupper för en leverans och definierar kontrollgrupper.

>[!VIDEO](https://video.tv.adobe.com/v/3453206?captions=swe&quality=12)