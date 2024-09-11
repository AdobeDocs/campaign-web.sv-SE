---
product: campaign
title: Granskningskedja
description: Lär dig övervaka instansen med granskningsspår för Campaign
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: dfd5f2e000b02d4382eaac0c9bb00fe940a99f79
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 1%

---

# Granskningskedja{#audit-trail}

I Adobe Campaign webbanvändargränssnitt ger funktionen **[!UICONTROL Audit trail]** användarna fullständig synlighet för alla ändringar som görs i viktiga entiteter i instansen, vanligtvis sådana som påverkar instansens smidiga funktion avsevärt.

>[!IMPORTANT]
>
>* Adobe Campaign webbanvändargränssnitt granskar inte ändringar som gjorts i användarrättigheter, mallar, personalisering eller kampanjer.
>* Granskningsspårning kan bara hanteras av administratörer för instansen.

Funktionen **[!UICONTROL Audit trail]** registrerar hela tiden en detaljerad logg över åtgärder och händelser som äger rum i Adobe Campaign-instansen i realtid. Den erbjuder en praktisk metod för att få tillgång till en kronologisk datapost, som behandlar frågor som till exempel status för arbetsflöden, de senaste personerna att ändra dem eller aktiviteter som utförs av användare i instansen.

+++ Läs mer om tillgängliga enheter för granskningsspår

* **Source Schema-granskningsspår** gör att du kan övervaka aktiviteter och nyligen gjorda ändringar av dina scheman i klientkonsolen för Campaign V8.

  Mer information om scheman finns i [Kampanjdokumentation ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Arbetsflödets granskningsspår** gör att du kan hålla reda på aktiviteter och nyligen gjorda ändringar i arbetsflöden, inklusive deras aktuella tillstånd, som:

   * Starta
   * Pausa
   * Stoppa
   * Starta om
   * Rensning som motsvarar åtgärden Rensa historik
   * Simulera vilket motsvarar åtgärden Starta i simuleringsläge
   * Aktivering som är lika med åtgärden Kör väntande uppgifter nu
   * Ovillkorligt stopp

  Mer information om arbetsflöden finns på [sidan](../workflows/gs-workflows.md).

* Med **Alternativ granskningsspår** kan du övervaka aktiviteter och nyligen gjorda ändringar av dina alternativ i Campaign V8.

  Mer information om alternativ finns på [sidan](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Leveransverifieringskedja** gör att du kan kontrollera aktiviteter och senaste ändringar som du har gjort i leveranserna.

  Mer information om leveranser finns på [sidan](../msg/gs-deliveries.md).

* Med **externt konto** kan du kontrollera ändringar som gjorts i externa konton i Campaign V8, som används av tekniska processer som tekniska arbetsflöden eller kampanjarbetsflöden.

  Mer information om externt konto finns på [sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* Med **Leveransmappning** kan du övervaka aktiviteter och nyligen gjorda ändringar av din leveransmappning i kampanj V8.

  Mer information om leveransmappning finns på [sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* Med **Webbprogram** kan du kontrollera ändringar som gjorts i webbformulär i Campaign V8 som används för att skapa sidor med indata- och urvalsfält, och som kan innehålla data från databasen.

  Mer information om webbprogram finns på [sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* Med **Erbjudandet** kan du kontrollera aktiviteter och senaste ändringar av dina erbjudanden.

  Mer information om erbjudanden finns på [sidan](../msg/offers.md).

* Med **Operator** kan du övervaka aktiviteter och nyligen gjorda ändringar av dina operatorer i Campaign V8.

  Mer information om operatorer finns på [sidan](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Åtkomst till granskningsspår {#accessing-audit-trail}

Så här kommer du åt instansens **[!UICONTROL Audit trail]**:

1. Välj **[!UICONTROL Audit trail]** på menyn **[!UICONTROL Administration]**.

   ![](assets/audit-trail-1.png)

1. Fönstret **[!UICONTROL Audit trail]** öppnas med listan över dina enheter. Adobe Campaign webbanvändargränssnitt granskar åtgärderna för att skapa, redigera och ta bort för arbetsflöden, alternativ, leveranser och scheman.

   Välj en av enheterna om du vill veta mer om de senaste ändringarna.

1. Fönstret **[!UICONTROL Audit entity]** ger dig mer detaljerad information om den valda entiteten, till exempel:

   * **[!UICONTROL Type]**: Arbetsflöde, alternativ, leveranser eller scheman.
   * **[!UICONTROL Entity]**: Inbyggt namn på dina aktiviteter.
   * **[!UICONTROL Modified by]**: Användarnamn för den senaste personen som ändrade entiteten.
   * **[!UICONTROL Action]**: Senaste åtgärden som utfördes på den här entiteten, antingen Skapad, Ändrad eller Borttagen.
   * **[!UICONTROL Modification date]**: Datum för den senaste åtgärden som utfördes på entiteten.

   Kodblocket ger dig mer information om exakt vad som har ändrats i din enhet.

   ![](assets/audit-trail-2.png)
