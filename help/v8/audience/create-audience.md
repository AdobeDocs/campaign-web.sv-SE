---
audience: end-user
title: Skapa målgrupper
description: Lär dig skapa målgrupper i Adobe Campaign Web
badge: label="Beta"
source-git-commit: ba449ee0b5a4b41db8efbbabeb37ce7cd7cc3720
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# Skapa målgrupper {#create-audiences}

målgruppsmenyn

kan skapa och inrikta sig på dem i fristående leveranser eller kampanjer

## Skapa din första målgrupp {#create}

1. Målgrupp > meny
1. Skapa målgrupper
1. Egenskaper: etikett och ytterligare alternativ
1. Arbetsyta med en målgruppsaktivitet som bygger upp
1. Redigera aktivitet, redigera arbetsflöde beroende på hans behov
1. starta arbetsflödet (kan endast lägga till riktade aktiviteter? Inga kanalaktiviteter?) = Skapar målgruppen och arbetsflödet

## Övervaka och hantera era målgrupper {#monitor}

I målgruppen som skapats har du en kontrollpanel med två flikar:
* översikt: egenskaper + arbetsflödesstatus och antal mottagardelar av den här målgruppen genom att anropa calculate + kan komma åt och redigera arbetsflödet härifrån
* data: visa dataprofiler som ingår i målgruppen. Kan lägga till nya kolumner vid behov. Se berikade data

målgruppslista: duplicera, ta bort

**frågor:**

Arbetsflöde i &quot;målgruppsläge&quot; => utskickskanalaktiviteter är inte tillgängliga

* på sceninstans: vi kan ta bort den senaste qsave-aktiviteten och lägga till en kanalaktivitet i stället
* Hur känner vi igen ett arbetsflöde i målgruppsläge?
