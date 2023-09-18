---
audience: end-user
title: Hantera kampanjmallar med Adobe Campaign Web
description: Lär dig hantera kampanjmallar med Adobe Campaign Web
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---


# Hantera kampanjmallar{#manage-campaign-templates}

Alla marknadsföringskampanjer bygger på en mall som lagrar de viktigaste egenskaperna och funktionerna. Campaign innehåller en uppsättning inbyggda mallar som hjälper er att komma igång. Du kan skapa och konfigurera kampanjmallar och sedan skapa kampanjer utifrån dessa mallar.

## Skapa en kampanjmall

Så här skapar du en kampanjmall:

Öppna Campaign Explorer och bläddra till Resurser > Mallar > Campaign-mallar.
Klicka på Nytt i verktygsfältet ovanför listan med mallar.


Du kan också duplicera den inbyggda mallen för att återanvända och anpassa dess konfiguration. Om du vill göra det högerklickar du på mallen och väljer Duplicera.

Ange etiketten för den nya kampanjmallen.

Klicka på Spara och öppna mallen igen.

Definiera mallegenskaperna på fliken Redigera.

Välj länken Avancerade kampanjparametrar för att lägga till ett arbetsflöde i kampanjmallen.



Ändra målvärdet och arbetsflödesvärdet till Ja och bekräfta. Lär dig hur du lägger till funktioner i det här avsnittet.

Fliken Mål och arbetsflöden läggs till i mallen. Klicka på Lägg till ett arbetsflöde.., ange en etikett och klicka på OK.

Skapa arbetsflödet efter behov.



Klicka på Spara. Mallen är nu klar att användas för att skapa en ny kampanj.

På de olika flikarna och underflikarna i kampanjmallen kan du komma åt inställningarna som beskrivs i den allmänna konfigurationen.

Välj moduler Med länken Avancerade kampanjparametrar kan du aktivera och inaktivera jobb för kampanjer som är baserade på den här mallen. Välj de funktioner som du vill aktivera i kampanjer som skapas baserat på den här mallen.



Om ingen funktion är markerad, de element som rör processen (menyer, ikoner, alternativ, flikar, underflikar osv.) visas inte i mallens gränssnitt eller i kampanjer som är baserade på den här mallen. Flikarna till vänster om kampanjinformationen och de tillgängliga flikarna sammanfaller med de funktioner som valts i mallen. Funktionen för utgifter och mål är till exempel inte aktiverad, och motsvarande budgetflik visas inte i kampanjer som baseras på den här mallen.

Dessutom läggs genvägar till konfigurationsfönstren till på kontrollpanelen för kampanjer. När en funktion är aktiverad får en direktlänk åtkomst till den från kontrollpanelen för kampanjer.

Exempel på konfiguration med följande inställningar:



Kampanjpanelen visar:



Observera att fliken Mål och arbetsflöden saknas.

Följande funktioner är tillgängliga:



Observera att fliken Budget saknas.

De avancerade inställningarna för kampanjen återspeglar även den här konfigurationen.



Observera att fliken Godkännanden inte är tillgänglig.

Med den här konfigurationen:


Kampanjpanelen visar:



Observera att fliken Mål och arbetsflöden är tillgänglig men länken Lägg till ett dokument saknas.

Följande funktioner är tillgängliga:



Observera att fliken Budget är tillgänglig.

De avancerade inställningarna för kampanjen återspeglar även den här konfigurationen.



Observera att fliken Godkännanden är tillgänglig men flikarna Kontrollifyllning och dirigeringsadresser är inte aktiverade.

Typologi av moduler Kontrollgrupp

När den här modulen är markerad läggs en extra flik till i de avancerade inställningarna för mallen och kampanjerna som är baserade på den här mallen. Konfigurationen kan definieras via mallen eller individuellt för varje kampanj. Läs mer om kontrollgrupper i det här avsnittet.



Dirigerade adresser

När den här modulen är markerad läggs en extra flik till i de avancerade inställningarna för mallen och kampanjerna som är baserade på den här mallen. Konfigurationen kan definieras via mallen eller individuellt för varje kampanj.



Dokument

När den här modulen är markerad läggs en extra flik till på fliken Redigera i mallen och de kampanjer som är baserade på den här mallen. Bifogade dokument kan läggas till från mallen eller individuellt för varje kampanj. Läs mer om dokument i det här avsnittet.



Leveransbeskrivning

När den här modulen är markerad läggs en underflik för leveransdispositioner till på fliken Dokument för att definiera leveransdispositioner för kampanjen. Läs mer om leveransdispositioner i det här avsnittet.



Målgruppsanpassning och arbetsflöden

När du väljer modulen Mål och arbetsflöden läggs en flik till så att du kan skapa ett eller flera arbetsflöden för kampanjer som är baserade på den här mallen. Arbetsflöden kan också konfigureras individuellt för varje kampanj baserat på den här mallen.Läs mer om kampanjarbetsflöden i det här avsnittet.



När den här modulen är aktiverad läggs en jobbflik till i de avancerade inställningarna för kampanjen för att definiera processkörningssekvensen.

Godkännanden

Om du aktiverar godkännandena kan du välja vilka processer som ska godkännas och vilka operatörer som ansvarar för godkännandena. Läs mer om godkännanden i det här avsnittet.



Du kan välja om du vill aktivera processgodkännande eller inte via fliken Godkännanden i mallavsnittet Avancerade inställningar.

Utgifter och mål

När den här modulen har valts läggs en budgetflik till i informationen om mallen och kampanjer som är baserade på den här mallen, så att den associerade budgeten kan väljas.



Mallegenskaper


När du skapar en kampanjmall måste du ange följande information:

Ange mallens etikett: etiketten är obligatorisk och är standardetikett för alla kampanjer som baseras på den här mallen.
Välj kampanjtyp i listrutan. De värden som är tillgängliga i den här listan är de som har sparats i natureOp-uppräkningen.
Lär dig hur du får åtkomst till och konfigurerar uppräkningarna på den här sidan.

Välj kampanjtyp: unik, återkommande eller periodisk. Som standard används kampanjmallar för unika kampanjer. Återkommande och periodiska kampanjer beskrivs i det här avsnittet.

Ange kampanjens varaktighet, dvs. antalet dagar som kampanjen ska äga rum. När du skapar en kampanj som baseras på den här mallen fylls start- och slutdatumet för kampanjen i automatiskt.

Om kampanjen är återkommande måste du ange kampanjens start- och slutdatum direkt i mallen.

Ange mallens relaterade program: kampanjer som är baserade på den här mallen är länkade till det valda programmet.

