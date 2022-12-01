---
audience: end-user
title: Förbered och skicka ett e-postmeddelande
description: Webbdokumentation för Campaign v8
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 2%

---

# Förbered och skicka e-post {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Förbered och skicka e-post"
>abstract="Upptäck hur du förbereder e-postmeddelandet och lär dig mer om hur du skickar nyckeltal."

>[!NOTE]
>
>Dokumentationen håller på att byggas och uppdateras ofta. Den slutliga versionen av detta innehåll är klar i januari 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Förbered sändningen

Under beredningen beräknas målpopulationen och meddelandeinnehållet genereras för varje profil som ingår i målet. När färdigställandet är klart är meddelandena klara att skickas, antingen omedelbart eller vid det schemalagda datumet och klockslaget. Valideringsreglerna som används vid analysen beskrivs i detta [section](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Klicka på **Förbered** i det övre högra hörnet.

1. Förberedelseförloppet visas. Beroende på storleken på målpopulationen kan den här åtgärden ta en stund.

   >[!NOTE]
   >
   >Du kan när som helst avbryta beredningen med **Stoppa förberedelse** -knappen. Under beredningsfasen skickas inga meddelanden. Du kan därför starta eller stoppa detta utan risk för att påverka något.

1. När färdigställandet är klart ska du kontrollera **Målinriktad**, **Att leverera** och **Att exkludera** KPI:er. Om antalet meddelanden som ska skickas inte matchar dina förväntningar ändrar du målgruppen och startar om förberedelsen.

1. Klicka på **Loggar** och kontrollera att det inte finns något fel. Alla valideringssteg, varningar och fel visas. Färgade ikoner visar meddelandetypen:

   * Den grå ikonen visar ett informativt meddelande.
   * Den gula ikonen indikerar ett icke-kritiskt bearbetningsfel.
   * Den röda ikonen anger ett kritiskt fel som förhindrar leverans.

1. Starta om preparatet när du har gjort ändringarna.

När färdigställandet är klart är ditt meddelande klart att skickas. Mer information finns i Bekräfta sändning.


## Skicka meddelandet

När färdigställandet är klart följer du stegen nedan för att skicka meddelandet.

1. Klicka på **Skicka-knapp** i det övre högra hörnet och bekräfta.

1. Sändningsförloppet visas tillsammans med tre nyckeltal: Levererat, öppnar, klickar.

1. Slutför sändningen genom att klicka på OK.

LOGGAR

>[!NOTE]
>
>Om meddelandet är schemalagt skickas det när sändningstiden nås. Mer information om roller finns i detta avsnittet.

