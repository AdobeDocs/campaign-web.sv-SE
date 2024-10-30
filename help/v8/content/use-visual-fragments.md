---
audience: end-user
title: Lägg till visuella fragment i e-postmeddelanden
description: Lär dig hur du lägger till visuella fragment i e-postmeddelanden
badge: label="Begränsad tillgänglighet"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 0b85b5a4b6eff4fdb9835a0d1ccb5d0a86c103a0
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# Lägg till visuella fragment i e-postmeddelanden {#use-visual-fragments}

>[!AVAILABILITY]
>
>Den här funktionen är begränsad tillgänglighet (LA). Den är begränsad till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

Du kan använda ett visuellt fragment i en [e-postleverans](../email/get-started-email-designer.md) eller i en [innehållsmall](../email/use-email-templates.md). Stegen beskrivs nedan. [Lär dig skapa och hantera innehållsfragment](fragments.md).

![](assets/fragments.gif)

## Använda ett visuellt fragment {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentalternativ"
>abstract="Den här rutan innehåller alternativ som är relaterade till det valda fragmentet. Du kan välja vilka enheter du vill att fragmentet ska visas på och öppna innehållet i det här fragmentet. Använd fliken **[!UICONTROL Styles]** för att anpassa fragmentet ytterligare. Du kan också bryta arvet med det ursprungliga visuella fragmentet."

<!-- pas vu dans l'UI-->

Följ stegen nedan om du vill infoga ett visuellt fragment i ett e-postinnehåll:

1. Öppna e-post- eller mallinnehåll med hjälp av [e-post-Designer](../email/get-started-email-designer.md).

1. Välj ikonen **[!UICONTROL Fragments]** i den vänstra listen.

   ![](assets/fragments-in-designer.png)

1. Listan över alla visuella fragment som skapats i den aktuella sandlådan visas. Du kan:

   * Sök efter ett visst fragment genom att börja skriva dess etikett.
   * Sortera fragment i stigande eller fallande ordning.
   * Ändra hur fragmenten visas (kort eller listvy).

   >[!NOTE]
   >
   >Fragment sorteras efter skapandedatum: nyligen tillagda fragment visas först i listan.

   Om några synliga fragment har ändrats eller lagts till medan du redigerar ditt innehåll klickar du på ikonen **Uppdatera** för att uppdatera listan med de senaste ändringarna.

1. Dra och släpp ett visuellt fragment från listan till området där du vill infoga det. Precis som andra komponenter kan du flytta runt fragmentet i innehållet.

1. Markera fragmentet för att visa dess alternativ i den högra rutan.

   ![](assets/fragment-right-pane.png)

   På fliken **[!UICONTROL Settings]** kan du:

   * Välj de enheter som du vill att fragmentet ska visas på.
   * Klicka på knappen **Redigera innehåll** för att öppna innehållet i det här fragmentet. [Läs mer](../content/fragments.md#edit-fragments)

     Du kan anpassa fragmentet ytterligare med fliken **[!UICONTROL Styles]**.

1. Vid behov kan du bryta arvet med det ursprungliga visuella fragmentet. [Läs mer](#break-inheritance)

   Du kan också ta bort fragmentet från innehållet eller duplicera det. Dessa åtgärder kan utföras direkt från den snabbmeny som visas ovanpå fragmentet.

1. Lägg till så många visuella fragment du vill och **[!UICONTROL Save]** dina ändringar.

### Visual fragment in read-only mode {#fragment-readonly}

Åtkomsträttigheter kan tillämpas på visuella fragment.

Om du inte har redigeringsbehörighet för ett visst visuellt fragment visas innehållsmallen i **skrivskyddat läge**. I det här fallet ersätts knappen **[!UICONTROL Edit content]** med knappen **[!UICONTROL View content]** så att du kan visa fragmentet utan att göra några ändringar.

![](assets/fragment-readonly.png){zoomable="yes"}

Som framgår nedan är alla funktionsikoner inaktiverade, vilket begränsar interaktionen till att endast visas.

![](assets/fragment-readonly-view.png){zoomable="yes"}

## Bryt arv {#break-inheritance}

När du redigerar ett visuellt fragment synkroniseras ändringarna. De sprids automatiskt till alla e-postleveranser och innehållsmallar som innehåller det fragmentet.

När fragment läggs till i ett e-postmeddelande eller i en innehållsmall synkroniseras de som standard.

Du kan emellertid bryta arvet från det ursprungliga fragmentet. I så fall kopieras fragmentets innehåll till den aktuella designen och ändringarna synkroniseras inte längre.

Följ stegen nedan för att bryta arv:

1. Markera det visuella fragmentet.

1. Klicka på upplåsningsikonen i det sammanhangsberoende verktygsfältet.

   ![](assets/fragment-break-inheritance.png)

1. Det fragmentet blir ett fristående element som inte längre är länkat till det ursprungliga fragmentet. Redigera det som vilken annan innehållskomponent som helst i innehållet. [Läs mer](../email/content-components.md)
