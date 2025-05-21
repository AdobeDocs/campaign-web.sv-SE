---
audience: end-user
title: Använd aktiviteten Överför fil
description: Lär dig hur du använder arbetsflödesaktiviteten Överför fil
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 6%

---

# För över fil {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="För över fil"
>abstract="Med aktiviteten **Överför fil** kan du ta emot eller skicka filer, testa om det finns filer eller lista över filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll."

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
>abstract="Ange den server som ska anslutas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Överför filkälla"
>abstract="Ange önskat filnamn."

Aktiviteten **Överför fil** är en **datahanteringsaktivitet**. Du kan ta emot eller skicka filer, testa om det finns filer eller lista med filer på en server. Det protokoll som används kan antingen vara server-till-server-protokoll eller HTTP-protokoll.

>[!NOTE]
>
>Med Campaigns webbanvändargränssnitt har två aktiviteter konsoliderats till en genom att sammanfoga funktionerna för både **filöverföring** och **webbhämtning**. Denna konsolidering påverkar inte aktivitetens funktion på något sätt.

Följ stegen nedan för att konfigurera aktiviteten **Överför fil**.

## Välj överföringsprotokoll och -åtgärd {#protocol}

1. Lägg till en **överföringsfilaktivitet** i arbetsflödet och ange sedan vilken typ av överföring som ska utföras beroende på vilket protokoll du vill använda:

   * För HTTP-protokoll väljer du **[!UICONTROL Web Download]**. Detta gör att du kan utföra en GET- eller POST-åtgärd för att hämta en fil på en explicit URL, ett externt konto eller en Adobe Campaign-instans.
   * För andra server-till-server-protokoll och relaterade åtgärder väljer du **[!UICONTROL File transfer]**.

1. Välj vilken åtgärd som ska utföras med aktiviteten. Vilka åtgärder som är tillgängliga beror på vilken typ av överföring du har valt. Expandera avsnitten nedan om du vill ha mer information.

   +++Åtgärder tillgängliga med **filöverföringsaktiviteter**

   * **[!UICONTROL File download]**: Hämta en fil från servern.
   * **[!UICONTROL File upload]**: Överför en fil till servern.
   * **[!UICONTROL Test to see if file exists]**: Kontrollera om det finns en angiven fil på servern. Genererar två utgående övergångar efter aktiviteten: &quot;Fil finns&quot; och &quot;Fil finns inte&quot;.
   * **[!UICONTROL File listing]**: Visa alla filer som är tillgängliga på servern.

+++

   +++Åtgärder tillgängliga med aktiviteter av typen **Webbhämtning**

   * **[!UICONTROL Simple transfer (GET)]**: Hämta en fil.
   * **[!UICONTROL Transfer using a form (POST)]**: Överför en fil och ytterligare parametrar.

+++

   ![Skärmbild som visar alternativ för filöverföringsåtgärd i arbetsflödet](../assets/workflow-transfer-file-action.png)

1. Som standard används den fil som har angetts i föregående aktivitet för filöverföringsåtgärder. Om du vill använda en annan fil inaktiverar du alternativet **[!UICONTROL Use file from previous activity]** och klickar på knappen **[!UICONTROL Add file]**.

   I fältet **[!UICONTROL Source]** anger du det önskade filnamnet eller använder uttrycksredigeraren för att beräkna filnamnet med hjälp av händelsevariabler. [Lär dig hur du arbetar med händelsevariabler och uttrycksredigeraren](../event-variables.md). Upprepa åtgärden för att lägga till så många filer som behövs.

## Definiera överföringsmålet {#destination}

1. I avsnittet **[!UICONTROL Remote server]** anger du vilken server som ska anslutas på något av följande sätt:

   * **[!UICONTROL Use connection parameters defined in an external account]**: Anslut till en server med anslutningsparametrarna för ett externt konto. I fältet **[!UICONTROL Server folder]** anger du sökvägen till filen (eller till mappen för fillisteåtgärder).
   * **[!UICONTROL Quick configuration]**: Ange filens (eller mappens) URL-adress för fillisteåtgärder.
   * **[!UICONTROL Adobe Campaign instance]** (typaktiviteter för webbnedladdning): Hämta en fil från en Adobe Campaign-instansserver.

   ![Skärmbild som visar konfigurationsalternativ för filserver för arbetsflödesöverföring](../assets/workflow-transfer-file-server.png)

1. För Web download POST-åtgärder kan du skicka ytterligare parametrar med åtgärden. Det gör du genom att klicka på knappen **[!UICONTROL Add parameter]** och sedan ange parameterns namn och värde. Du kan lägga till så många parametrar som behövs.

1. Som standard sparas de filer som överförs till en server automatiskt vid filöverföring. Om du inte vill behålla den här historiken inaktiverar du alternativet **[!UICONTROL Keep history of files sent]**.

## Historikinställningar {#historization}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Filhistorik"
>abstract="Varje gång en **[!UICONTROL Transfer file]**-aktivitet körs så sparas de överförda eller hämtade filerna i en dedikerad mapp. En mapp skapas för varje överföringsfilaktivitet i ett arbetsflöde. Som standard sparas filer i standardlagringskatalogen för Adobe Campaign-installationsmappen (`/vars`) innan de bearbetas. Om du vill använda en viss mapp avaktiverar du alternativet **[!UICONTROL Use a default storage directory]** och anger sökvägen till katalogen."

Varje gång en **[!UICONTROL Transfer file]**-aktivitet körs så sparas de överförda eller hämtade filerna i en dedikerad mapp. En mapp skapas för varje överföringsfilaktivitet i ett arbetsflöde. Som standard sparas filer i standardlagringskatalogen för Adobe Campaign-installationsmappen (`/vars`) innan de bearbetas. Om du vill använda en viss mapp avaktiverar du alternativet **[!UICONTROL Use a default storage directory]** och anger sökvägen till katalogen.

![Skärmbild som visar inställningar för historik för filöverföring i arbetsflödet](../assets/workflow-transfer-file-historization.png)

Det är viktigt att begränsa storleken på den här mappen för att bevara det fysiska utrymmet på servern. Det gör du genom att definiera ett maximalt antal filer eller en total storlek för aktivitetsmappen. Som standard så är 100 filer och 50 MB tillåtet.

Varje gång aktiviteten körs så kontrolleras mappen enligt följande:

* Endast filer som skapats mer än 24 timmar innan aktiviteten kördes tas med i beräkningen.
* Om antalet filer som ska beaktas överstiger värdet för fältet **[!UICONTROL Number of files]** tas de äldsta filerna bort tills det högsta antalet tillåtna filer har uppnåtts.
* Om den totala storleken på de filer som beaktas överskrider värdet för parametern **[!UICONTROL Maximum size (in MB)]** tas de äldsta filerna bort tills den största tillåtna storleken nås.

>[!CAUTION]
>
>Om aktiviteten inte körs igen kontrolleras eller rensas inte dess mapp. Var försiktig när du överför stora filer.

## Avancerade alternativ för felhantering {#advanced}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Ta bort källfilerna efter överföringen"
>abstract="Radera källfilerna när överföringen är klar."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Visa sessionsloggarna"
>abstract="Information om överföringsåtgärden visas i arbetsflödesloggarna."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Visa alla filer"
>abstract="Det här alternativet indexerar alla filer som finns på servern i händelsevariabeln **vars.filenames** ."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Bearbeta saknade filer"
>abstract="Med det här alternativet kan du aktivera en utgående övergång av typen **Ingen fil** efter aktiviteten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Processfel"
>abstract="Med det här alternativet kan du aktivera en utgående **Error**-övergång efter aktiviteten."

1. I **[!UICONTROL Advanced options]** finns ytterligare alternativ tillgängliga baserat på den typ av aktivitet som du konfigurerar. Expandera avsnitten nedan om du vill ha mer information.

   +++Ytterligare alternativ för **[!UICONTROL File transfer]**-typaktiviteter

   * **[!UICONTROL Delete the source files after transfer]**: Radera källfilerna efter en slutförd överföring.
   * **[!UICONTROL Display the session logs]**: När det här alternativet aktiveras visas information om överföringsåtgärden i arbetsflödesloggarna när arbetsflödet har körts.
   * **[!UICONTROL List all files]** (Filliståtgärder): Det här alternativet indexerar alla filer som finns på servern i `vars.filenames` -händelsevariabeln, där filnamnen avgränsas med `n`-tecknen. [Lär dig hur du arbetar med händelsevariabler](../event-variables.md)

+++

   +++Ytterligare alternativ för **[!UICONTROL Web download]**-typaktiviteter

   * **[!UICONTROL Follow redirections]**: Med filomdirigering kan du använda åsidosättningar för att dirigera dataindata eller utdata till en enhet av en annan typ.
   * **[!UICONTROL Add the HTTP headers to the file]**: I vissa fall kanske du vill lägga till ytterligare HTTP-huvuden i en fil. Vanligtvis används dessa rubriker för att tillhandahålla ytterligare information i felsökningssyfte, för [Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS) eller för att ange specifika cachelagringsdirektiv.
   * **[!UICONTROL Ignore the HTTP return code]**: HTTP-returkoder, som också kallas HTTP-statuskoder, anger resultatet av en HTTP-begäran.

1. Med alternativet **[!UICONTROL Process errors]** kan du aktivera en utgående felövergång efter aktiviteten om något fel inträffar under överföringen.

   För aktiviteter av typen **Filöverföring** kan du med alternativet **[!UICONTROL Process missing file]** dessutom aktivera en utgående övergång utan fil efter aktiviteten om filen inte är tillgänglig på den angivna sökvägen.