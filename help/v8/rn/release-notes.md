---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 7%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga med tidigare versioner visas på sidorna [2024](release-notes-24.md) och [2025](release-notes-25.md) .

## 25 oktober {#25-10-updates}

_28 okt 2025_

<table>
<thead>
<tr>
<th><strong>Flerspråkiga funktioner för transaktionsmeddelanden, push-meddelanden och SMS (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nu kan du skicka flera transaktionsmeddelanden, push-meddelanden och SMS-meddelanden på olika språk i Adobe Campaign webbanvändargränssnitt. Med funktionen för flerspråkig leverans kan du välja standardspråk för leveransen samt de olika språk som leveransen kan skickas till. Du kan även förhandsgranska leveransen på de språk du har valt.</p>
<p>Obs! Den här funktionen är bara tillgänglig för en uppsättning organisationer (begränsad tillgänglighet) och kommer att lanseras globalt i en framtida version.</p>
<p>Mer information finns i den <a href="../msg/multilingual.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>Profilberikning i transaktionsmeddelanden (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Med den här funktionen kan du anpassa transaktionsmeddelanden genom att länka Adobe Campaign-databasfält till meddelandeinnehållet. Du kan välja målmappningar, berikningskolumner och en avstämningsnyckel för att säkerställa korrekt personalisering i realtid samtidigt som prestandatrösklar bibehålls.</p>
<p>Obs! Den här funktionen är bara tillgänglig för en uppsättning organisationer (begränsad tillgänglighet) och kommer att lanseras globalt i en framtida version. Den här funktionen är för närvarande endast tillgänglig för e-post.</p>
<p>Mer information finns i den <a href="../transactional-messaging/profile-enrichment.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integrering med Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>För att effektivisera marknadsföringen och bibehålla varumärkets enhetlighet kan ni nu smidigt integrera GenStudio for Performance Marketing-upplevelser med Campaign. På så sätt kan ni utnyttja GenStudio AI-kraftfulla innehållsskapande tillsammans med Campaigns avancerade orkestreringsfunktioner.<p>
<p>Mer information finns i den <a href="../integrations/genstudio.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Stöd för mörkt läge i e-postdesignern</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Med e-post-Designer kan du nu växla till mörkt läge, där du kan definiera ytterligare anpassade inställningar. Observera att den slutliga återgivningen är beroende av mottagarens e-postklient och inte alla e-postklienter stöder mörkt läge.</p>
<p>Mer information finns i den <a href="../email/accessible-content.md#dark-mode">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Förbättringar {#25-10-improvements}

* I leveranser som skapats i klientkonsolen visar nu avsnittet **Målgrupp** om ett dynamiskt villkor har definierats för korrekturmål. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Du kan nu växla mellan det nya och det gamla regelverktyget när du ställer in ett villkor med funktionen för villkorligt innehåll i e-postprogrammet för Designer. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Nu kan du välja samlingslänkar, till exempel inköp, i skärmdefinitionen för mottagarschemat. Då visas relaterade data på profilskärmar via en dedikerad flik. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Som kampanjadministratör kan du nu konfigurera anslutningar till Salesforce CRM och Microsoft Dynamics.
  [Läs mer](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

