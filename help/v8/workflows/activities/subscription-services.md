---
audience: end-user
title: Använd aktiviteten Prenumerationstjänster
description: Lär dig använda arbetsflödesaktiviteten för prenumerationstjänster
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 15%

---

# Prenumerationstjänster {#subscription-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Aktivitet för prenumerationstjänster"
>abstract="Med aktiviteten Prenumerationstjänster kan flera profiler prenumereras på eller avbeställas från en tjänst i en enda åtgärd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Allmänna parametrar för prenumerationstjänst"
>abstract="Välj önskad tjänst och vilken åtgärd som ska utföras (prenumeration eller avprenumeration). Aktivera alternativet **Skicka bekräftelsemeddelande** för att meddela populationen att de prenumererar eller avbryter prenumerationen på den valda tjänsten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Generera en utgående övergång"
>abstract="Växla alternativet **Generera en utgående övergång** för att lägga till en övergång efter aktiviteten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="Ytterligare information"
>abstract="Ange prenumerationens data och ursprung för varje post. Du kan lämna det här avsnittet tomt. I så fall kommer inget datum eller ursprung att anges när arbetsflödet körs. Om inkommande data innehåller en kolumn som anger prenumerationsdatumet för profilen för tjänsten kan du markera den i fältet **[!UICONTROL Date]**. Ange prenumerationens ursprung i fältet **[!UICONTROL Origin path]**. Du kan ställa in den på ett av fälten för inkommande data eller på ett valfritt konstant värde genom att markera alternativet **[!UICONTROL Set a constant as origin]**."

Aktiviteten **Prenumerationstjänster** är en **datahanteringsaktivitet**. Du kan skapa eller ta bort en prenumeration på en informationstjänst för den population som anges i övergången.

## Konfigurera aktiviteten för prenumerationstjänster {#subscription-services-configuration}

Så här konfigurerar du aktiviteten **Prenumerationstjänster**:

1. Lägg till en **prenumerationstjänstaktivitet** i ditt arbetsflöde. Du kan använda den här aktiviteten efter att du har angett profiler som mål eller importerat en fil med identifierade data.

1. Välj den tjänst som du vill hantera prenumerationerna för med något av följande alternativ:

   * **[!UICONTROL Select a specific service]**: Välj en tjänst manuellt i fältet **[!UICONTROL Service]**.

   * **[!UICONTROL From inbound transition]**: Använd tjänsten som anges i övergången för inkommande trafik. Du kan till exempel importera en fil som anger vilken tjänst som ska hanteras för varje rad. Den tjänst som åtgärden ska utföras på väljs sedan dynamiskt för varje profil.

   ![](../assets/workflow-subscription-service.png)

1. Välj åtgärden som ska utföras: **Prenumerera** eller **Avsluta prenumerationen**.

   Om tjänsten definieras i den inkommande övergången kan du välja hur du vill hämta den här åtgärden:

   * **Välj en specifik åtgärdstyp**: Välj åtgärden som ska utföras manuellt (**Prenumerera** eller **Avsluta prenumeration**)

   * **Välj en åtgärdstyp från en sökväg till en inkommande övergång**: Markera den kolumn med inkommande data som anger vilken åtgärd som ska utföras för varje post. Du kan till exempel importera en fil som anger vilken åtgärd som ska utföras för varje rad i en åtgärdskolumn.

     Endast booleska fält och heltalsfält kan väljas här. Se till att de data som innehåller åtgärden som ska utföras matchar detta format. Om du till exempel läser in data från en inläsningsfilsaktivitet, kontrollerar du att du har angett korrekt format för kolumnen som innehåller åtgärden i aktiviteten **[!UICONTROL Load file]**. Ett exempel visas i [det här avsnittet](#uc2).

     >[!CAUTION]
     >
     >Om du väljer det här alternativet förväntas som standard en länkdefinition till tabellen **Tjänster (nms)** i arbetsflödet finnas för aktiviteten **Prenumerationstjänster**. Det gör du genom att kontrollera att du har konfigurerat en avstämningslänk uppåt i en **anrikningsaktivitet** i arbetsflödet. Ett exempel som visar hur du använder det här alternativet finns [här](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Om du vill meddela mottagarna att de prenumererar på eller avbryter prenumerationen på den valda tjänsten aktiverar du alternativet **[!UICONTROL Send a confirmation message]**. Innehållet i det här meddelandet definieras i en leveransmall som är kopplad till informationstjänsten.

1. Om du använder data från en inkommande övergång visas ett **[!UICONTROL Additional information]**-avsnitt som gör att du kan ange prenumerationens data och ursprung för varje post. Du kan lämna det här avsnittet tomt. I så fall kommer inget datum eller ursprung att anges när arbetsflödet körs.

   * Om inkommande data innehåller en kolumn som anger prenumerationsdatumet för profilen för tjänsten kan du markera den i fältet **[!UICONTROL Date]**.

   * Ange prenumerationens ursprung i fältet **[!UICONTROL Origin path]**. Du kan ställa in den på ett av fälten för inkommande data eller på ett valfritt konstant värde genom att markera alternativet **[!UICONTROL Set a constant as origin]**.

   ![](../assets/workflow-subscription-service-additional.png)

1. Om du vill lägga till en utgående övergång efter aktiviteten aktiverar du alternativet **[!UICONTROL Generate an outbound transition]**.

## Exempel {#example}

### Prenumerera på en viss tjänst {#uc1}

Det här arbetsflödet nedan visar hur du prenumererar på en befintlig tjänst.

![](../assets/workflow-subscription-service-uc1.png)

* En **[!UICONTROL Build audience]**-aktivitet har en befintlig målgrupp som mål.

* Med en **[!UICONTROL Subscription Services]**-aktivitet kan du välja den tjänst som profilerna ska prenumerera på.

### Uppdatera flera prenumerationsstatusar från en fil {#uc2}

Arbetsflödet nedan visar hur du importerar en fil som innehåller profiler och uppdaterar deras prenumeration till flera tjänster som anges i filen.

![](../assets/workflow-subscription-service-uc2.png)

* En **[!UICONTROL Load file]**-aktivitet läser in en CSV-fil som innehåller data och definierar strukturen för de importerade kolumnerna. Kolumnerna &quot;tjänst&quot; och &quot;åtgärd&quot; anger vilken tjänst som ska uppdateras och vilken åtgärd som ska utföras (prenumeration eller avprenumeration).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Som du kanske har märkt anges åtgärden i filen som &quot;sub&quot; eller &quot;unsub&quot;. Systemet förväntar sig ett **booleskt värde** eller **heltalsvärde** som identifierar åtgärden som ska utföras: &quot;0&quot; för att avprenumerera och &quot;1&quot; för att prenumerera. För att matcha detta krav:
   * **Datatypen** för åtgärdskolumnen är inställd på heltal.
   * En **värdeommappning** måste utföras för att matcha värdena för sub och unsub med värdena 1 och 0.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Om filen redan använder &quot;0&quot; och &quot;1&quot; för att identifiera operationen behöver du inte mappa om dessa värden. Kontrollera bara att kolumnen bearbetas som **Boolean** eller **Integer** i exempelfilkolumnerna.

* En **[!UICONTROL Reconciliation]**-aktivitet identifierar att data från filen tillhör profildimensionen i Adobe Campaign-databasen. Fältet **email** i filen matchar fältet **email** i profilresursen.

  ![](../assets/workflow-subscription-service-uc2-reconciliation.png)

* En **[!UICONTROL Enrichment]**-aktivitet skapar en avstämningslänk till tabellen Tjänster (nms), med en enkel koppling mellan kolumnen Tjänst i den överförda filen och tjänstens fält för internt namn i databasen.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* En **[!UICONTROL Subscription Services]** identifierar de tjänster som ska uppdateras från övergången.

  **[!UICONTROL Operation type]** identifieras som att det kommer från fältet **operation** i filen. Endast fälten Booleskt värde eller Heltalsvärde kan markeras här. Om kolumnen i filen som innehåller åtgärden som ska utföras inte visas i listan, ska du kontrollera att du har angett kolumnformatet korrekt i **[!UICONTROL Load file]**-aktiviteten, vilket förklaras ovan i det här exemplet.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
