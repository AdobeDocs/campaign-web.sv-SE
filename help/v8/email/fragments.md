---
audience: end-user
title: Skapa innehållsfragment
description: Lär dig skapa med innehållsfragment
hidefromtoc: true
hide: true
source-git-commit: 341e2a5ab073405d3be19068f85b9ea917b32a69
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Skapa innehållsfragment {#fragments}


>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Definiera egna fragment"
>abstract="Ett fragment är en återanvändbar komponent som kan refereras i en eller flera e-postmeddelanden mellan kampanjer."

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Spara fragment"
>abstract="Spara fragment"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Definiera egna fragment"
>abstract="Ett fragment är en återanvändbar komponent som kan refereras i en eller flera e-postmeddelanden mellan kampanjer."

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragmentegenskaper"
>abstract="Fragmentegenskaper"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Typ av fragment"
>abstract="Välj fragmenttyp. För närvarande är endast visuella fragment tillgängliga för e-post."

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Definiera egna fragment"
>abstract="Ett fragment är en återanvändbar komponent som kan refereras i en eller flera e-postmeddelanden mellan kampanjer. Du kan också använda fragment i dina e-postmallar. För närvarande är endast visuella fragment tillgängliga."

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentdetaljer"
>abstract="Fragmentdetaljer"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="Definiera egna fragment"
>abstract="Ett fragment är en återanvändbar komponent som kan refereras i en eller flera e-postmeddelanden mellan kampanjer."

Ett fragment är en återanvändbar komponent som kan refereras i en eller flera e-postmeddelanden mellan kampanjer. När du ändrar ett fragment uppdateras allt innehåll som använder det.

Med den här funktionen kan man skapa flera anpassade innehållsblock som kan användas av marknadsföringsanvändare för att snabbt sammanställa e-postinnehåll i en förbättrad designprocess.

![](assets/fragments.gif)


Så här använder du fragment på bästa sätt:

* Skapa egna visuella fragment, enligt beskrivningen nedan.
* Använd dem så många gånger som behövs i ditt innehåll via e-postdesignern. Se [Lägg till visuella fragment i e-postmeddelanden](../email/use-visual-fragments.md).

## Skapa ett Visual fragment {#create-fragments}

Det finns två sätt att skapa fragment:

* Skapa ett fragment från grunden med **[!UICONTROL Fragments]** egen meny. [Lär dig mer](#create-from-scratch)

* När du utformar innehåll sparar du en del av innehållet som fragment. [Lär dig mer](#save-as-fragment)

När fragmentet har sparats kan det användas i ett e-postmeddelande eller i en e-postmall. Oavsett om du har skapat från grunden eller från ett befintligt innehåll kan du nu använda det här avsnittet när du skapar innehåll i Campaign. Se [Lägg till visuella fragment](../email/use-visual-fragments.md).

### Skapa ett fragment från grunden {#create-from-scratch}

Följ stegen nedan om du vill skapa ett fragment från grunden.

1. [Åtkomst till fragmentlistan](#access-manage-fragments) via **[!UICONTROL Content Management]** > **[!UICONTROL Fragments]** vänster meny.

   ![](assets/fragments-list.png)

1. Välj **[!UICONTROL Create fragment]**.

1. Ange fragmentets etikett.

   ![](assets/fragment-create.png)

1. Om det behövs kan du definiera ytterligare alternativ, till exempel fragmentets interna namn, dess mapp och en beskrivning.

   >[!NOTE]
   >
   >För tillfället kan du bara skapa visuella fragment.

1. Klicka på **Skapa** för att konfigurera fragmentets innehåll.

1. The [E-postdesigner](../email/get-started-email-designer.md) visas. Redigera innehåll efter behov, på samma sätt som du gör för alla e-postmeddelanden i en kampanj. Du kan lägga till bilder, länkar, anpassningsfält och dynamiskt innehåll.

   ![](assets/fragment-designer.png)

1. När fragmentet är klart klickar du **[!UICONTROL Save & close]**. Den läggs till i [fragmentlista](#access-manage-fragments).

Det här fragmentet är nu klart att användas när du skapar [e-post](../email/get-started-email-designer.md) eller [innehållsmall](use-email-templates.md) inom Campaign. [Lär dig mer](../email/use-visual-fragments.md)


### Spara ett innehåll som fragment {#save-as-fragment}

Allt e-postinnehåll kan sparas som fragment för framtida återanvändning. När du utformar en [innehållsmall](use-email-templates.md) eller en [e-post](../email/get-started-email-designer.md) kan du spara en del av innehållet som ett visuellt fragment. Gör så här:

1. I [E-postdesigner](../email/get-started-email-designer.md)klickar du på **Mer** överst till höger på skärmen.

1. Välj **[!UICONTROL Save as fragment]** i listrutan.

   ![](assets/fragment-save-as.png)

1. The **[!UICONTROL Save as fragment]** visas. Här väljer du de element som du vill inkludera i fragmentet, inklusive anpassningsfält och dynamiskt innehåll.

   >[!CAUTION]
   >
   >Du kan bara markera intilliggande avsnitt. Du kan inte markera en tom struktur eller ett annat fragment.

   ![](assets/fragment-save-as-screen.png)

1. Klicka på **[!UICONTROL Create]**. Fyll i fragmentnamnet och spara det.

   ![](assets/fragment-save-confirm.png)

   Det här innehållet är nu ett fristående fragment som läggs till i [fragmentlista](#manage-fragments)och kan öppnas via den dedikerade menyn. Du kan nu använda det här fragmentet när du skapar [e-post](../email/get-started-email-designer.md) eller [innehållsmall](use-email-templates.md) inom Campaign. [Lär dig mer](../email/use-visual-fragments.md)

>[!NOTE]
>
>Ändringar i det nya fragmentet sprids inte till e-postmeddelandet eller mallen som det kommer från. På samma sätt ändras inte det nya fragmentet när det ursprungliga innehållet redigeras i e-postmeddelandet eller mallen.

## Hantera dina fragment {#manage-fragments}

Du kan redigera, uppdatera, duplicera eller ta bort ett fragment från fragmentlistan.

### Redigera och uppdatera ett fragment {#edit-fragments}

Om du vill redigera ett fragment följer du stegen nedan.

1. Klicka på namnet på det fragment som du vill redigera från **[!UICONTROL Fragments]** lista.
1. Klicka på **Redigera innehåll** för att öppna innehållet i det här fragmentet.

   ![](assets/fragment-edit-content.png)

1. Gör de ändringar du behöver och spara ändringarna.

>[!CAUTION]
>
>Alla ändringar i ett fragment sprids till e-postleveranser eller mallar som använder det.


### Ta bort ett fragment {#delete-fragments}

Så här tar du bort ett fragment:

1. Gå till fragmentlistan och klicka på **[!UICONTROL More actions]** -knappen bredvid det fragment som ska tas bort.
1. Klicka **Ta bort** och bekräfta.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>När du tar bort ett innehållsfragment uppdateras e-postleveranser och mallar som använder det och fragmentet tas bort från meddelandeinnehållet. Du kan bryta arv om det behövs. [Läs mer](use-visual-fragments.md#break-inheritance)
>

### Duplicera ett fragment {#duplicate-fragments}

Du kan enkelt duplicera ett fragment och skapa ett nytt. Så här duplicerar du ett befintligt fragment:

1. Gå till fragmentlistan och klicka på **[!UICONTROL More actions]** -knappen bredvid det fragment som ska tas bort.
1. Klicka **Duplicera** och bekräfta.
1. Ange det nya fragmentets etikett och spara ändringarna.

   Fragmentet läggs till i fragmentlistan. Du kan redigera den och konfigurera den efter behov.
