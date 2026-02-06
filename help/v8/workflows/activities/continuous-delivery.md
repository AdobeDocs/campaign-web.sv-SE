---
audience: end-user
title: Använd en kontinuerlig arbetsflödesaktivitet för leverans
description: Lär dig hur du använder arbetsflödesaktiviteten Kontinuerlig leverans
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Kontinuerlig leverans {#continuous-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Kontinuerlig leveransaktivitet"
>abstract="Nu kan du lägga till nya mottagare till en befintlig leverans. Med den här leveranstypen slipper du skapa en ny leverans varje gång, vilket gör den mer effektiv för meddelanden med låg volym eller meddelanden som skickas efter behov."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=sv-SE" text="Se versionsinformation"

Med aktiviteten **Kontinuerlig leverans** kan du lägga till nya mottagare till en befintlig leverans. Med den här leveranstypen slipper du skapa en ny leverans varje gång, vilket gör den mer effektiv för meddelanden med låg volym eller meddelanden som skickas efter behov.

En kontinuerlig leverans skapar en enda leveransinstans. Alla leveransloggar (broadLog) och spårningsloggar refererar till denna enda leverans, vilket förenklar övervakning och rapportering.

## Konfigurera aktiviteten Kontinuerlig leverans {#configure}

1. Lägg till en **kontinuerlig**-aktivitet på arbetsytan.

   ![Skärmbild som visar kontinuerlig leveransaktivitet](../assets/continuous-delivery.png){zoomable="yes"}

1. Ange en anpassad **[!UICONTROL Label]** för aktiviteten (valfritt). Som standard heter den&quot;Kontinuerlig leverans&quot;.

1. Klicka på sökikonen bredvid fältet **[!UICONTROL Template]** för att välja en leveransmall. Det går bara att välja mallar (inte standardleveranser). Mallen definierar leveranskanalen, innehållet och konfigurationen.

1. I **[!UICONTROL Targeting options]** väljer du hur målpopulationen definieras:

   * **[!UICONTROL Specified by the inbound events]**: Målet kommer från den inkommande övergången (från aktiviteter uppströms som Build-målgrupp eller Stegvis fråga). Det här är det vanligaste alternativet.

   * **[!UICONTROL Specified in the delivery template]**: Målet definieras i själva mallen.

   * **[!UICONTROL File specified in the input event]**: Målet tillhandahålls via en fil som skickas via arbetsflödet.

Aktiviteten för kontinuerlig leverans genererar automatiskt en utgående övergång för att fortsätta ditt arbetsflöde.

## Relaterade ämnen {#related}

* [Om arbetsflödesaktiviteter](about-activities.md)
* [E-post, SMS, push, direktreklam](channels.md)
* [Leveransmallar](../../msg/delivery-template.md)
