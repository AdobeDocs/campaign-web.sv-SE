---
audience: end-user
title: Godkännande
description: Läs om samtycke på Adobe Campaign Web
badge: label="Begränsad tillgänglighet"
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 6%

---

# Hantera medgivande {#manage-consent}

## Allmänna rekommendationer {#general-recommendations}

Med Adobe Campaign kan ni samla in data, inklusive personuppgifter och känslig information. Det är viktigt att inhämta och övervaka samtycke från mottagare i enlighet med dataskyddsbestämmelser som GDPR (General Data Protection Regulation) och annan tillämplig integritetslagstiftning.

* Undvik först att skicka oönskade e-postmeddelanden, push-meddelanden och SMS-meddelanden (&quot;spam&quot;). Adobe stöder aktivt principerna om tillståndsmarknadsföring för att främja kundens livstidsvärde och lojalitet. Adobe förbjuder strikt användning av Adobe Campaign för att skicka oombedda meddelanden. [Läs mer](#denylisted-profiles)

* Se alltid till att mottagarna accepterar att ta emot meddelanden genom att ge dem möjlighet att välja bort från leveranserna <!-- and keep honoring opt-out requests as quickly as possible-->. [Läs mer](#opt-out)

* Använd prenumerationshanteringsprocessen för att hantera mottagarnas inställningar och spåra vilka mottagare som har valt att prenumerera på specifika typer. [Läs mer](../../delivery/using/about-services-and-subscriptions.md)

## Hantera avanmälan {#opt-out}

Att ge mottagarna möjlighet att avbryta prenumerationen på information från ett varumärke är ett juridiskt krav. Det är också nödvändigt att säkerställa att detta val respekteras. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html?lang=sv-SE#privacy-regulations){target="_blank"}.-->

**Varför är det viktigt?**

* Om ni inte följer dessa regler medför detta juridiska risker för ert varumärke.
* Det hjälper till att undvika att skicka oombedd kommunikation till mottagare, vilket kan leda till att de kan markera dina meddelanden som skräppost och skada ditt rykte.

Se till att kunderna kan avbryta prenumerationen när de skickar leveranser via Adobe Campaign Web. När prenumerationen har avbrutits tas profiler automatiskt bort från målgruppen för framtida marknadsföringsmeddelanden.

### Avanmäl dig via e-post {#email-opt-out}

Om du vill tillåta mottagarna att avbryta prenumerationen på e-postmeddelanden inkluderar du en **länk för att avbryta prenumerationen** i alla e-postmeddelanden som skickas till mottagarna.

Följ de här stegen:

1. Skapa en extern landningssida och placera den på valfritt tredjepartssystem.

1. Skapa en e-postleverans. [Lär dig hur](../email/create-email.md)

1. Infoga en länk i ditt e-postinnehåll. [Lär dig hur](../email/message-tracking.md#insert-links)

   ![Infoga länk i e-postinnehåll](../email/assets/message-tracking-insert-link.png)

1. Klistra in länken till tredjepartssidan i fältet **[!UICONTROL Url]**.

1. Klicka på ikonen **[!UICONTROL Links]** i den vänstra rutan om du vill visa en lista över alla URL:er i ditt innehåll som ska spåras.

1. Klicka på pennikonen bredvid den nya länken för att redigera den.

1. Ändra **[!UICONTROL Tracking Type]** och ställ in den på **[!UICONTROL Opt out]**.

   ![Redigera spårningstyp för avanmälan](../email/assets/message-tracking-edit-a-link.png)

1. Klicka på **[!UICONTROL Save]** och skicka meddelandet. [Läs mer](../monitor/prepare-send.md)

1. Om mottagaren klickar på länken för att avbryta prenumerationen visas din startsida när meddelandet har tagits emot.

1. När mottagaren skickar landningssidans formulär uppdateras profildata. [Läs mer](#denylisted-profiles)

<!--Any other option available such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Blocklist profiler {#denylisted-profiles}

Efter en avanmälan (avanmälan) läggs profiler till i **blockeringslista** för en viss kanal. Det innebär att de inte längre används av någon leverans.

>[!NOTE]
>
>Om en profil på blockeringslista för e-postkanalen har två e-postadresser, utesluts båda adresserna från leveransen.

Du kan kontrollera om det finns en profil på blockeringslista för en eller flera kanaler under **[!UICONTROL No longer contact]** på fliken **[!UICONTROL Details]** i profilen. [Läs mer](../audience/about-recipients.md#access)

![Kontrollera status för blockeringslista i profilinformation](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html?lang=sv-SE#feedback-loops){target="_blank"}.

Learn more about quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=sv-SE#non-deliverable-bounces){target="_blank"}.-->