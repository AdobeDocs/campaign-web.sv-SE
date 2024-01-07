---
audience: end-user
title: Exempel på frågor
description: Lär dig hur du arbetar med regelbyggaren.
hide: true
hidefromtoc: true
badge: label="Begränsad tillgänglighet"
source-git-commit: e555a6aabab6a20a5b3f3ddecf9d63d49292d55a
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 3%

---

# Exempel på frågor {#query-samples}

## Frågor om mottagare {#querying-recipient-table}

* återställ namn och e-post för mottagare vars e-postdomän är orange.co.uk och som inte bor i London.

* mottagare som inte har kontaktats under de senaste 7 dagarna.

* e-postdomäner som är avsedda för fler än 30 gånger under tidigare leveranser.

## Frågor om leveranser {#number-of-clicks-for-a-specific-delivery}

* antal klick för en viss leverans.

* mottagare som inte öppnat ett e-postmeddelande de senaste sju dagarna.

* profiler som öppnat en leverans de senaste två veckorna:

* Följ upp efter en tidigare leverans.

  Sommarsportserbjudandet skickas ut. Fyra dagar efter leveransen skickas två andra leveranser. Ett av dem är &quot;vattensporterbjudande&quot;, det andra är en uppföljning av det första &quot;Sommarsportserbjudandet&quot;. Leveransen av&quot;vattensporterbjudandet&quot; skickas till mottagare som klickade på länken&quot;vattensporter&quot; vid första leveransen. Dessa klick visar att mottagaren är intresserad av ämnet. Det är rimligt att styra dem mot liknande erbjudanden. Mottagare som inte klickade i &quot;Sommarsportserbjudandet&quot; kommer dock att få samma innehåll igen.
