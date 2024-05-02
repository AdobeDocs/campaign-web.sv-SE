---
audience: end-user
title: Använd aktiviteten Överför fil
description: Lär dig hur du använder arbetsflödesaktiviteten Överför fil
source-git-commit: 6fe8be5510e13cdb9e9e1bce44aadb80619275e4
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 8%

---

# För över fil {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="För över fil"
>abstract="The **Överföringsfil** kan du ta emot eller skicka filer, testa om det finns filer eller lista med filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Alternativ för filöverföring"
>abstract="Alternativ för filöverföring"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Filöverföringsaktivitet"
>abstract="Filöverföringsaktivitet"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Fjärrserver för överföringsfil"
>abstract="Fjärrserver för överföringsfil"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Överför filkälla"
>abstract="Överför filkälla"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Ta bort källfilerna efter överföringen"
>abstract="Ta bort källfilerna efter överföringen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Visa sessionsloggarna"
>abstract="Visa sessionsloggarna"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Visa alla filer"
>abstract="Visa alla filer"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Filhistorik"
>abstract="Filhistorik"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Bearbeta saknade filer"
>abstract="Bearbeta saknade filer"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Processfel"
>abstract="Processfel"

The **Överföringsfil** aktiviteten är en **Datahantering** aktivitet. Du kan ta emot eller skicka filer, testa om det finns filer eller lista med filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll.

>[!NOTE]
>
>Med Campaign Web User Interface har vi konsoliderat två aktiviteter till en genom att slå samman båda **Filöverföring** och **Webbnedladdning** funktioner. Denna konsolidering påverkar inte aktivitetens funktion på något sätt.

Följ stegen nedan för att konfigurera **Överföringsfil** aktivitet.

## Välj överföringsprotokoll och -åtgärd {#protocol}

1. Lägg till en **Överföringsfil** anger du vilken typ av överföring som ska utföras beroende på vilket protokoll du vill använda:

   * För HTTP-protokoll väljer du **[!UICONTROL Web Download]**. På så sätt kan du utföra en GET- eller POST-hämtning av en fil på en explicit URL, ett externt konto eller en Adobe Campaign-instans.
   * För andra server-till-server-protokoll och relaterade åtgärder väljer du **[!UICONTROL File transfer]**.

1. Välj vilken åtgärd som ska utföras med aktiviteten. Vilka åtgärder som är tillgängliga beror på vilken typ av överföring du har valt. Expandera avsnitten nedan om du vill ha mer information.

   +++Åtgärder tillgängliga med **Filöverföring** typverksamhet

   * **[!UICONTROL File download]**: Hämta en fil från servern.
   * **[!UICONTROL File upload]**: Överför en fil till servern.
   * **[!UICONTROL Test to see if file exists]**: Kontrollera om det finns en viss fil på servern. Genererar två utgående övergångar efter aktiviteten: &quot;Filen finns&quot; och &quot;filen finns inte&quot;.
   * **[!UICONTROL File listing]**: Lista alla filer som är tillgängliga på servern.

+++

   +++Åtgärder tillgängliga med **Webbnedladdning** typverksamhet

   * **[!UICONTROL Simple transfer (GET)]**: Hämta en fil.
   * **[!UICONTROL Transfer using a form (POST)]**: Överför en fil och ytterligare parametrar.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. Som standard används den fil som har angetts i föregående aktivitet för filöverföringsåtgärder. Om du vill använda en annan fil växlar du **[!UICONTROL Use file from previous activity]** avaktivera och klicka på **[!UICONTROL Add file]** -knappen.

   I **[!UICONTROL Source]** anger du önskat filnamn eller använder uttrycksredigeraren för att beräkna filnamnet med hjälp av händelsemariabler. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md). Upprepa åtgärden för att lägga till så många filer som behövs.

## Definiera överföringsmålet {#destination}

1. I **[!UICONTROL Remote server]** anger du vilken server som ska anslutas på något av följande sätt:

   * **[!UICONTROL Use connection parameters defined in an external account]**: Anslut till en server med anslutningsparametrarna för ett externt konto. I **[!UICONTROL Server folder]** anger du sökvägen till filen (eller till mappen för fillisteåtgärder).
   * **[!UICONTROL Quick configuration]**: Ange URL-adressen till filen (eller mappen för fillisteåtgärder).
   * **[!UICONTROL Adobe Campaign instance]** (Webbhämtningstypaktiviteter): Hämta en fil från en Adobe Campaign-instansserver.

   ![](../assets/workflow-transfer-file-server.png)

1. För åtgärder för hämtning av POST för webben kan du skicka ytterligare parametrar med åtgärden. Klicka på **[!UICONTROL Add parameter]** anger sedan parameterns namn och värde. Du kan lägga till så många parametrar som behövs.

1. Som standard sparas de filer som överförs på en server automatiskt vid filöverföring. Om du inte vill behålla den här historiken växlar du **[!UICONTROL Keep history of files sent]** avaktiverat.

## Historikinställningar {#historization}

Varje gång en **[!UICONTROL Transfer file]**-aktivitet körs så sparas de överförda eller hämtade filerna i en dedikerad mapp. En mapp skapas för varje överföringsfilaktivitet i ett arbetsflöde. Som standard sparas filerna i standardlagringskatalogen för Adobe Campaign-installationsmappen (`/vars`) innan den bearbetas. Om du vill använda en viss mapp växlar du **[!UICONTROL Use a default storage directory]** och ange sökvägen till katalogen.

![](../assets/workflow-transfer-file-historization.png)

Det är viktigt att du kan begränsa storleken på den här mappen för att bevara det fysiska utrymmet på servern. Det gör du genom att definiera ett maximalt antal filer eller en total storlek för aktivitetens mapp. Som standard så är 100 filer och 50 MB tillåtet.

Varje gång aktiviteten körs så kontrolleras mappen enligt följande:

* Endast filer som skapats mer än 24 timmar innan aktiviteten kördes tas med i beräkningen.
* Om antalet filer som ska beaktas är större än värdet för **[!UICONTROL Number of files]** i tas de äldsta filerna bort tills det maximala antalet filer har uppnåtts.
* Om den totala storleken på de filer som beaktas är större än värdet på **[!UICONTROL Maximum size (in MB)]** -parametern tas de äldsta filerna bort tills den största tillåtna storleken (i MB) nås.

>[!CAUTION]
>
>Om aktiviteten inte körs igen så kontrolleras eller rensas inte dess mapp. Var därför försiktig när du överför stora filer.

## Avancerade alternativ för felhantering {#advanced}

1. I **[!UICONTROL Advanced options]**, finns det ytterligare alternativ som baseras på den typ av aktivitet som du konfigurerar. Expandera avsnitten nedan om du vill ha mer information.

   +++Fler alternativ för **[!UICONTROL File transfer]** typverksamhet

   * **[!UICONTROL Delete the source files after transfer]**: Radera källfilerna efter en slutförd överföring.
   * **[!UICONTROL Display the session logs]**: När det här alternativet är aktiverat visas information om överföringsåtgärden i arbetsflödesloggarna när arbetsflödet har körts.
   * **[!UICONTROL List all files]** (Fillistningsåtgärder): Det här alternativet indexerar alla filer som finns på servern i `vars.filenames` händelsevariabel, där filnamnen avgränsas med `n` tecken. [Lär dig hur du arbetar med händelsevariabler](../event-variables.md)

+++

   +++Fler alternativ för **[!UICONTROL Web download]** typverksamhet

   * **[!UICONTROL Follow redirections]**: Med filomdirigering kan du använda åsidosättningar för att dirigera datainmatning eller utdata till en enhet av en annan typ.
   * **[!UICONTROL Add the HTTP headers to the file]**: I vissa fall kanske du vill lägga till ytterligare HTTP-huvuden i en fil. Vanligtvis används dessa rubriker för att ge ytterligare information i felsökningssyfte, för [Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS)eller för att ange specifika cachelagringsdirektiv.
   * **[!UICONTROL Ignore the HTTP return code]**: HTTP-returkoder, som också kallas HTTP-statuskoder, visar resultatet av en HTTP-begäran.

1. The **[!UICONTROL Process errors]** kan du aktivera en utgående Error-övergång efter aktiviteten om något fel inträffar under överföringen.

   Dessutom, för **Filöverföring** typsnittsverksamhet, **[!UICONTROL Process missing file]** kan du aktivera en utgående övergång av typen &quot;Ingen fil&quot; efter aktiviteten om filen inte är tillgänglig på den angivna sökvägen.
