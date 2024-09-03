---
audience: end-user
title: Skapa innehållsfragment
description: Lär dig skapa innehållsfragment
source-git-commit: d27bbc8647d17dc442656465aa6d5a7e4fe7f060
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 0%

---


# Skapa innehållsfragment {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Definiera egna innehållsfragment"
>abstract="Definiera fragmentegenskaperna och den typ av fragment som du vill skapa. Du kan sedan använda e-postdesignern eller uttrycksredigeraren för att konfigurera innehållet i fragmentet."

<!-- pas vu dans l'UI-->

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragmentegenskaper"
>abstract="Ange fragmentets etikett. Om det behövs kan du definiera ytterligare alternativ, till exempel fragmentets interna namn, dess mapp och en beskrivning."

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Typ av innehållsfragment"
>abstract="Välj den typ av fragment som du vill skapa. **Visuella fragment** är fördefinierade visuella block som du kan återanvända i flera e-postleveranser eller i innehållsmallar. **Uttrycksfragment** är fördefinierade uttryck som är tillgängliga från en dedikerad post i uttrycksredigeraren."

Det finns två sätt att skapa innehållsfragment:

* Skapa ett fragment från grunden med den dedikerade menyn **[!UICONTROL Fragments]**. [Lär dig hur](#create-from-scratch)
* När du utformar innehåll sparar du en del av innehållet som fragment. [Lär dig hur](#save-as-fragment)

  >[!NOTE]
  >
  >Den här funktionen är endast tillgänglig för visuella fragment. Uttrycksfragment skapas exklusivt från menyn **Fragment** .

När du har sparat ditt innehållsfragment är det tillgängligt för användning i alla mallar för leverans och innehåll.

## Skapa ett innehållsfragment från grunden {#create-from-scratch}

Om du vill skapa ett innehållsfragment från grunden följer du stegen nedan.

1. [Gå till fragmentlistan](#access-manage-fragments) via menyn **[!UICONTROL Content Management]** > **[!UICONTROL Fragments]** till vänster och välj **[!UICONTROL Create fragment]**.

   ![](assets/fragments-list.png)

1. Ange fragmentets etikett. Om det behövs kan du definiera ytterligare alternativ, till exempel fragmentets interna namn, dess mapp och en beskrivning.

1. Välj den typ av fragment som du vill skapa: **Visual fragment** eller **Expression fragment**. [Lär dig skillnaderna mellan visuella fragment och uttrycksfragment](fragments.md)

   ![](assets/fragment-create.png)

   >[!AVAILABILITY]
   >
   >Visual fragments in Limited Availability (LA). De är begränsade till kunder som migrerar **från Adobe Campaign Standard till Adobe Campaign v8** och kan inte distribueras i någon annan miljö.

1. Klicka på knappen **Skapa**.

   * För **visuella fragment** visas [e-post-Designer](../email/get-started-email-designer.md). Redigera ditt innehåll efter behov, på samma sätt som du gör för e-postmeddelanden i en kampanj och klicka sedan på knappen **Spara och stäng** . Du kan lägga till bilder, länkar, anpassningsfält och dynamiskt innehåll.

     ![](assets/fragment-designer.png)

   * För **uttrycksfragment** öppnas uttrycksredigeraren. Utnyttja sina personaliserings- och redigeringsfunktioner för att skapa ditt innehåll och klicka sedan på **Bekräfta**. [Lär dig arbeta med uttrycksredigeraren](../personalization/personalize.md)

     ![](assets/fragment-expression.png)

1. När innehållet är klart klickar du på **Spara**.

Innehållsfragmentet kan nu användas när du skapar en leverans eller [innehållsmall](../email/use-email-templates.md) i Campaign. Lär dig hur du använder visuella fragment och uttrycksfragment i följande avsnitt:
* [Lägg till visuella fragment i e-postmeddelanden](use-visual-fragments.md)
* [Lägg till uttrycksfragment i uttrycksredigeraren](use-expression-fragments.md)

## Spara ett innehåll som ett visuellt fragment {#save-as-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Spara som fragment"
>abstract="Om du vill spara ett innehåll som ett visuellt fragment markerar du de element du vill inkludera i fragmentet, inklusive anpassningsfält och dynamiskt innehåll. Du kan bara markera intilliggande avsnitt. Du kan inte markera en tom struktur eller ett annat innehållsfragment. Det här innehållet blir då ett fristående fragment som läggs till i fragmentlistan och kan nås från den dedikerade menyn. Du kan använda det här avsnittet när du skapar e-post- eller innehållsmallar i Campaign."

<!--pas vu dans l'UI-->

Allt e-postinnehåll kan sparas som ett visuellt fragment för framtida återanvändning. När du utformar en [innehållsmall](../email/use-email-templates.md) eller en [e-postleverans](../email/get-started-email-designer.md) kan du spara en del av innehållet som ett visuellt fragment. Gör så här:

1. Klicka på knappen **Mer** överst till höger på skärmen i [Skicka e-post till Designer](../email/get-started-email-designer.md).

1. Välj **[!UICONTROL Save as fragment]** i listrutan.

   ![](assets/fragment-save-as.png)

1. Skärmen **[!UICONTROL Save as fragment]** visas. Här väljer du de element som du vill inkludera i fragmentet, inklusive anpassningsfält och dynamiskt innehåll.

   >[!CAUTION]
   >
   >Du kan bara markera intilliggande avsnitt. Du kan inte markera en tom struktur eller ett annat innehållsfragment.

   ![](assets/fragment-save-as-screen.png)

1. Klicka på **[!UICONTROL Create]**. Fyll i fragmentnamnet och spara det.

   ![](assets/fragment-save-confirm.png)

   Det här innehållet är nu ett fristående fragment som läggs till i [fragmentlistan](#manage-fragments) och kan nås från den dedikerade menyn. Du kan nu använda det här fragmentet när du skapar en [e-postadress](../email/get-started-email-designer.md) eller [innehållsmall](../email/use-email-templates.md) i Campaign. [Lär dig hur](../content/use-visual-fragments.md)

>[!NOTE]
>
>Ändringar i det nya fragmentet sprids inte till e-postmeddelandet eller mallen som det kommer från. På samma sätt ändras inte det nya fragmentet när det ursprungliga innehållet redigeras i e-postmeddelandet eller mallen.—>

## Hantera era innehållsfragment {#manage-fragments}

Du kan redigera, uppdatera, duplicera eller ta bort ett innehållsfragment från fragmentlistan.

### Redigera och uppdatera ett innehållsfragment {#edit-fragments}

Om du vill redigera ett innehållsfragment följer du stegen nedan.

1. Klicka på namnet på det fragment som ska redigeras i listan **[!UICONTROL Fragments]**.
1. Klicka på knappen **Redigera innehåll** för att öppna innehållet i det här fragmentet.

   ![](assets/fragment-edit-content.png)

1. Gör de ändringar du behöver och spara ändringarna.

>[!CAUTION]
>
>Alla ändringar i ett fragment sprids till leveranser eller mallar som använder det.

### Ta bort ett innehållsfragment {#delete-fragments}

Så här tar du bort ett innehållsfragment:

1. Bläddra till fragmentlistan och klicka på knappen **[!UICONTROL More actions]** bredvid fragmentet som ska tas bort.
1. Klicka på **Ta bort** och bekräfta.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>När du tar bort ett fragment uppdateras leveranser och mallar som använder det: fragmentet tas bort från innehållet, men refereras ändå. Om du vill behålla fragmentinnehållet i de leveranserna och mallarna måste du bryta arvet innan du tar bort fragmentet, [enligt informationen i det här avsnittet](use-visual-fragments.md#break-inheritance).

### Arkivera ett innehållsfragment {#archive}

Du kan rensa fragmentlistan från de fragment som inte längre är relevanta för ert varumärke. Om du vill göra det klickar du på knappen **[!UICONTROL More actions]** bredvid det önskade fragmentet och väljer **[!UICONTROL Archive]**. Fragmentet tas bort från fragmentlistan, vilket förhindrar användare att använda det i framtida e-postmeddelanden eller mallar.

Använd filtreringsrutan för att visa arkiverade fragment. Om du vill avarkivera ett fragment klickar du på knappen **[!UICONTROL More actions]** och väljer **[!UICONTROL Unarchive]**.

![](assets/fragment-unarchive.png)

>[!NOTE]
>
>Om du arkiverar ett fragment som används i ett innehåll påverkas inte det innehållet.

### Duplicera ett innehållsfragment {#duplicate-fragments}

Du kan enkelt duplicera ett innehållsfragment och skapa ett nytt. Så här duplicerar du ett befintligt fragment:

1. Bläddra till fragmentlistan och klicka på knappen **[!UICONTROL More actions]** bredvid fragmentet som ska dupliceras.
1. Klicka på **Duplicera** och bekräfta.
1. Ange det nya fragmentets etikett och spara ändringarna.

   Fragmentet läggs till i listan med innehållsfragment. Du kan redigera den och konfigurera den efter behov.
