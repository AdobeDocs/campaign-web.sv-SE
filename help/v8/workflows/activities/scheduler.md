---
audience: end-user
title: Använd arbetsflödesaktiviteten för schemaläggaren
description: Lär dig hur du använder arbetsflödesaktiviteten i schemaläggaren
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 15%

---


# Schemaläggare {#scheduler}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler activity"
>abstract="The Scheduler activity allows you..."
-->

The **Schemaläggare** aktiviteten är en **Flödeskontroll** aktivitet. Du kan schemalägga när arbetsflödet startas. Denna aktivitet bör betraktas som en planerad start. Den kan bara användas som den första aktiviteten i arbetsflödet.

## God praxis

Schemalägg inte ett arbetsflöde så att det körs mer än var 15:e minut eftersom det kan påverka den totala systemprestandan negativt och skapa block i databasen.

## Konfiguration

Följ de här stegen för att konfigurera **Schemaläggare** aktivitet:

1. Lägg till en **Schemaläggare** till ditt arbetsflöde.

   ![](../assets/workflow-scheduler.png)

1. Konfigurera **Körningsfrekvens**:

   * **En gång**: arbetsflödet körs en gång.

   * **Dagligen**: arbetsflödet körs vid en viss tidpunkt, en gång om dagen.

   * **Flera gånger om dagen:** arbetsflödet körs regelbundet flera gånger om dagen. Du kan ställa in körningar vid specifika tidpunkter eller med jämna mellanrum.

   * **Vecka**: arbetsflödet körs vid ett angivet tillfälle, en eller flera gånger i veckan.

   * **Månadsvis**: arbetsflödet körs vid ett angivet tillfälle, en eller flera gånger i månaden. Du kan välja de månader du vill att arbetsflödet ska köras.  Du kan också ställa in körningar på angivna veckodagar i månaden, till exempel den andra tisdagen i månaden.

1. Definiera körningsinformationen utifrån den valda frekvensen.  Detaljfälten kan variera beroende på vilken frekvens som används (tid, repetitionsfrekvens, angivna dagar etc.).

1. Klicka **Tidpunkter för förhandsgranskning** för att kontrollera schemat för de kommande tio körningarna av ditt arbetsflöde.

1. Definiera giltighetsperioden för schemaläggaren:

   * **Permanent (upphör aldrig)**: arbetsflödet körs enligt angiven frekvens, utan begränsningar av tidsramen eller antalet iterationer.

   * **Giltighetsperiod**: arbetsflödet körs enligt angiven frekvens fram till ett visst datum. Du måste ange start- och slutdatum.

## Exempel

I följande exempel är aktiviteten konfigurerad så att arbetsflödet startar flera gånger per dag kl. 9 och kl. 12 varje veckodag från 1 oktober 2023 till 1 januari 2024.

![](../assets/workflow-scheduler2.png)



