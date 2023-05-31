---
audience: end-user
title: Använd aktiviteten för e-postarbetsflöde
description: Lär dig hur du använder arbetsflödesaktiviteten för e-post
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 1%

---


# E-post {#email}

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
