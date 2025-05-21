---
audience: end-user
title: Skapa innehållsfragment
description: Lär dig skapa innehållsfragment
exl-id: 8f37e9e6-3085-4a68-9746-8ca34cfa4242
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1002'
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
* När du utformar innehåll sparar du en del av innehållet som ett fragment. [Lär dig hur](#save-as-fragment)

  >[!NOTE]
  >
  >Den här funktionen är endast tillgänglig för visuella fragment. Uttrycksfragment skapas exklusivt från menyn **Fragment** .

När innehållsfragmentet har sparats är det tillgängligt för användning i alla leverans- och innehållsmallar.

## Skapa ett innehållsfragment från grunden {#create-from-scratch}

Om du vill skapa ett innehållsfragment från grunden följer du stegen nedan.

1. [Gå till fragmentlistan](#access-manage-fragments) via menyn **[!UICONTROL Content Management]** > **[!UICONTROL Fragments]** till vänster och välj **[!UICONTROL Create fragment]**.

   ![Skärmen Fragmentlista visar alternativet Skapa fragment](assets/fragments-list.png)

1. Ange fragmentets etikett. Definiera ytterligare alternativ om det behövs, till exempel fragmentets interna namn, dess mapp och en beskrivning.

1. Välj den typ av fragment som ska skapas: **Visual fragment** eller **Expression fragment**. [Lär dig skillnaderna mellan visuella fragment och uttrycksfragment](fragments.md)

   ![Skärmen Fragmentskapande visar typval](assets/fragment-create.png)

   >[!AVAILABILITY]
   >
   >Visual fragments require an update to Campaign v8.6.4. Läs mer i [Versionsinformation för Campaign v8-klientkonsolen](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/releases/release-notes).

1. Klicka på knappen **Skapa**.

   * För **visuella fragment** visas [e-post-Designer](../email/get-started-email-designer.md). Redigera innehållet efter behov, på samma sätt som för alla e-postmeddelanden i en kampanj och klicka sedan på knappen **Spara och stäng** . Lägg till bilder, länkar, anpassningsfält och dynamiskt innehåll.

     ![Skicka e-post till Designer-skärmen för visuella fragment](assets/fragment-designer.png)

   * För **uttrycksfragment** öppnas uttrycksredigeraren. Använd dess anpassnings- och redigeringsfunktioner för att skapa innehållet och klicka sedan på **Bekräfta**. [Lär dig arbeta med uttrycksredigeraren](../personalization/personalize.md)

     ![Skärm för uttrycksredigerare för uttrycksfragment](assets/fragment-expression.png)

1. När innehållet är klart klickar du på **Spara**.

Innehållsfragmentet kan nu användas när du skapar en leverans eller [innehållsmall](../email/use-email-templates.md) i Campaign. Lär dig hur du använder visuella fragment och uttrycksfragment i följande avsnitt:
* [Lägg till visuella fragment i e-postmeddelanden](use-visual-fragments.md)
* [Lägga till uttrycksfragment i uttrycksredigeraren](use-expression-fragments.md)

## Spara innehåll som visuellt fragment {#save-as-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Spara som fragment"
>abstract="Om du vill spara innehåll som ett visuellt fragment markerar du de element som ska inkluderas i fragmentet, inklusive anpassningsfält och dynamiskt innehåll. Det går endast att markera närliggande avsnitt. Tomma strukturer eller andra innehållsfragment kan inte markeras. Innehållet blir sedan ett fristående fragment som läggs till i fragmentlistan och kan nås från den dedikerade menyn. Det här fragmentet kan användas när du skapar e-post- eller innehållsmallar i Campaign."

<!--pas vu dans l'UI-->

Allt e-postinnehåll kan sparas som ett visuellt fragment för framtida återanvändning. När du utformar en [innehållsmall](../email/use-email-templates.md) eller en [e-postleverans](../email/get-started-email-designer.md) sparar du en del av innehållet som ett visuellt fragment. Gör så här:

1. Klicka på knappen **Mer** längst upp till höger på skärmen i [Skicka e-post till Designer](../email/get-started-email-designer.md).

1. Välj **[!UICONTROL Save as fragment]** i listrutan.

   ![Alternativet Spara som fragment i e-post-Designer](assets/fragment-save-as.png)

1. Skärmen **[!UICONTROL Save as fragment]** visas. Markera elementen som ska inkluderas i fragmentet, inklusive anpassningsfält och dynamiskt innehåll.

   >[!CAUTION]
   >
   >Det går endast att markera närliggande avsnitt. Tomma strukturer eller andra innehållsfragment kan inte markeras.

   ![Spara som fragmentskärm med elementmarkering](assets/fragment-save-as-screen.png)

1. Klicka på **[!UICONTROL Create]**. Fyll i fragmentnamnet och spara det.

   ![Spara bekräftelseskärmen för visuella fragment](assets/fragment-save-confirm.png)

   Det här innehållet är nu ett fristående fragment som läggs till i [fragmentlistan](#manage-fragments) och kan nås från den dedikerade menyn. Använd det här fragmentet när du skapar en [e-postadress](../email/get-started-email-designer.md) eller [innehållsmall](../email/use-email-templates.md) i Campaign. [Lär dig hur](../content/use-visual-fragments.md)

>[!NOTE]
>
>Ändringar i det nya fragmentet sprids inte till e-postmeddelandet eller mallen som det kommer från. På samma sätt ändras inte det nya fragmentet när det ursprungliga innehållet redigeras i e-postmeddelandet eller mallen.

## Hantera era innehållsfragment {#manage-fragments}

Du kan redigera, uppdatera, duplicera eller ta bort ett innehållsfragment från fragmentlistan.

### Redigera och uppdatera ett innehållsfragment {#edit-fragments}

Om du vill redigera ett innehållsfragment följer du stegen nedan.

1. Klicka på namnet på det fragment som ska redigeras i listan **[!UICONTROL Fragments]**.
1. Klicka på knappen **Redigera innehåll** för att öppna fragmentets innehåll.

   ![Redigera innehållsknapp för fragment](assets/fragment-edit-content.png)

1. Gör de ändringar som behövs och spara ändringarna.

>[!CAUTION]
>
>Ändringar i ett fragment sprids till leveranser eller mallar som använder det.

### Ta bort ett innehållsfragment {#delete-fragments}

Så här tar du bort ett innehållsfragment:

1. Bläddra till fragmentlistan och klicka på knappen **[!UICONTROL More actions]** bredvid fragmentet som ska tas bort.
1. Klicka på **Ta bort** och bekräfta.

   ![Ta bort alternativ i fragmentlistan](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>När du tar bort ett fragment uppdateras leveranser och mallar som använder det. Fragmentet tas bort från innehållet men refereras fortfarande. Om du vill behålla fragmentinnehållet i dessa leveranser och mallar bryter du arvet innan du tar bort fragmentet, [enligt informationen i det här avsnittet](use-visual-fragments.md#break-inheritance).

### Arkivera ett innehållsfragment {#archive}

Ni kan rensa fragmentlistan genom att arkivera fragment som inte längre är relevanta för ert varumärke. Om du vill göra det klickar du på knappen **[!UICONTROL More actions]** bredvid det önskade fragmentet och väljer **[!UICONTROL Archive]**. Fragmentet tas bort från fragmentlistan, vilket förhindrar användare att använda det i framtida e-postmeddelanden eller mallar.

Använd filtreringsrutan för att visa arkiverade fragment. Om du vill avarkivera ett fragment klickar du på knappen **[!UICONTROL More actions]** och väljer **[!UICONTROL Unarchive]**.

![Oarkiveringsalternativ för fragment](assets/fragment-unarchive.png)

>[!NOTE]
>
>Om du arkiverar ett fragment som används i ett innehåll påverkas inte det innehållet.

### Duplicera ett innehållsfragment {#duplicate-fragments}

Du kan enkelt duplicera ett innehållsfragment och skapa ett nytt. Så här duplicerar du ett befintligt fragment:

1. Bläddra till fragmentlistan och klicka på knappen **[!UICONTROL More actions]** bredvid fragmentet som ska dupliceras.
1. Klicka på **Duplicera** och bekräfta.
1. Ange etiketten för det nya fragmentet och spara ändringarna.

   Fragmentet läggs till i listan med innehållsfragment. Redigera och konfigurera den efter behov.