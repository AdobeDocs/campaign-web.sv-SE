---
audience: end-user
title: Lägg till visuella fragment i e-postmeddelanden
description: Lär dig hur du lägger till visuella fragment i e-postmeddelanden
hide: true
hidefromtoc: true
source-git-commit: 341e2a5ab073405d3be19068f85b9ea917b32a69
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# Lägg till visuella fragment i e-postmeddelanden {#use-visual-fragments}

Du kan använda ett visuellt fragment i en [e-postleverans](get-started-email-designer.md)eller i en [innehållsmall](use-email-templates.md). Stegen beskrivs nedan.


>[!NOTE]
>
>Lär dig hur du skapar och hanterar fragment i [det här avsnittet](fragments.md).


## Använda ett fragment {#use-fragment}

Följ stegen nedan om du vill infoga ett fragment i ett e-postinnehåll:

1. Öppna e-post- eller mallinnehåll med [E-postdesigner](get-started-email-designer.md).

1. Välj **[!UICONTROL Fragments]** ikonen från den vänstra listen.

   ![](assets/fragments-in-designer.png)

1. Listan över alla visuella fragment som skapats i den aktuella sandlådan visas. Du kan:

   * Sök efter ett visst fragment genom att börja skriva dess etikett.
   * Sortera fragment i stigande eller fallande ordning.
   * Ändra hur fragmenten visas (kort eller listvy).

   >[!NOTE]
   >
   >Fragment sorteras efter skapandedatum: nyligen tillagda visuella fragment visas först i listan.

   Om några fragment har ändrats eller lagts till medan du redigerar ditt innehåll klickar du på **Uppdatera** om du vill uppdatera listan med de senaste ändringarna.

1. Dra och släpp ett fragment från listan till området där du vill infoga det. Precis som andra komponenter kan du flytta runt fragmentet i innehållet.

1. Markera fragmentet för att visa dess alternativ i den högra rutan.

   ![](assets/fragment-right-pane.png)

   Från **[!UICONTROL Settings]** kan du

   * Välj de enheter som du vill att fragmentet ska visas på.
   * Öppna fragmentet på en ny flik om du vill redigera det. [Läs mer](../email/fragments.md#edit-fragments)

   Du kan anpassa fragmentet ytterligare med **[!UICONTROL Styles]** -fliken.

1. Vid behov kan du bryta arvet med det ursprungliga fragmentet. [Läs mer](#break-inheritance)
Du kan också ta bort fragmentet från innehållet eller duplicera det. Dessa åtgärder kan utföras direkt från den snabbmeny som visas ovanpå fragmentet.

1. Lägg till så många fragment du vill och **[!UICONTROL Save]** dina ändringar.

## Bryt arv {#break-inheritance}

När du redigerar ett visuellt fragment synkroniseras ändringarna. De sprids automatiskt till alla e-postleveranser och innehållsmallar som innehåller det fragmentet.

När fragment läggs till i ett e-postmeddelande eller i en innehållsmall synkroniseras de som standard.

Du kan emellertid bryta arvet från det ursprungliga fragmentet. I så fall kopieras fragmentets innehåll till den aktuella designen och ändringarna synkroniseras inte längre.

Följ stegen nedan för att bryta arv:

1. Markera fragmentet.

1. Klicka på upplåsningsikonen i det sammanhangsberoende verktygsfältet.

   ![](assets/fragment-break-inheritance.png)

1. Det fragmentet blir ett fristående element som inte längre är länkat till det ursprungliga fragmentet. Redigera det som vilken annan innehållskomponent som helst i innehållet. [Läs mer](content-components.md)
