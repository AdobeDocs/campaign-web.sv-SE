---
audience: end-user
title: Arbeta med arbetsflöden, kanalaktiviteter
description: Lär dig använda kanalaktiviteter i Adobe Campaign Web-arbetsflöden
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och köra marknadsföringskampanjer i flera kanaler, som e-post, SMS eller push. Med Adobe Campaign arbetsflöden kan du kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende.

Du kan till exempel skapa en välkomstkampanj för e-post som innehåller en serie meddelanden i olika kanaler, som e-post, SMS och push. Du kan också skicka ett uppföljningsmeddelande via e-post när en kund har slutfört ett köp eller skicka ett personligt födelsedagsmeddelande till en kund via SMS.

Genom att använda kanalaktiviteter kan ni skapa omfattande, personaliserade kampanjer som engagerar kunder över flera kontaktytor och driver konverteringar.

Kanalaktiviteter är tillgängliga från paletten, till vänster på skärmen, i avsnittet Kanaler.

## E-post {#email}

description, which use case you can perform (common other tasks that you can link before of after the activity)

lägga till och konfigurera aktiviteten

exempel på en konfigurerad aktivitet i ett arbetsflöde


Med aktiviteten för e-postleverans kan du konfigurera skickandet av ett e-postmeddelande i ett arbetsflöde.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

E-postmottagare definieras uppströms aktiviteten i samma arbetsflöde, via en målgruppsaktivitet.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->