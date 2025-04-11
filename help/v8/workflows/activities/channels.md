---
audience: end-user
title: Använd en leveransarbetsflödesaktivitet
description: Lär dig hur du lägger till en leveransarbetsflödesaktivitet (e-post, push, SMS, direktreklam)
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# E-post, SMS, push, direktreklam {#channel}

Med Adobe Campaign Web kan ni automatisera och genomföra marknadsföringskampanjer via e-post, SMS, direktreklam och push-kanaler. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende och data.

Skapa till exempel en välkomstkampanj för e-post som innehåller en serie meddelanden över olika kanaler, som e-post, SMS, push och direktreklam. Du kan också skicka ett uppföljningsmeddelande via e-post när en kund har slutfört ett köp eller skicka ett personligt födelsedagmeddelande till en kund via SMS.

Genom att använda kanalaktiviteter kan du skapa omfattande och personaliserade kampanjer som engagerar kunder över flera kontaktytor och driver konverteringar.

>[!NOTE]
>
>Du kan också skapa en engångsleverans utanför ett kampanjarbetsflöde. Läs mer i följande avsnitt:
>* [Skapa fristående e-postleverans](../../email/create-email.md)
>* [Skapa fristående SMS-leverans](../../sms/create-sms.md)
>* [Skapa fristående push-leverans](../../push/create-push.md)
>* [Skapa fristående direktutskick](../../direct-mail/create-direct-mail.md)

## Förhandskrav {#channel-activity-prereq}

Bygg upp arbetsflödet med relevanta aktiviteter:

* Definiera målgruppen innan du infogar en kanalaktivitet. Målgruppen är huvudmålet för leveransen: de profiler som tar emot meddelandena. När du skickar meddelanden i ett kampanjarbetsflöde definieras inte meddelandemålgruppen i kanalaktiviteten utan i en dedikerad aktivitet, till exempel:

   * En **Skapa målgruppsaktivitet**. [Läs mer](build-audience.md).

     ![Skärmbild som visar tillägg av en leverans i ett arbetsflöde](../../msg/assets/add-delivery-in-wf.png)

   * En **Läs in fil**-aktivitet följd av en **avstämningsaktivitet**. [Läs mer](load-file.md).

     ![Skärmbild som visar villkor för arbetsflödesavstämning](../assets/workflow-reconciliation-criteria.png)

* Om du vill skicka en återkommande leverans startar du arbetsflödet med en **schemaläggaraktivitet**. Använd en **schemaläggaraktivitet** för engångsleveranser för att ange kontaktdatum för den leveransen. Kontaktdatumet kan även anges i leveransinställningarna. Se [det här avsnittet](scheduler.md).

## Konfigurera kanalaktiviteten {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="E-postaktivitet"
>abstract="E-postaktiviteten underlättar e-postutskick i ditt arbetsflöde och gör det möjligt att skicka både enstaka och återkommande meddelanden. Det automatiserar processen för att skicka e-post till ett mål som beräknas inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS-aktivitet"
>abstract="SMS-aktiviteten underlättar SMS-utskick inom ditt arbetsflöde och gör det möjligt att skicka både engångs- och återkommande meddelanden. Det automatiserar processen för att skicka SMS till ett mål som beräknas inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Push iOS activity"
>abstract="Push iOS-aktiviteten effektiviserar processen att skicka iOS Push-meddelanden som en del av ditt arbetsflöde. Det gör det möjligt att leverera både engångs- och återkommande meddelanden, och automatiserar sändningen av iOS Push-meddelanden till ett fördefinierat mål inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Push Android activity"
>abstract="Push Android-aktiviteten effektiviserar processen att skicka Android Push-meddelanden som en del av ditt arbetsflöde. Det gör det möjligt att leverera både engångs- och återkommande meddelanden, och automatiserar sändningen av Android Push-meddelanden till ett fördefinierat mål inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Aktivitet för direktreklam"
>abstract="Med aktiviteten Direktreklam blir det enklare att skicka direktreklam i arbetsflödet, vilket möjliggör både engångs- och återkommande meddelanden. Det automatiserar processen för att generera extraheringsfilen som krävs av direktreklamleverantörer. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som triggar åtgärder baserat på kundbeteende och data."

Följ stegen nedan för att konfigurera en leverans i ett arbetsflödes sammanhang:

1. Lägg till en kanalaktivitet: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]**, **[!UICONTROL Push notification (iOS)]** eller **[!UICONTROL Direct mail]**.

1. Välj **Typ av leverans**: enkel eller återkommande.

   * En **enskild leverans** är en engångsleverans som bara skickas en gång, till exempel ett svartvitt e-postmeddelande på fredag.
   * En **återkommande leverans** skickas flera gånger baserat på dess körningsfrekvens som definierats i en [schemaläggaraktivitet](scheduler.md). Varje gång arbetsflödet körs beräknas målgruppen om och leveransen skickas till den uppdaterade målgruppen med det uppdaterade innehållet. Det här kan vara ett veckonyhetsbrev eller ett återkommande födelsedagskalender.

1. Välj en **leveransmall**. Mallar är förkonfigurerade leveransinställningar som är specifika för en kanal. En inbyggd mall är tillgänglig för varje kanal och förfylld som standard. [Läs mer](../../msg/delivery-template.md)

   ![Skärmbild som visar leveransaktivitet i ett arbetsflöde](../assets/delivery-activity-in-wf.png)

   Välj mallen i det vänstra fönstret för kanalaktivitetskonfigurationen. Om den tidigare valda publiken inte är kompatibel med kanalen kan du inte välja en mall. Du löser detta genom att uppdatera aktiviteten **Bygg målgrupp** och välja en målgrupp med rätt målmappning. Läs mer om målmappningar i [det här avsnittet](../../audience/targeting-dimensions.md).

1. Klicka på **Skapa leverans**. Definiera meddelandeinställningar och innehåll på samma sätt som du skapar en fristående leverans. Testa och simulera innehållet. [Läs mer](../../msg/gs-messages.md)

1. Gå tillbaka till arbetsflödet. Om du vill fortsätta med ditt arbetsflöde växlar du till alternativet **Generera en utgående övergång** och lägger till en övergång efter kanalaktiviteten.

1. Klicka på **Start** för att starta arbetsflödet.

   Som standard utlöses meddelandeförberedelsefasen utan att meddelandet skickas omedelbart när ett arbetsflöde startas.

1. Öppna din kanalaktivitet för att bekräfta sändningen från knappen **Granska och skicka**.

1. Klicka på **Skicka** på kontrollpanelen för leverans.

## Exempel {#cross-channel-workflow-sample}

Här är ett exempel på flerkanaligt arbetsflöde med segmentering och två leveranser. Arbetsflödet riktar sig till alla kunder som bor i Paris och är intresserade av kaffemaskiner. Bland dessa personer skickas ett e-postmeddelande till vanliga kunder och ett SMS skickas till VIP-kunder.

![Skärmbild som visar ett exempel på flerkanalsarbetsflöde](../assets/workflow-channel-example.png)

Du kan också skapa ett återkommande arbetsflöde för att skicka ett personaliserat SMS varje dag i månaden kl. 20.00 till alla kunder i Paris.

![Skärmbild som visar ett exempel på återkommande arbetsflöde](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->