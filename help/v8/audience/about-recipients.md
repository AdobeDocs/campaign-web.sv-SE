---
title: Arbeta med mottagare och målgrupper
description: Lär dig hur du arbetar med mottagare på Campaign Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 30786dd96dbe74c12d9af19d1c1b46b67e3d909d
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 1%

---

# Arbeta med mottagare och målgrupper {#about-recipients}

I Adobe Campaign är målgruppen en leverans en målgrupp. En målgrupp är en uppsättning personer som har liknande beteenden och/eller egenskaper. Den här samlingen personer kan antingen genereras, markeras eller läsas in [enligt nedan](#audiences). I de flesta fall består publiken av profiler som lagras som [mottagare](#recipients) i Adobe Campaign. Du kan även arbeta med andra målmappningar genom att ändra dimensionen enligt beskrivningen [i det här avsnittet](#targeting-dimensions).

## Vad är mottagare? {#recipients}


>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360-vy med dina mottagare"
>abstract="Skapa nya mottagare och övervaka dem med kraftfulla rapporter och verktyg. Få åtkomst till mottagarens attribut, interaktioner och loggar. Använd filtreringsalternativen för att bläddra i mottagarlistan, redigera och uppdatera deras profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Se versionsinformation"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiler"
>abstract="En profil är en individ som ska ta emot meddelanden från Adobe Campaign. I Adobe Campaign är mottagare standardprofiler för att skicka leveranser (e-post, SMS). I den här listan kan du visa mottagarens profil utifrån dina behörigheter. Använd filteralternativen för att bläddra i den här listan. Du kan redigera och uppdatera en liten uppsättning av mottagarens attribut."

En mottagare är en profil som är avsedd att ta emot meddelanden som skickas av Adobe Campaign. I Adobe Campaign är mottagarna de standardprofiler som väljs för att skicka leveranser till (e-post, SMS etc.). Med mottagardata som lagras i databasen kan du skapa målgrupper som tar emot alla angivna leveranser och lägga till personaliseringsdata i leveransinnehållet. Andra typer av profiler lagras i databasen. De är utformade för olika användningsområden: t.ex. skapas utsädesprofiler för att testa dina leveranser innan de skickas till den slutliga målgruppen.

Mottagare kan bara läggas till från Campaign-klientkonsolen. De visas dock på Campaign-webben från **Mottagare** inträde för det vänstra navigeringsfältet. Du kan också redigera mottagarens attribut från den skärmen.

Om du vill redigera mottagarens data klickar du på de tre punkterna bredvid namnet och väljer **Redigera...**.

![Redigera en mottagarprofil](assets/recipient-edit.png)

Du kan uppdatera en begränsad uppsättning attribut, till exempel förnamn, efternamn, e-postadress och telefonnummer.

![Uppdatera en mottagarprofil](assets/recipient-update.png)

>[!NOTE]
>
>Det här begränsade profilredigeringsformuläret finns endast för betatestning. Den kommer att förbättras i den framtida versionen. Det gör att användaren snabbt kan lägga till en e-postadress och ett telefonnummer till en profil så att han/hon kan testa e-post- och SMS-kanalerna och ta emot de meddelanden som skickas.

Du kan filtrera mottagarna med hjälp av sökfältet från **Visa filter** -knappen.

Du kan även komma åt mottagare från **Explorer** visa, bläddra och skapa mappar och undermappar och kontrollera tillhörande behörigheter.

![Mottagarlista från Utforskaren-vyn](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Beroende på dina behörigheter kanske du inte har tillgång till den fullständiga listan över mottagare som lagras i databasen. Läs mer om behörigheter i [det här avsnittet](../get-started/permissions.md).

Dessutom kan du hantera prenumerationen och avprenumerationen av dina mottagare på tjänster som nyhetsbrev. Lär dig hur du arbetar med prenumerationstjänster i [den här sidan](manage-services.md)

Du kan skapa arbetsflöden för att deduplicera, berika, kombinera profiler och bygga målgrupper. Läs mer i [det här avsnittet](../workflows/gs-workflows.md).

## Vad är målgrupper? {#audiences}

Målgruppen är huvudmålet för leveransen: mottagarna som tar emot meddelandena. Vilken typ av målgrupp det är beror på målmappningen som definieras i leveransmallen. Läs mer om leveransmallar i [den här sidan](../msg/delivery-template.md).

Om du vill definiera en målgrupps befolkning kan du:

* [Skapa nya målgrupper](create-audience.md) från **[!UICONTROL Audiences]** meny,
* [Välj en befintlig målgrupp](add-audience.md) som har skapats som en lista i klientkonsolen eller som kommer från Adobe Experience Platform,
* [Bygg en ny publik](segment-builder.md) med regelbyggaren genom att definiera och kombinera filtervillkor,
* [Använda en målgrupp från en extern fil](file-audience.md). Det här alternativet är bara tillgängligt för fristående e-postleveranser och kan inte användas i kampanjleveranser.

När ni riktar in er på en målgrupp kan ni också definiera **kontrollgrupper** för att undvika att skicka meddelanden till en del av er målgrupp och mäta effekten av era kampanjer. [Lär dig hur du ställer in en kontrollgrupp](control-group.md)

>[!NOTE]
>
>När meddelanden skickas i samband med ett kampanjarbetsflöde definieras målgruppen i en specifik **Bygg målgrupper** arbetsflödesaktivitet. I det här sammanhanget kan du inte läsa in en målgrupp från en fil för en e-postleverans, och målgruppen definieras endast i den här dedikerade aktiviteten. Lär dig definiera målgruppen för leveransen i ett kampanjarbetsflöde i [det här avsnittet](../workflows/activities/build-audience.md)

## Måldimensioner {#targeting-dimensions}

Målgruppsdimensionen, även kallad. målmappning, är den typ av data som hanteras av en åtgärd. Det gör att du kan definiera målpopulationen: mottagare, avtalspliktiga mottagare, operatörer, prenumeranter osv.

Måldimensionen för ett arbetsflöde definieras av den första **[!UICONTROL Build audience]** aktiviteten och används för alla andra aktiviteter fram till arbetsflödets slut. Om du till exempel gör en fråga till mottagarna från databasen, kommer den utgående övergången att innehålla data av typen mottagare och den kommer att överföras till nästa aktivitet.

Observera att du kan byta måldimension i ett arbetsflöde med en [Ändra dimensionsaktivitet](../workflows/activities/change-dimension.md). Detta gör att du till exempel kan ställa frågor till databasen i en viss tabell, som inköp eller prenumerationer, och sedan ändra måldimensionen till mottagare för att skicka leveranser till motsvarande mottagare.

Som standard har mallar för e-post och SMS-leverans som mål **[!UICONTROL Recipients]**. Måldimensionen använder därför fälten i **nms:mottagare** tabell. Standardmåldimensionen för push-meddelanden är **Prenumerationsprogram nms:appSubscriptionRcp**, som är länkad till mottagartabellen.

Du kan även använda andra inbyggda målmappningar i dina arbetsflöden och leveranser som listas nedan:

| Namn | Använd för | Schema |
|---|---|---|
| Mottagare | Leverera till mottagare (inbyggd mottagartabell) | nms:mottagare |
| Besökare | Leverera till besökare vars profiler har samlats in via hänskjutning (viral marketing) för ex. | mns:besökare |
| Prenumerationer | Leverera till mottagare som prenumererar på en informationstjänst som ett nyhetsbrev | nms:prenumeration |
| Prenumerationer på besökare | Skicka till besökare som prenumererar på en informationstjänst | nms:visitorSub |
| Operatorer | Leverera till Adobe Campaign | nms:operator |
| Extern fil | Leverera via en fil som innehåller all information som behövs för leveransen | Inget länkat schema, inget mål har angetts |
| Prenumerationsprogram | Leverera till mottagare som prenumererar på ett program | nms:appSubscriptionRcp |

Dessutom kan du skapa en ny målmappning beroende på dina behov. Detta görs från klientkonsolen. Läs mer i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
