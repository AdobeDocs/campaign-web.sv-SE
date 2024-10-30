---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5dc96beadbd5ea02540185634971cef44357aefa
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 8%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

## Oktober-version {#24-10-release}

**Releasedatum**: 29 okt 2024

Följande funktioner och förbättringar är tillgängliga från och med oktober.

### Funktioner

<table>
<thead>
<tr>
<th><strong>Externa konton</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du konfigurera och hantera externa konton direkt via Adobe Campaign webbanvändargränssnitt. Den här nya funktionen gör det enkelt att konfigurera olika typer av externa konton, till exempel studentmeddelanden (POP3) eller exekveringsinstanser.</p>
<p>Mer information finns i den <a href="../administration/external-account.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transaktionsmeddelanden</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transactional Messaging (Message Center) är nu tillgängligt i webbgränssnittet för Campaign. Det här tillägget är utformat för att utlösa meddelanden som genereras från händelser som utlöses från informationssystem, och kan vara: faktura, orderbekräftelse, leveransbekräftelse, lösenordsändring, meddelande om produkttillgänglighet, kontobesked, skapande av webbkonto osv.</p>
<p>Mer information finns i den <a href="../transactional-messaging/transactional.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Förbättringar

* **Arbetsflödesaktiviteter** - Du kan nu flytta en aktivitet och alla dess underordnade noder från en övergång till en annan i ett arbetsflöde. En dedikerad **Flytta**-knapp är tillgänglig i aktivitetens egenskapspanel för att utföra detta. [Läs mer](../workflows/orchestrate-activities.md#move)

* **Aktivitet för arbetsflödesberikning**

   * Du kan nu definiera ett alias och en etikett när du skapar ett nytt fält i aktiviteten **Enrichment**. [Läs mer](../workflows/activities/enrichment.md#collection-settings)
   * Nu kan du lägga till erbjudanden för varje profil i aktiviteten **Enrichment**. [Läs mer](../workflows/activities/enrichment.md##add-offers)

* **Distribution av värden** - Vid åtkomst till listan med fält för anpassning kan du nu kontrollera hur värden distribueras för varje fält. Ett dedikerat popup-fönster visar antalet och procentandelen för varje värde. [Läs mer](../query/build-query.md#distribution-values-query)

* **Version- och systeminformation** - Nu kan du komma åt information om dina instansversioner, både för klientkonsolen och webbanvändargränssnittet. I det nya avsnittet visas även alla inbyggda paket som är installerade i din miljö. [Läs mer](../get-started/user-interface.md#user-interface-about)

* **Listor** - Nu kan du enkelt ändra ordningen på värdena i en lista. [Läs mer](../get-started/work-with-folders.md)
