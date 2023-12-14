---
audience: end-user
title: Skapa din första fråga med frågemodelleraren
description: Lär dig hur du skapar din första fråga i Adobe Campaign Web Query Modeler.
source-git-commit: e78122b0788c04c39eac27231272cb96ad019bdc
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 0%

---

# Bygg din första fråga {#build-query}

Om du vill börja skapa en fråga öppnar du frågemodelleraren från valfri plats, beroende på vilken åtgärd du vill utföra. Frågemodelleraren öppnas med en tom arbetsyta. Klicka på **+** för att konfigurera den första noden i frågan.

Du kan lägga till två typer av element:

* **Filtrera komponenter** (Anpassat villkor, Välj målgrupp, Fördefinierat filter) låter dig skapa egna regler, välja en målgrupp eller ett fördefinierat filter för att förfina din fråga. [Lär dig hur du arbetar med filterkomponenter](#filtering)

  Exempel:

  *Mottagare som prenumererar på nyhetsbrevet Sports*. *Mottagare som bor i New York*, *Mottagare som bor i San Francisco*

* **Gruppoperatorer** (AND, OR, EXCEPT) gör att du kan gruppera filterkomponenter i diagrammet efter behov. [Lär dig arbeta med operatorer](#filtering)

  Exempel:

  *Mottagare som prenumererar på nyhetsbrevet Sports **OCH**som bor i New York **ELLER**San Francisco*.

![](assets/query-add-component.png)

## Lägga till filterkomponenter {#filtering}

Med filterkomponenter kan du förfina frågan genom att använda:

* **Anpassade villkor**: Filtrera frågan genom att skapa ett eget villkor med attribut från databasen och avancerade uttryck.
* **Målgrupper**: Filtrera frågan med en befintlig målgrupp.
* **Fördefinierat filter**: Filtrera frågan med befintliga fördefinierade filter.

### Konfigurera ett anpassat villkor

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Anpassat villkor"
>abstract="Anpassat villkor"

Så här filtrerar du frågan med ett anpassat villkor:

1. Klicka på **+** på önskad nod och välj **[!UICONTROL Custom condition]**. Rutan för anpassade villkorsegenskaper öppnas till höger.

1. I **Attribut** väljer du attributet från databasen som du vill använda för att skapa villkoret. Attributlistan innehåller alla attribut från Campaign-databasen, inklusive attribut som är länkade till din tabell.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Med knappen Redigera uttryck kan du använda redigeraren för Campaign-webbuttryck för att manuellt definiera ett uttryck med hjälp av fält från databasen och hjälpfunktionerna.

1. Välj den operator som ska användas i listrutan. Olika operatorer är tillgängliga för användning. Observera att operatorer som är tillgängliga i listrutan beror på attributets datatyp.

   +++Lista över tillgängliga operatorer

   | Operatör | Syfte | Exempel |
   |  ---  |  ---  |  ---  |
   | Lika med | Returnerar ett resultat som är identiskt med de data som anges i den andra värdekolumnen. | Efternamnet (@lastName) är lika med &#39;Jones&#39;, returnerar bara mottagare vars efternamn är Jones. |
   | Inte lika med | Returnerar alla värden som inte är identiska med det angivna värdet. | Språk (@language) till samma som &quot;English&quot; |
   | Större än | Returnerar ett värde som är större än det angivna värdet. | Ålder (@age) större än 50</strong>, returnerar alla värden som är större än &quot;50&quot;, dvs. &quot;51&quot;, &quot;52&quot; osv. |
   | Mindre än | Returnerar ett värde som är mindre än det angivna värdet. | Skapad (@created) före &#39;DaysAgo(100)&#39;</strong>, returnerar alla mottagare som skapades för mindre än 100 dagar sedan. |
   | Större än eller lika med | Returnerar alla värden som är lika med eller större än det angivna värdet. | Ålder (@age) större än eller lika med 30</strong>, returnerar alla mottagare som är 30 år eller äldre. |
   | Mindre än eller lika med | Returnerar alla värden som är lika med eller lägre än det angivna värdet. | Ålder (@age) mindre än eller lika med 60</strong>, returnerar alla mottagare som är 60 år eller yngre. |
   | Ingår i | Returnerar resultat som ingår i de angivna värdena. Dessa värden måste avgränsas med kommatecken. | Födelsedatum (@BirthDate) ingår i &quot;12/10/1979, 12/10/1984&quot;, returnerar de mottagare som är födda mellan dessa datum. |
   | Inte i | Fungerar som operatorn Inkluderad i. Här vill vi exkludera mottagare baserat på de angivna värdena. | Födelsedatum (@BirthDate) ingår inte i &#39;12/10/1979,12/10/1984&#39;. Till skillnad från i föregående exempel returneras inte mottagare som fötts inom dessa datum. |
   | Är tom | I det här fallet matchar resultatet vi söker efter ett tomt värde i den andra värdekolumnen. | Mobilen (@mobilePhone) är tom returnerar alla mottagare som inte har något mobilnummer. |
   | Är inte tom | Fungerar i motsatt riktning till operatorn Är tom. Du behöver inte ange data i den andra värdekolumnen. | E-postadressen (@email) är inte tom. |
   | Börjar med | Returnerar resultatet med början på det angivna värdet. | Kontonr (@account) börjar med 32010. |
   | Börjar inte med | Returnerar resultat som inte börjar med det angivna värdet | Kontonr (@account) börjar inte med 20 |
   | Innehåller | Returnerar resultatet som innehåller minst det angivna värdet. | E-postdomänen (@domain) innehåller &#39;mail&#39;</strong>, returnerar alla domännamn som innehåller &quot;mail&quot;. Domänen gmail.com returneras alltså också. |
   | Innehåller inte | Returnerar resultat som inte innehåller det angivna värdet. | E-postdomänen (@domain) innehåller inte &#39;vo&#39;</strong>. I det här fallet returneras inte domännamn som innehåller &quot;vo&quot;. Domännamnet voila.fr visas inte i resultatet. |
   | Gilla | Liknar mycket operatorn Contains. Du kan infoga ett % jokertecken i värdet. | Efternamn (@lastName) som &#39;Jon%s&#39;. Här används jokertecknet som&quot;joker&quot; för att hitta namnet&quot;Jones&quot;, om operatorn hade glömt den saknade bokstaven mellan&quot;n&quot; och&quot;s&quot;. |
   | Inte som | Liknar mycket operatorn Contains. Du kan infoga ett % jokertecken i värdet. | Efternamnet (@lastName) är inte som Smi%h. Här returneras inte mottagare vars efternamn är Smi%h. |

+++

1. I **Värde** definierar du det förväntade värdet. Du kan också använda redigeringsprogrammet för webbuttryck i Campaign för att manuellt definiera ett uttryck med hjälp av fält från databasen och hjälpfunktionerna. Klicka på **Redigera uttryck** -knappen.

   *Frågeexempel som returnerar alla profiler som är 21 år eller äldre:*

   ![](assets/query-custom-condition.png)

**Anpassade villkor i fjärrtabeller (1-1- och 1-N-länkar)**

Anpassade villkor gör att du kan fråga fjärrtabeller som är länkade till mottagartabellen.

För **1-1 länk** med en annan databasresurs väljer du värdet direkt från måltabellen.

+++Exempel på fråga

Här är frågan riktad till mottagare vars land eller region ingår i angivna värden (uk och us)

![](assets/custom-condition-1-1.png)

+++

För **1-N-länk** med en annan databasresurs kan du definiera undervillkor för fälten i den här andra resursen.

Du kan till exempel välja operatorn Exists på profilinköpen för att ange alla profiler som det finns inköp för som mål. När du är klar lägger du till ett anpassat villkor för den utgående övergången och skapar ett filter som passar dina behov.

+++Exempel på fråga

Här riktar frågan sig till mottagare som har gjort inköp relaterade till BrewMaster-produkten, med ett totalt belopp på minst 100$.

![](assets/custom-condition-1-N.png)

+++

### Välj en målgrupp

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Välj målgrupp"
>abstract="Välj målgrupp"

Så här filtrerar du frågan med en befintlig målgrupp:

1. Klicka på **+** på önskad nod och välj **[!UICONTROL Select audience]**.

1. The **Välj målgrupp** egenskapspanelen öppnas till höger. Välj den målgrupp som du vill använda för att filtrera frågan.

   *Frågeexempel som returnerar alla profiler som tillhör målgruppen Festival Goers:*

   ![](assets/query-audience.png)

### Använda ett fördefinierat filter

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Fördefinierat filter"
>abstract="Fördefinierat filter"

Så här filtrerar du frågan med ett fördefinierat filter:

1. Klicka på **+** på önskad nod och välj **[!UICONTROL Predefined filter]**.

1. The **Fördefinierat filter** egenskapspanelen öppnas till höger. Välj ett fördefinierat filter i listan med anpassade filter eller bland favoriter.

   *Frågeexempel som returnerar alla profiler som motsvarar det fördefinierade filtret &quot;Inaktiva kunder&quot;:*

   ![](assets/query-predefined-filter.png)

## Kombinera filterkomponenter med operatorer {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Grupp"
>abstract="Grupp"

Varje gång du lägger till en ny filterkomponent i frågan länkas den automatiskt till den andra komponenten av en AND-operator. Detta innebär att resultat från båda filterkomponenterna kombineras med frågeresultaten.

I det här exemplet har vi lagt till en ny filtreringskomponent av publiktyp i den andra övergången. Komponenten är länkad till det fördefinierade filtertypsvillkoret med en AND-operator, vilket innebär att frågeresultatet innehåller mottagare som har det fördefinierade Madridians-filtret OCH som tillhör målgruppen&quot;Rabattväljare&quot;.

![](assets/query-operator.png)

Om du vill ändra operatorn som används för att länka samman filtervillkoren klickar du på den och väljer önskad operator i grupprutan som öppnas till höger.

Tillgängliga operatorer:

* **OCH (skärning)**: Kombinerar resultat som matchar alla filterkomponenter i utgående övergångar.
* **OR (Union)**: Innehåller resultat som matchar minst en av filterkomponenterna i utgående övergångar.
* **UTOM (Uteslutning)**: Utesluter resultat som matchar alla filterkomponenter i den utgående övergången.

![](assets/query-operator-change.png)

## Kontrollera och validera frågan

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Regelegenskaper"
>abstract="Regelegenskaper"

När du har skapat frågan på arbetsytan kan du kontrollera den med **Regelegenskaper** rutan till höger. Tillgängliga åtgärder är:

* **Visa resultat:** Visar de data som är resultatet av din fråga.
* **kodvyn**: Visar en kodbaserad version av frågan i SQL.
* **Beräkna**: Uppdaterar och visar antalet poster som frågan riktar sig till.
* **Markera eller spara filter**: Välj ett befintligt fördefinierat filter som ska användas på arbetsytan eller spara frågan som ett fördefinierat filter för framtida återanvändning. [Lär dig hur du arbetar med fördefinierade filter](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Välj ett fördefinierat filter i rutan Regelegenskaper om du vill ersätta frågan som har byggts in på arbetsytan med det valda filtret.
