---
audience: end-user
title: Godkännande
description: Läs om samtycke på Adobe Campaign Web
badge: label="Begränsad tillgänglighet"
source-git-commit: 9a184d7558ca39be3afed4a7217a5e5687799c0d
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 7%

---

# Hantera medgivande {#manage-consent}

## Allmänna rekommendationer {#general-recommendations}

Med Adobe Campaign kan ni samla in data, inklusive personuppgifter och känslig information. Det är därför viktigt att ni inhämtar och övervakar samtycke från era mottagare i enlighet med dataskyddsbestämmelser som GDPR (General Data Protection Regulation) och annan tillämplig sekretesslagstiftning.

* För det första ska du inte skicka e-post, push-meddelanden eller SMS-meddelanden (&quot;spam&quot;) som du inte har bett om. Adobe tror starkt på principerna om tillståndsmarknadsföring när det gäller att främja kundens livstidsvärde och lojalitet, och förbjuder därför strikt användning av Adobe Campaign för att skicka oönskade meddelanden. [Läs mer](#denylisted-profiles)

* Se alltid till att mottagarna accepterar att ta emot meddelanden genom att ge dem möjlighet att välja bort från leveranserna<!-- and keep honoring opt-out requests as quickly as possible-->. [Läs mer](#opt-out)

* Genom prenumerationshanteringen kan du hantera mottagarnas inställningar och spåra vilka mottagare som har valt vilken typ av prenumerationer du vill ha. [Läs mer](../../delivery/using/about-services-and-subscriptions.md)

## Hantera avanmälan {#opt-out}

Att ge mottagarna möjlighet att avbryta prenumerationen på information från ett varumärke är ett juridiskt krav, liksom att se till att detta val respekteras. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Varför är det viktigt?**

* Om ni inte följer dessa regler medför detta juridiska risker för ert varumärke.
* Det hjälper er att undvika att skicka oombedda meddelanden till era mottagare, vilket kan få dem att märka era meddelanden som skräppost och skada ert rykte.

När du skickar leveranser via Adobe Campaign Web måste du alltid se till att kunderna kan avbeställa dem från framtida kommunikation. När prenumerationen har avbrutits tas profilerna automatiskt bort från målgruppen för framtida marknadsföringsmeddelanden.

### Avanmäl dig via e-post {#email-opt-out}

Om du vill ge mottagarna möjlighet att avbryta prenumerationen på e-postmeddelanden måste du alltid inkludera en **avbeställ länk** i alla e-postmeddelanden som skickas till mottagarna.

Följ stegen nedan för att göra detta.

1. Skapa en extern landningssida och placera den på valfritt tredjepartssystem.

1. Skapa en e-postleverans. [Lär dig mer](../email/create-email.md)

1. Infoga en länk till ditt e-postinnehåll. [Lär dig mer](../email/message-tracking.md#insert-links)

   ![](../email/assets/message-tracking-insert-link.png)

1. I **[!UICONTROL Url]** klistra in länken till tredjepartssidan.

1. Klicka på **[!UICONTROL Links]** i den vänstra rutan för att visa en lista över alla URL:er för ditt innehåll som ska spåras.

1. Klicka på pennikonen bredvid den nya länken för att redigera den.

1. Ändra **[!UICONTROL Tracking Type]** och ange **[!UICONTROL Opt out]**.

   ![](../email/assets/message-tracking-edit-a-link.png)

1. Klicka **[!UICONTROL Save]** och skicka meddelandet. [Läs mer](../monitor/prepare-send.md)

1. Om mottagaren klickar på länken för att avbryta prenumerationen visas din startsida när meddelandet har tagits emot.

1. När mottagaren skickar landningssidans formulär uppdateras profildata. [Läs mer](#denylisted-profiles)

<!--Any other option availabe such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Blocklist profiler {#denylisted-profiles}

Efter en avanmälan (avanmälan) finns profilerna på **blockeringslista** för en viss kanal: detta innebär att de inte längre omfattas av någon leverans.

>[!NOTE]
>
>Om en profil på blockeringslista för e-postkanalen har två e-postadresser, kommer båda adresserna inte att levereras.

Du kan kontrollera om det finns en profil på blockeringslista för en eller flera kanaler i dialogrutan **[!UICONTROL No longer contact]** del av profilens **[!UICONTROL Details]** -fliken. [Läs mer](../audience/about-recipients.md#access)

![](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->



