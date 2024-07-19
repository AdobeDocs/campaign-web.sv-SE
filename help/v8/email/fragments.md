---
audience: end-user
title: Skapa innehållsfragment
description: Lär dig skapa med innehållsfragment
hide: true
hidefromtoc: true
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# Skapa innehållsfragment {#fragments}


>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Definiera egna fragment"
>abstract="Ett fragment är en återanvändbar komponent som kan refereras i en eller flera e-postmeddelanden mellan kampanjer. Den här funktionen används för att skapa flera anpassade innehållsblock som kan användas av marknadsföringsanvändare för att snabbt sammanställa e-postinnehåll i en förbättrad designprocess."

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
* Använd dem så många gånger som behövs i ditt innehåll via e-post-Designer. Se [Lägg till visuella fragment i e-postmeddelanden](../email/use-visual-fragments.md).

## Skapa ett Visual fragment {#create-fragments}

Det finns två sätt att skapa fragment:

* Skapa ett fragment från grunden med den dedikerade menyn **[!UICONTROL Fragments]**. [Lär dig hur](#create-from-scratch)

* När du utformar innehåll sparar du en del av innehållet som fragment. [Lär dig hur](#save-as-fragment)

När fragmentet har sparats kan det användas i ett e-postmeddelande eller i en e-postmall. Oavsett om du har skapat från grunden eller från ett befintligt innehåll kan du nu använda det här avsnittet när du skapar innehåll i Campaign. Se [Lägg till visuella fragment](../email/use-visual-fragments.md).

### Skapa ett fragment från grunden {#create-from-scratch}

Följ stegen nedan om du vill skapa ett fragment från grunden.

1. [Öppna fragmentlistan](#access-manage-fragments) via den vänstra menyn **[!UICONTROL Content Management]** > **[!UICONTROL Fragments]**.

   ![](assets/fragments-list.png)

1. Välj **[!UICONTROL Create fragment]**.

1. Ange fragmentets etikett.

   ![](assets/fragment-create.png)

1. Om det behövs kan du definiera ytterligare alternativ, till exempel fragmentets interna namn, dess mapp och en beskrivning.

   >[!NOTE]
   >
   >För tillfället kan du bara skapa visuella fragment.

1. Klicka på knappen **Skapa** för att konfigurera innehållet i fragmentet.

1. [E-postmeddelandet för Designer](../email/get-started-email-designer.md) visas. Redigera innehåll efter behov, på samma sätt som du gör för alla e-postmeddelanden i en kampanj. Du kan lägga till bilder, länkar, anpassningsfält och dynamiskt innehåll.

   ![](assets/fragment-designer.png)

1. När fragmentet är klart klickar du på **[!UICONTROL Save & close]**. Den har lagts till i [fragmentlistan](#access-manage-fragments).

Det här fragmentet kan nu användas när du skapar en [e-post](../email/get-started-email-designer.md) eller [innehållsmall](use-email-templates.md) i Campaign. [Lär dig hur](../email/use-visual-fragments.md)


### Spara ett innehåll som fragment {#save-as-fragment}

Allt e-postinnehåll kan sparas som fragment för framtida återanvändning. När du utformar en [innehållsmall](use-email-templates.md) eller en [e-postleverans](../email/get-started-email-designer.md) kan du spara en del av innehållet som ett visuellt fragment. Gör så här:

1. Klicka på knappen **Mer** överst till höger på skärmen i [Skicka e-post till Designer](../email/get-started-email-designer.md).

1. Välj **[!UICONTROL Save as fragment]** i listrutan.

   ![](assets/fragment-save-as.png)

1. Skärmen **[!UICONTROL Save as fragment]** visas. Här väljer du de element som du vill inkludera i fragmentet, inklusive anpassningsfält och dynamiskt innehåll.

   >[!CAUTION]
   >
   >Du kan bara markera intilliggande avsnitt. Du kan inte markera en tom struktur eller ett annat fragment.

   ![](assets/fragment-save-as-screen.png)

1. Klicka på **[!UICONTROL Create]**. Fyll i fragmentnamnet och spara det.

   ![](assets/fragment-save-confirm.png)

   Det här innehållet är nu ett fristående fragment som läggs till i [fragmentlistan](#manage-fragments) och kan nås från den dedikerade menyn. Du kan nu använda det här fragmentet när du skapar en [e-postadress](../email/get-started-email-designer.md) eller [innehållsmall](use-email-templates.md) i Campaign. [Lär dig hur](../email/use-visual-fragments.md)

>[!NOTE]
>
>Ändringar i det nya fragmentet sprids inte till e-postmeddelandet eller mallen som det kommer från. På samma sätt ändras inte det nya fragmentet när det ursprungliga innehållet redigeras i e-postmeddelandet eller mallen.

## Hantera dina fragment {#manage-fragments}

Du kan redigera, uppdatera, duplicera eller ta bort ett fragment från fragmentlistan.

### Redigera och uppdatera ett fragment {#edit-fragments}

Om du vill redigera ett fragment följer du stegen nedan.

1. Klicka på namnet på det fragment som ska redigeras i listan **[!UICONTROL Fragments]**.
1. Klicka på knappen **Redigera innehåll** för att öppna innehållet i det här fragmentet.

   ![](assets/fragment-edit-content.png)

1. Gör de ändringar du behöver och spara ändringarna.

>[!CAUTION]
>
>Alla ändringar i ett fragment sprids till e-postleveranser eller mallar som använder det.


### Ta bort ett fragment {#delete-fragments}

Så här tar du bort ett fragment:

1. Bläddra till fragmentlistan och klicka på knappen **[!UICONTROL More actions]** bredvid fragmentet som ska tas bort.
1. Klicka på **Ta bort** och bekräfta.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>När du tar bort ett innehållsfragment uppdateras e-postleveranser och mallar som använder det: fragmentet tas bort från e-postinnehållet, men refereras ändå. Om du vill behålla fragmentinnehållet i de leveranserna och mallarna måste du bryta arvet innan du tar bort fragmentet, [enligt informationen i det här avsnittet](use-visual-fragments.md#break-inheritance).
>

### Duplicera ett fragment {#duplicate-fragments}

Du kan enkelt duplicera ett fragment och skapa ett nytt. Så här duplicerar du ett befintligt fragment:

1. Bläddra till fragmentlistan och klicka på knappen **[!UICONTROL More actions]** bredvid fragmentet som ska tas bort.
1. Klicka på **Duplicera** och bekräfta.
1. Ange det nya fragmentets etikett och spara ändringarna.

   Fragmentet läggs till i fragmentlistan. Du kan redigera den och konfigurera den efter behov.
