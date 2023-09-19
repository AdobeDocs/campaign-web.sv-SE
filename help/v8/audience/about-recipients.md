---
title: Arbeta med mottagare och målgrupper
description: Lär dig hur du arbetar med mottagare på Campaign Web
badge: label="Beta"
source-git-commit: 269cbb51f070b0f9f771691497ffa07bb94e2d49
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 2%

---


# Arbeta med mottagare och målgrupper {#about-recipients}

## Mottagare {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Mottagare"
>abstract="En mottagare är en profil som är avsedd att ta emot meddelanden som skickas av Adobe Campaign. I Adobe Campaign är mottagare standardprofiler för att skicka leveranser (e-post, SMS). I den här listan kan du visa mottagarens profil utifrån dina behörigheter. Använd filteralternativen för att bläddra i den här listan. Du kan redigera och uppdatera en liten uppsättning av mottagarens attribut."

En mottagare är en profil som är avsedd att ta emot meddelanden som skickas av Adobe Campaign. I Adobe Campaign är mottagarna de standardprofiler som väljs för att skicka leveranser till (e-post, SMS etc.). Med mottagardata som lagras i databasen kan du skapa målgrupper som tar emot alla angivna leveranser och lägga till personaliseringsdata i leveransinnehållet. Andra typer av profiler lagras i databasen. De är utformade för olika användningsområden: t.ex. skapas utsädesprofiler för att testa dina leveranser innan de skickas till den slutliga målgruppen.

Mottagare kan bara läggas till från Campaign-klientkonsolen. De visas dock på Campaign-webben från **Mottagare** inträde för det vänstra navigeringsfältet.

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

Dessutom kan du hantera prenumerationen och avprenumerationen av dina mottagare på tjänster som nyhetsbrev. [Lär dig arbeta med prenumerationstjänster](create-service.md)

## Målgrupper {#audiences}

Målgruppen är huvudmålet för leveransen: mottagarna som tar emot meddelandena. Vilken typ av målgrupp det är beror på målmappningen som definieras i leveransmallen. [Lär dig vad som är en leveransmall](../msg/delivery-template.md).

Om du vill definiera en målgrupps befolkning kan du:

* [Skapa nya målgrupper](create-audience.md) från **[!UICONTROL Audiences]** meny,
* [Välj en befintlig målgrupp](add-audience.md) skapat som en lista i klientkonsolen,
* [Välja en Adobe Experience Platform-målgrupp](aep-audience.md),
* [Bygg en ny publik](segment-builder.md) med regelbyggaren genom att definiera och kombinera filtervillkor,
* [Använda en målgrupp från en extern fil](file-audience.md). Det här alternativet är bara tillgängligt för fristående e-postleveranser och kan inte användas i kampanjleveranser.

När ni riktar in er på en målgrupp kan ni också definiera **kontrollgrupper** för att undvika att skicka meddelanden till en del av er målgrupp och mäta effekten av era kampanjer. [Lär dig hur du ställer in en kontrollgrupp](control-group.md)

>[!NOTE]
>
>När meddelanden skickas i samband med ett kampanjarbetsflöde definieras målgruppen i en specifik **Bygg målgrupper** arbetsflödesaktivitet. I det här sammanhanget kan du inte läsa in en målgrupp från en fil för en e-postleverans, och målgruppen definieras endast i den här dedikerade aktiviteten. Lär dig definiera målgruppen för leveransen i ett kampanjarbetsflöde [i det här avsnittet](../workflows/activities/build-audience.md)
