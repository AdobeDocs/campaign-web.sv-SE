---
product: campaign
title: Granskningskedja
description: Lär dig övervaka instansen med granskningsspår för Campaign
feature: Audit Trail, Monitoring, Workflows
source-git-commit: 4f7dd30f02f83624a00b3d0e6ac7ba74c1c242e0
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 1%

---

# Granskningskedja{#audit-trail}

>[!IMPORTANT]
>
>Adobe Campaign webbanvändargränssnitt granskar inte ändringar som gjorts i användarrättigheter, mallar, personalisering eller kampanjer.\
>Granskningsspårning kan bara hanteras av administratörer för instansen.

I Adobe Campaign webbgränssnitt är **[!UICONTROL Audit trail]** -funktionen ger användarna fullständig synlighet för alla ändringar som görs på viktiga enheter i instansen, vanligtvis sådana som avsevärt påverkar en mjuk funktion i instansen.

**[!UICONTROL Audit trail]** funktionen registrerar ständigt en detaljerad logg över åtgärder och händelser som äger rum i Adobe Campaign-instansen i realtid. Den erbjuder en praktisk metod för att få tillgång till en kronologisk datapost, som behandlar frågor som till exempel status för arbetsflöden, de senaste personerna att ändra dem eller aktiviteter som utförs av användare i instansen.

+++ Läs mer om tillgängliga enheter för granskningsspår

* **Granskningsspår för källschema** gör att du kan övervaka aktiviteter och nyligen gjorda ändringar av dina scheman i klientkonsolen för Campaign V8.

  Mer information om scheman finns i [Campaign v8-dokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Granskningsspår för arbetsflöde** gör att du kan hålla reda på aktiviteter och nyligen gjorda ändringar i arbetsflöden, inklusive deras aktuella tillstånd som:

   * Starta
   * Pausa
   * Stoppa
   * Starta om
   * Rensning som motsvarar åtgärden Rensa historik
   * Simulera vilket motsvarar åtgärden Starta i simuleringsläge
   * Aktivering som är lika med åtgärden Kör väntande uppgifter nu
   * Ovillkorligt stopp

  Mer information om arbetsflöden finns i [page](../workflows/gs-workflows.md).

* **Alternativ granskningsspår** gör att du kan övervaka aktiviteter och nyligen gjorda ändringar av dina alternativ i Campaign V8.

  Mer information om alternativen finns i [page](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Granskningsspår för leverans** gör att du kan kontrollera aktiviteter och senaste ändringar som gjorts i leveranserna.

  Mer information om leveranser finns i [page](../msg/gs-deliveries.md).

* **Externt konto** gör att du kan kontrollera ändringar som gjorts i externa konton i Campaign V8, som används av tekniska processer som tekniska arbetsflöden eller kampanjarbetsflöden.

  Mer information om externt konto finns i [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Leveransmappning** gör att du kan övervaka aktiviteter och nyligen gjorda ändringar av din leveranskarta i Campaign V8.

  Mer information om leveransmappning finns i [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Webbprogram** Med kan du kontrollera ändringar som gjorts i webbformulär i Campaign V8 som används för att skapa sidor med indata- och urvalsfält, och som kan innehålla data från databasen.

  Mer information om webbprogram finns i [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Erbjudande** gör att du kan kontrollera aktiviteter och senaste ändringar som gjorts i dina erbjudanden.

  Mer information om erbjudanden finns i [page](../msg/offers.md).

* **Operator** gör att du kan övervaka aktiviteter och nyligen gjorda ändringar för dina operatorer i Campaign V8.

  Mer information om operatorer finns i [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Åtkomst till granskningsspår {#accessing-audit-trail}

Så här kommer du åt instansens **[!UICONTROL Audit trail]**:

1. Under **[!UICONTROL Administration]** meny, välja **[!UICONTROL Audit trail]** .

   ![](assets/audit-trail-1.png)

1. The **[!UICONTROL Audit trail]** öppnas med listan över dina enheter. Adobe Campaign webbanvändargränssnitt granskar åtgärderna för att skapa, redigera och ta bort för arbetsflöden, alternativ, leveranser och scheman.

   Välj en av enheterna om du vill veta mer om de senaste ändringarna.

1. The **[!UICONTROL Audit entity]** I fönstret finns mer detaljerad information om den valda enheten, till exempel:

   * **[!UICONTROL Type]** : Arbetsflöde, alternativ, leveranser eller scheman.
   * **[!UICONTROL Entity]** : Internt namn på dina aktiviteter.
   * **[!UICONTROL Modified by]** : Användarnamn för den sista personen som senast ändrade den här entiteten.
   * **[!UICONTROL Action]** : Senaste åtgärden som utfördes på den här entiteten, antingen Skapad, Ändrad eller Borttagen.
   * **[!UICONTROL Modification date]** : Datum för den senaste åtgärden som utfördes på den här entiteten.

   Kodblocket ger dig mer information om exakt vad som har ändrats i din enhet.

   ![](assets/audit-trail-2.png)

