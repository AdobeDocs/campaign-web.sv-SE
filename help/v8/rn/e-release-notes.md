---
title: Tidiga versionsinformation om webbanvändargränssnittet i Campaign v8
description: Upptäck nya funktioner i nästa version av Campaign Web User Interface
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: d4f9f3562f7dc2550bf9fea01f27456fdfdad43e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 1%

---

# Tidig versionsinformation {#e-release}

Adobe Campaign webbanvändargränssnitt innehåller kontinuerligt nya funktioner, förbättringar av befintliga funktioner och felkorrigeringar. Alla ändringar konsolideras i slutet av varje månad i [versionsinformationen](release-notes.md).

**Noteringar om tidig version nedan kan ändras utan föregående meddelande till releasedatum**. Länkar, skärmar och uppdaterad dokumentation publiceras i [versionsinformationen](release-notes.md) på releasedatum.

## Versionsinformation juli {#24-7-release}

**Releasedatum**: 30-31 juli 2024

Följande funktioner och förbättringar är tillgängliga från och med juliversionen.

### Utsändningslistor {#24-7-2}

En lista, alias. **Svällningsgrupp** är en lista med dirigerade adresser. Det används för att inkludera specifika adresser i leveranser och sedan målprofiler som inte matchar de definierade målvillkoren. På så sätt kan mottagare som inte är leveranskänsliga ta emot leveransen på samma sätt som andra målmottagare. Du kan använda dirigerade adresser när du skickar korrektur eller för att skydda din e-postlista.

### Detaljerade mallar för push-meddelanden {#24-7.3}

Nu kan du skicka omfattande push-meddelanden. Ett omfattande push-meddelande är en förbättrad form av mobilmeddelanden som går längre än enkla textmeddelanden genom att infoga multimediaelement som bilder, interaktiva knappar eller annat multimediematerial. I den här versionen finns det nu en uppsättning mallar för push-meddelanden för dina iOS- och Android-appar.

>[!AVAILABILITY]
>
>Den här funktionen kräver en uppdatering av Campaign v8.6.3 eller v8.7.2. [Läs mer i versionsinformationen för Campaign Client-konsolen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes)


### Förbättringar {#improvements-24-7}

**Mapphantering** - Nu kan du hantera behörigheter och begränsningar för mappar.

### Nya funktioner i begränsad tillgänglighet {#acs-24-4}

>[!AVAILABILITY]
>
>Följande funktioner är i Begränsad tillgänglighet (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.
>
>Se följande dokumentationssidor: [Campaign Standard övergång till Campaign v8](../rn/acs-migration.md) och [Funktioner för Campaign Standarder](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

#### Innehållsfragment {#LA-24-7}

Nu kan du skapa och använda innehållsfragment. Ett innehållsfragment är en återanvändbar komponent som kan refereras i ett eller flera meddelanden. När du ändrar ett fragment uppdateras allt innehåll som använder det. Med den här funktionen kan man skapa flera anpassade innehållsblock som kan användas av marknadsföringsanvändare för att snabbt sammanställa meddelandeinnehåll i en förbättrad designprocess.

Det finns två typer av fragment:

* **Uttrycksfragment** är fördefinierade uttryck som är tillgängliga från en dedikerad post i uttrycksredigeraren.
* **Visuella fragment** är fördefinierade visuella block som du kan återanvända i flera e-postleveranser eller i innehållsmallar. [Läs mer](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >**Visuella fragment** har begränsad tillgänglighet (LA). Den här funktionen är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.
