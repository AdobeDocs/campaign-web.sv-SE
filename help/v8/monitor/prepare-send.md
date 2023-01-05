---
audience: end-user
title: Förbered och skicka ett e-postmeddelande
description: Webbdokumentation för Campaign v8
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 75d579975023639840f35f673e63aab2a2d3a811
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 4%

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

## Förbered sändningen{#prepare}

När ni har definierat ert innehåll, er målgrupp och ert schema är ni redo att ta fram ert budskap. Under beredningen beräknas målpopulationen och meddelandeinnehållet genereras för varje profil som ingår i målet. När färdigställandet är klart är meddelandena klara att skickas, antingen omedelbart eller vid det schemalagda datumet och klockslaget. Valideringsreglerna som används vid analysen beskrivs i detta [section](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies).

Följ stegen nedan:

1. Klicka på **Förbered** i det övre högra hörnet och bekräfta.

   ![](assets/prepare.png)

   Förberedelseförloppet visas. Beroende på storleken på målpopulationen kan den här åtgärden ta en stund.

   >[!NOTE]
   >
   >Du kan när som helst avbryta beredningen med **Stoppa förberedelse** -knappen. Under beredningsfasen skickas inga meddelanden. Du kan därför starta eller stoppa detta utan risk för att påverka något.

1. Kontrollera KPI:erna när färdigställandet är klart. Om antalet meddelanden som ska skickas inte matchar dina förväntningar ändrar du målgruppen och startar om förberedelsen.

   ![](assets/prepare2.png)

   Här visas olika KPI:er:

   * **Målinriktad**: antalet mottagare
   * **Att leverera**: antalet meddelanden som ska skickas
   * **Att exkludera**: antalet meddelanden som utelämnats av en typologiregel

1. Klicka på **Loggar** och kontrollera att det inte finns något fel. I det sista loggmeddelandet visas eventuella felmeddelanden och antalet fel. Mer information finns i [det här avsnittet](#send).

   ![](assets/prepare-logs.png)

Om ett kritiskt fel upptäcks som förhindrar att leveransen skickas, visas statusen för förberedelsen som misslyckad på kontrollpanelen för leverans.

![](assets/prepare-error.png)

Om du behöver göra några ändringar i leveransen efter färdigställandet måste du starta om preparatet för att dessa ändringar ska beaktas.

När färdigställandet är klart utan fel är ditt meddelande klart att skickas. Mer information finns i [det här avsnittet](#send).

## Skicka meddelandet{#send}

När färdigställandet är klart kan du nu skicka ditt meddelande. Det här steget krävs bara för meddelanden som skickas omedelbart. Om meddelandet är schemalagt skickas det vid angivet datum.

Följ de här stegen:

1. Klicka på **Skicka** i det övre högra hörnet och bekräfta.

   ![](assets/send.png)

1. Sändningsförloppet visas. Kontrollera de KPI:er som visas. Du kan också kontrollera loggarna. Mer information finns i [det här avsnittet](#send).

   ![](assets/send2.png)

   Här visas olika KPI:er:

   * **Levererat**: antalet meddelanden som har skickats. Procentandelen baseras på det totala antalet målmottagare.
   * **Öppnar**: antalet öppnade meddelanden. Procentandelen baseras på antalet levererade meddelanden.
   * **Klickningar**: antalet mottagare som klickade minst en gång i e-postmeddelandet. Procentandelen baseras på antalet levererade meddelanden.

   >[!NOTE]
   >
   >The **Öppnar** och **Klickningar** kommer att uppdateras i realtid.

   Du kan när som helst pausa sändningen och sedan återuppta den. Om du avbryter leveransen medan den skickas kan du inte återuppta den.
