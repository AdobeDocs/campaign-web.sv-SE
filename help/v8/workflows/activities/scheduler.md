---
audience: end-user
title: Använd arbetsflödesaktiviteten för schemaläggaren
description: Lär dig hur du använder arbetsflödesaktiviteten i schemaläggaren
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 30%

---


# Schemaläggare {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Schemaläggaraktivitet"
>abstract="Med aktiviteten Schemaläggaren kan du.."

Med aktiviteten Schemaläggare så kan du schemalägga när ett arbetsflöde eller en aktivitet ska starta.

Schemaläggaraktiviteten ska betraktas som en schemalagd start. Den här aktiviteten kan bara användas som den första aktiviteten i arbetsflödet.

## God praxis

* Schemalägg inte ett arbetsflöde så att det körs mer än var 15:e minut eftersom det kan påverka den totala systemprestandan negativt och skapa block i databasen.

## Konfiguration

Följ de här stegen för att konfigurera **Schemaläggare** aktivitet:

1. Lägg till en **Schemaläggare** till ditt arbetsflöde.

1. Konfigurera **Körningsfrekvens**:

   * När: arbetsflödet körs en gång.

   * Dagligen: arbetsflödet körs vid en viss tidpunkt, en gång om dagen.

   * Flera gånger om dagen: arbetsflödet körs regelbundet flera gånger om dagen. Du kan ställa in körningar vid specifika tidpunkter eller med jämna mellanrum.

   * Varje vecka: arbetsflödet körs vid ett angivet tillfälle, en eller flera gånger i veckan.

   * Varje månad: arbetsflödet körs vid ett angivet tillfälle, en eller flera gånger i månaden. Du kan välja de månader du vill att arbetsflödet ska köras.  Du kan också ställa in körningar på vissa veckodagar i månaden som till exempel den andra tisdagen i månaden.
1. Definiera körningsinformationen utifrån den valda frekvensen.  Detaljfälten kan variera beroende på vilken frekvens som används (tid, repetitionsfrekvens, angivna dagar etc.).

1. Klicka **Tidpunkter för förhandsgranskning** för att kontrollera schemat för de kommande tio körningarna av ditt arbetsflöde.

1. Definiera giltighetsperioden för schemaläggaren:

   * Permanent (upphör aldrig att gälla): arbetsflödet körs enligt den angivna frekvensen, utan begränsningar av tidsramen eller antalet iterationer.

   * Giltighetsperiod: arbetsflödet körs enligt angiven frekvens, fram till ett visst datum. Tidsfristen för körningen måste av den anledningen anges.

## Exempel


