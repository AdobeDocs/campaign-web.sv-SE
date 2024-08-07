---
audience: end-user
title: Använd en leveransarbetsflödesaktivitet
description: Lär dig hur du lägger till en leveransarbetsflödesaktivitet (e-post, push, SMS, direktreklam)
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: 298b1e17e70eae7da98fd5ac60fbcad32ce5c44f
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 1%

---

# E-post, SMS, push, direktreklam {#channel}

Med Adobe Campaign Web kan ni automatisera och genomföra marknadsföringskampanjer via e-post, SMS, direktreklam och push-kanaler. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende och data.

Du kan till exempel skapa en välkomstkampanj för e-post som innehåller en serie meddelanden i olika kanaler, som e-post, SMS, push och direktreklam. Du kan också skicka ett uppföljningsmeddelande via e-post när en kund har slutfört ett köp eller skicka ett personligt födelsedagmeddelande till en kund via SMS.

Genom att använda kanalaktiviteter kan ni skapa omfattande och personaliserade kampanjer som engagerar kunder över flera kontaktytor och driver konverteringar.

>[!NOTE]
>
>Du kan också skapa en engångsleverans, utanför ramen för ett kampanjarbetsflöde. Läs mer i följande avsnitt:
>* [Skapa fristående e-postleverans](../../email/create-email.md)
>* [Skapa fristående SMS-leverans](../../sms/create-sms.md)
>* [Skapa fristående push-leverans](../../push/create-push.md)
>* [Skapa fristående direktutskick](../../direct-mail/create-direct-mail.md)

## Förhandskrav {#channel-activity-prereq}

Bygg upp arbetsflödet med relevanta aktiviteter:

* Innan du infogar en kanalaktivitet måste du definiera målgruppen. Målgruppen är huvudmålet för leveransen: de profiler som tar emot meddelandena. När du skickar meddelanden i ett kampanjarbetsflöde definieras inte meddelandemålgruppen i kanalaktiviteten, utan i en dedikerad aktivitet, till exempel:

   * En **Skapa målgruppsaktivitet**. [Läs mer](build-audience.md).

     ![](../../msg/assets/add-delivery-in-wf.png)

   * En **Läs in fil**-aktivitet följd av en **avstämningsaktivitet**. [Läs mer](load-file.md).

     ![](../assets/workflow-reconciliation-criteria.png)

* Om du vill skicka en återkommande leverans startar du arbetsflödet med en **schemaläggaraktivitet**. Du kan också använda en **schemaläggaraktivitet** för engångsleveranser för att ange kontaktdatum för den leveransen. Kontaktdatumet kan även anges i leveransinställningarna. Se [det här avsnittet](scheduler.md).

## Konfigurera kanalaktiviteten {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="E-postaktivitet"
>abstract="E-postaktiviteten underlättar e-postutskick i ditt arbetsflöde och gör det möjligt att skicka både enstaka och återkommande meddelanden. Den automatiserar processen för att skicka e-post till ett mål som beräknas inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS-aktivitet"
>abstract="SMS-aktiviteten underlättar SMS-utskick inom ditt arbetsflöde och gör det möjligt att skicka både engångs- och återkommande meddelanden. Den automatiserar processen för att skicka SMS till ett mål som beräknas inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Push iOS activity"
>abstract="Push iOS-aktiviteten effektiviserar processen att skicka iOS Push-meddelanden som en del av ditt arbetsflöde. Det gör det möjligt att leverera både engångs- och återkommande meddelanden, och automatiserar utskicksmeddelandena från iOS Push till ett fördefinierat mål inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Push Android activity"
>abstract="Push Android-aktiviteten effektiviserar processen att skicka Android Push-meddelanden som en del av ditt arbetsflöde. Det gör det möjligt att leverera både engångs- och återkommande meddelanden, och automatiserar utskicksmeddelandena från Android Push till ett fördefinierat mål inom samma arbetsflöde. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende och data."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Aktivitet för direktreklam"
>abstract="Med aktiviteten Direktreklam blir det enklare att skicka direktreklam i arbetsflödet, vilket möjliggör både engångs- och återkommande meddelanden. Den automatiserar processen för att generera extraheringsfilen som krävs av direktreklamleverantörer. Du kan kombinera kanalaktiviteter i arbetsytan för arbetsflöden för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende och data."

Följ stegen nedan för att konfigurera en leverans i ett arbetsflödes sammanhang:

1. Lägg till en kanalaktivitet: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]**, **[!UICONTROL Push notification (iOS)]** eller **[!UICONTROL Direct mail]**.

1. Välj **Typ av leverans**: enkel eller återkommande.

   * En **enskild leverans** är en engångsleverans, som bara skickas en gång, till exempel ett svartvitt e-postmeddelande på fredag.
   * En **återkommande leverans** skickas flera gånger baserat på dess körningsfrekvens som definierats i en [schemaläggaraktivitet](scheduler.md). Varje gång arbetsflödet körs beräknas målgruppen om och leveransen skickas till den uppdaterade målgruppen med det uppdaterade innehållet. Det här kan till exempel vara ett veckonyhetsbrev eller ett återkommande födelsedagskalender.

1. Välj en **leveransmall**. Mallar är förkonfigurerade leveransinställningar som är specifika för en kanal. En inbyggd mall är tillgänglig för varje kanal och förfylld som standard. [Läs mer](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)

   Du kan välja mallen i det vänstra fönstret för kanalaktivitetskonfigurationen. Om den tidigare valda publiken inte är kompatibel med kanalen kan du inte välja en mall. Du löser detta genom att uppdatera aktiviteten **Bygg målgrupp** och välja en målgrupp med rätt målmappning. Läs mer om målmappningar i [det här avsnittet](../../audience/targeting-dimensions.md)

1. Klicka på **Skapa leverans**. Du kan sedan definiera meddelandeinställningar och innehåll på samma sätt som du skapar en fristående leverans. Du kan också testa och simulera innehållet. [Läs mer](../../msg/gs-messages.md)

1. Gå tillbaka till arbetsflödet. Om du vill fortsätta med arbetsflödet växlar du till alternativet **Generera en utgående övergång** för att lägga till en övergång efter kanalaktiviteten.

1. Klicka på **Start** för att starta arbetsflödet.

   Som standard utlöses meddelandeförberedelsefasen när ett arbetsflöde startas, utan att meddelandet skickas omedelbart.

1. Öppna din kanalaktivitet för att bekräfta sändningen från knappen **Granska och skicka**.

1. Klicka på **Skicka** på kontrollpanelen för leverans.

## Exempel {#cross-channel-workflow-sample}

Här är ett exempel på flerkanaligt arbetsflöde med segmentering och två leveranser. Arbetsflödet riktar sig till alla kunder som bor i Paris och som är intresserade av kaffemaskiner. Bland de här befolkningsgrupperna skickas ett e-postmeddelande till de vanliga kunderna och ett SMS skickas till de VIP klienterna.

![](../assets/workflow-channel-example.png)

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->

Du kan också skapa ett återkommande arbetsflöde för att skicka ett personaliserat SMS varje dag i månaden kl. 20.00 till alla kunder i Paris.

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
