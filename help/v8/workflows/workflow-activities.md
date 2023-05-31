---
audience: end-user
title: Arbeta med arbetsflödesaktiviteter
description: Lär dig hur du arbetar med arbetsflödesaktiviteter
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: ebd119a38129f8576ad9b4e4b9301b116a255c9b
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 7%

---


# Arbetsflödesaktiviteter {#workflow-activities}

## Målinriktade aktiviteter {#targeting}

Med de här aktiviteterna kan du skapa ett eller flera mål genom att definiera uppsättningar och dela eller kombinera dem med hjälp av korsnings-, union- eller exkluderingsåtgärder.

### Bygg målgrupper {#build-audience}

Med den här aktiviteten kan du definiera en målgrupp. Du kan antingen välja en befintlig Campaign-förekomst eller använda regelbyggaren för att definiera en egen fråga.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

Följ de här stegen för att konfigurera **Bygg målgrupper** aktivitet:

1. Lägg till en Build-målgruppsaktivitet.
1. Definiera en etikett.
1. Definiera målgruppstyp: **Skapa en egen** eller **Läsa målgrupper**.

Så här skapar du en egen fråga:

1. Välj **Skapa en egen (fråga)**.
1. Välj **Måldimension**. Med måldimensionen kan du definiera målgruppen för åtgärden: mottagare, mottagare, mottagare, operatör, abonnenter osv. Som standard är målet markerat bland mottagarna. Se [v8-dokumentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Klicka **Fortsätt**.
1. Använd regelbyggaren för att definiera frågan, på samma sätt som du skapar en målgrupp när du utformar ett nytt e-postmeddelande. Se detta [section](../audience/segment-builder.md).

Så här väljer du en befintlig målgrupp:

1. Välj **Läsa målgrupper**.
1. Klicka **Fortsätt**.
1. Välj målgrupp på samma sätt som du använder en målgrupp när du utformar ett nytt e-postmeddelande. Se detta [section](../audience/add-audience.md).

### Kombinera {#combine}

Med den här aktiviteten kan du bearbeta uppsättningar på inkommande data. Du kan alltså kombinera flera populationer, utesluta en del av dem eller bara behålla data som är gemensamma för flera mål. Här är de tillgängliga segmenteringstyperna:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* The **Union** kan du gruppera om resultatet av flera aktiviteter till ett enda mål.
* The **Skärningspunkt** gör att du bara kan behålla de element som är gemensamma för de olika inkommande populationerna i aktiviteten.
* The **Uteslutning** gör att du kan utesluta element från en population enligt vissa kriterier.

Följ de här stegen för att konfigurera **Kombinera** aktivitet:

1. Lägg till **Kombinera** aktivitet till någon av de tidigare segmenteringsövergångarna.
1. Välj segmenteringstyp: union, skärning eller uteslutning.
1. Klicka **Fortsätt**.
1. I **Uppsättningar att förena** markerar du alla tidigare aktiviteter du vill delta i.

För **Union** och **Skärningspunkt** måste du välja **Avstämningstyp** för att definiera hur dubbletter hanteras:

    * Endast tangenter: det här är standardläget. Aktiviteten behåller endast ett element när element från olika inkommande övergångar har samma nyckel.  Detta alternativ kan endast användas om de inkommande populationerna är homogena.
    * En markering med kolumner: Välj det här alternativet om du vill definiera listan med kolumner som datavstämningen ska tillämpas på. Du måste först markera den primära uppsättningen (som innehåller källdata) och sedan de kolumner som ska användas för kopplingen.

För **Skärningspunkt** och **Uteslutning** kan du kontrollera **Generera slutförande** om du vill bearbeta den återstående populationen. Komplementet ska innehålla en kombination av resultaten av alla inkommande aktiviteter minus skärningspunkten. En ytterligare utgående övergång läggs sedan till i aktiviteten.

För **Uteslutning** väljer du **Primär uppsättning** från inkommande övergångar, i **Uppsättningar att förena** -avsnitt. Detta är den uppsättning från vilken element utesluts. De andra uppsättningarna matchar element innan de utesluts från den primära uppsättningen.

### Berikning {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anrikningsaktivitet"
>abstract="Med Enrichment-aktiviteten kan du förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter riktade aktiviteter.<br/>När berikningsdata har lagts till i arbetsflödet kan de användas i aktiviteter som lagts till efter Enrichment-aktiviteten för att segmentera kunder i olika grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får genklang hos målgruppen."

Med Enrichment-aktiviteten kan du förbättra måldata med ytterligare information från databasen. Det används ofta i ett arbetsflöde efter riktade aktiviteter.

Anrikningsdata kan komma antingen:

* **Från samma arbetsregister** som den som är inriktad på ditt arbetsflöde:

   *Ange en grupp kunder som målgrupp och lägg till fältet&quot;Födelsedatum&quot; i den aktuella arbetstabellen*

* **Från en annan arbetstabell**:

   *Ange kunder som målgrupp och lägg till fälten&quot;Belopp&quot; och&quot;Typ av produkt&quot; som kommer från tabellen&quot;Inköp&quot;*.

När berikningsdata har lagts till i arbetsflödet kan de sedan användas i aktiviteter som lagts till efter Enrichment-aktiviteten för att segmentera kunder i olika grupper baserat på deras beteenden, önskemål och behov, eller för att skapa personaliserade marknadsföringsmeddelanden och kampanjer som troligtvis får genklang hos målgruppen.

Du kan till exempel lägga till information om kundernas inköp i arbetsflödets arbetsregister och använda dessa data för att anpassa e-postmeddelanden med deras senaste köp eller hur mycket som spenderas på dessa inköp.

Så här lägger du till en fördjupningsaktivitet i arbetsflödet:

1. lägg till aktivitet
1. välj attribut att använda som anrikningsdata

   visa avancerat fält, alternativ i

   Obs! attribut från måldimensionen

1. Välj hur data samlas in
1. antal poster som ska hämtas om du vill hämta en samling med flera poster
1. Använda filter och skapa regel

   markera ett befintligt filter och spara filtret för att återanvända resultatet av filtret visuellt eller i kodvyn

1. sortera poster med ett attribut

utnyttja anrikningsdata i kampanjen

där vi kan använda anrikningsdata: personalisera e-post, andra användningsfall?

## Kanalaktiviteter {#channel}

Med Adobe Campaign Web kan ni automatisera och köra marknadsföringskampanjer i flera kanaler, som e-post, SMS eller push. Med Adobe Campaign arbetsflöden kan du kombinera kanalaktiviteter på arbetsytan för att skapa flerkanaliga arbetsflöden som kan utlösa åtgärder baserat på kundbeteende.

Du kan till exempel skapa en välkomstkampanj för e-post som innehåller en serie meddelanden i olika kanaler, som e-post, SMS och push. Du kan också skicka ett uppföljningsmeddelande via e-post när en kund har slutfört ett köp eller skicka ett personligt födelsedagsmeddelande till en kund via SMS.

Genom att använda kanalaktiviteter kan ni skapa omfattande, personaliserade kampanjer som engagerar kunder över flera kontaktytor och driver konverteringar.

Kanalaktiviteter är tillgängliga från paletten, till vänster på skärmen, i avsnittet Kanaler.

### E-post {#email}

description, which use case you can perform (common other tasks that you can link before of after the activity)

lägga till och konfigurera aktiviteten

exempel på en konfigurerad aktivitet i ett arbetsflöde


Med aktiviteten för e-postleverans kan du konfigurera skickandet av ett e-postmeddelande i ett arbetsflöde.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

E-postmottagare definieras uppströms aktiviteten i samma arbetsflöde, via en målgruppsaktivitet.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Push-meddelande (Android) {#push-android}

### Push-meddelande (iOS) {#push-ios}

## Flödeskontrollaktiviteter {#flow-control}

content TBD

<!--à reformuler-->Med de här aktiviteterna kan du skapa ett eller flera mål genom att definiera uppsättningar och dela eller kombinera dem med hjälp av korsnings-, union- eller exkluderingsåtgärder.

Flödeskontrollaktiviteter används för att samordna arbetsflödesaktiviteter.

### Förgrening {#fork}

### AND-join {#join}


### Vänta {#wait}

### End {#end}

## Datahanteringsaktiviteter {#data-management}

översikt: vad de används för vilket användningsfall du kan använda dem

visa tillgängliga aktiviteter + kort beskrivning + ref to section

