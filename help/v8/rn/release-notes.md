---
title: Versionsinformation om webbgränssnittet i Campaign v8
description: Upptäck nya funktioner i den senaste versionen av Campaign Web User Interface
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 8%

---

# Versionsinformation {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionsinformation"
>abstract="Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Versionsinformationen för Campaign uppdateras därför flera gånger i månaden, med de senaste funktionerna, förbättringarna och korrigeringarna. Vi rekommenderar att du regelbundet kontrollerar dem."

Adobe Campaign Web Interface används i en kontinuerlig leveransmodell som ger en mer skalbar, stegvis metod för driftsättning av funktioner. Därför uppdateras versionsinformationen flera gånger i månaden. Kontrollera dem regelbundet.

Ändringar och förbättringar som är tillgängliga med tidigare versioner visas på sidorna [2024](release-notes-24.md) och [2025](release-notes-25.md) .

## Uppdateringar 25 oktober {#25-9-updates}

_9 okt 2025_

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


## 25 september {#25-9-release}

_23 september 2025_

Följande funktioner är tillgängliga från och med september.

<table>
<thead>
<tr>
<th><strong>Anpassad kanal för API-leveranser</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Du kan nu, direkt från Adobe Campaign Web UI, samordna och köra leveranser baserade på anpassade API-kanaler. Dessa leveranser kan vara fristående eller ingå i ett arbetsflöde. Konfigurationen av den anpassade API-kanalen utförs i konsolen.</p>
<p>Mer information finns i den <a href="../call-center/gs-custom-channel.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Skapa externa konton</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Som Campaign-administratör kan du nu skapa nya anslutningar med externa system från användargränssnittet i Campaign Web. Du kan också visa, uppdatera och hantera befintliga externa konton.</p>
<p>Mer information finns i den <a href="../administration/create-external-account.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Låsning av e-postinnehåll</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Med Campaign kan ni nu låsa innehåll i e-postmallar, antingen genom att låsa hela mallen eller specifika strukturer och komponenter. På så sätt kan ni förhindra oavsiktliga redigeringar och borttagningar, vilket ger er bättre kontroll över mallanpassning och förbättrar effektiviteten och tillförlitligheten i era e-postkampanjer.</p>
<p>Mer information finns i den <a href="../content/content-locking.md">detaljerade dokumentationen</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Förbättringar {#25-9-improvements}

* En uppsättning nya operatorer har lagts till när ett villkor skapas med e-postens Designer-funktion för villkorligt innehåll.
* Filtreringsdimensionen är nu tillgänglig i arbetsflödesaktiviteten **Bygg målgrupp**. Om du vill visa eller ändra den klickar du på ikonen bredvid måldimensionen. [Läs mer](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

