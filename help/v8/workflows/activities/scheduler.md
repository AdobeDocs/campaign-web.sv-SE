---
audience: end-user
title: Använd arbetsflödesaktiviteten för schemaläggaren
description: Lär dig hur du använder arbetsflödesaktiviteten i schemaläggaren
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 058a9347329b35e49463b7d74bffa5b3c69b4a92
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 2%

---

# Schemaläggare {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Schemaläggaraktivitet"
>abstract="Med aktiviteten **Schemaläggaren** kan du schemalägga när arbetsflödet startas. Denna aktivitet bör betraktas som en planerad start. Den kan bara användas som den första aktiviteten i arbetsflödet."

Aktiviteten **Schemaläggaren** är en **Flödeskontroll**-aktivitet. Du kan schemalägga när arbetsflödet startas. Denna aktivitet bör betraktas som en planerad start. Den kan bara användas som den första aktiviteten i arbetsflödet.

## Bästa praxis {#scheduler-best-practices}

* Schemalägg inte ett arbetsflöde så att det körs mer än var 15:e minut, eftersom det kan påverka den totala systemprestandan negativt och skapa block i databasen.
* Om du vill skicka en engångsleverans i arbetsflödet lägger du till en schemaläggaraktivitet och anger att den ska köras **En gång**. Definiera **Schedule** i leveransinställningarna.
* Om du vill skicka en återkommande leverans i ditt arbetsflöde använder du en **schemaläggaraktivitet** och anger körningsfrekvensen. Den återkommande leveransaktiviteten tillåter inte att du definierar ett schema.

## Konfigurera aktiviteten Schemaläggaren {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Schemaläggarens giltighet"
>abstract="Du kan definiera en giltighetsperiod för schemaläggaren. Den kan vara permanent (standard) eller giltig till ett visst datum."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Alternativ för schemaläggare"
>abstract="Definiera frekvensen för schemaläggaren. Den kan köras vid ett specifikt tillfälle, en eller flera gånger per dag, vecka eller månad."

Följ de här stegen för att konfigurera aktiviteten **Schemaläggaren**:

![Konfigurationsgränssnitt för schemaläggaraktivitet](../assets/workflow-scheduler.png)

1. Lägg till en **schemaläggaraktivitet** i ditt arbetsflöde.

1. Konfigurera **körningsfrekvensen**:

   * **En gång**: Arbetsflödet körs en gång.
   * **Dagligen**: Arbetsflödet körs vid en viss tidpunkt, en gång om dagen.
   * **Flera gånger om dagen**: Arbetsflödet körs regelbundet flera gånger om dagen. Ställ in exekveringar vid specifika tidpunkter eller med jämna mellanrum.
   * **Veckovis**: Arbetsflödet körs vid en angiven tidpunkt, en eller flera gånger i veckan.
   * **Månadsvis**: Arbetsflödet körs vid ett angivet tillfälle, en eller flera gånger i månaden. Välj månader när arbetsflödet måste köras. Du kan också ställa in körningar på angivna veckodagar i månaden, till exempel den andra tisdagen i månaden.

1. Definiera körningsinformationen utifrån den valda frekvensen.  Detaljfälten kan variera beroende på vilken frekvens som används (tid, repetitionsfrekvens, angivna dagar och liknande alternativ).

1. Klicka på **Förhandsgranska starttider** för att kontrollera schemat för de kommande tio körningarna av arbetsflödet.

1. Definiera giltighetsperioden för schemaläggaren:

   * **Permanent (upphör aldrig att gälla)**: Arbetsflödet körs enligt den angivna frekvensen, utan begränsningar för tidsramen eller antalet iterationer.
   * **Giltighetsperiod**: Arbetsflödet körs enligt angiven frekvens, fram till ett visst datum. Ange start- och slutdatum.

>[!NOTE]
>Om du vill starta arbetsflödet direkt klickar du på **Kör väntande uppgift** i schemaläggarens övre åtgärdsfält. Den här knappen är bara tillgänglig när arbetsflödet har startats.

## Exempel {#scheduler-example}

I följande exempel är aktiviteten konfigurerad så att arbetsflödet körs flera gånger per dag kl. 9 och 12, varje veckodag från 1 oktober 2023 till 1 januari 2024.

![Exempelkonfiguration för schemaläggaraktivitet](../assets/workflow-scheduler2.png)
