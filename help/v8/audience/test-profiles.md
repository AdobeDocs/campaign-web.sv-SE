---
title: Skapa testprofiler i Campaign
description: Lär dig skapa och hantera testprofiler i Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 2%

---

# Skapa och hantera testprofiler {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Skapa testprofiler"
>abstract="Testprofiler skapas som dirigerade adresser. De är ytterligare mottagare i databasen som används för att rikta fiktiva profiler som inte matchar de definierade målvillkoren."

Testprofiler skapas som dirigerade adresser. De är ytterligare mottagare i databasen som används för att rikta fiktiva profiler som inte matchar de definierade målvillkoren. De gör att du kan förhandsgranska och testa personaliseringen och återgivningen innan du skickar leveransen, genom att skicka dem som korrektur.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

Stegen för att skicka korrektur till dirigerade adresser beskrivs i [det här avsnittet](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>Testprofiler exkluderas automatiskt från rapporter om följande leveransstatistik: **[!UICONTROL Clicks]**, **[!UICONTROL Opens]**, **[!UICONTROL Unsubscriptions]**. [Läs mer om rapporter]

## Få åtkomst till och hantera testprofiler {#access-test-profiles}

Om du vill öppna testprofillistan väljer du **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** från den vänstra menyn och klicka på **[!UICONTROL Test profiles]** -fliken.

![](assets/test-profile-list.png){zoomable=&quot;yes&quot;}

* Du kan filtrera på en viss [mapp](../get-started/permissions.md#folders) använda listrutan eller lägga till regler med [frågemodellerare](../query/query-modeler-overview.md).

  ![](assets/test-profile-list-filters.png){zoomable=&quot;yes&quot;}

* Du kan duplicera valfri testprofil och uppdatera den efter behov. Stegen för att redigera en testprofil är desamma som när [skapa en testprofil](#create-test-profile).

* Om du vill ta bort en testprofil väljer du motsvarande alternativ i dialogrutan **[!UICONTROL More actions]** -menyn.

  ![](assets/test-profile-list-delete.png){zoomable=&quot;yes&quot;}

* Om du vill redigera en testprofil klickar du på önskat objekt i listan. Stegen för att redigera en testprofil är desamma som när [skapa en testprofil](#create-test-profile).

Du kan även komma åt testprofiler via **[!UICONTROL Explorer]** visa, från **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** nod.

Därifrån kan du bläddra, skapa och hantera mappar eller undermappar samt kontrollera tillhörande behörigheter. [Lär dig hur du skapar mappar](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png){zoomable=&quot;yes&quot;}

Från **[!UICONTROL Explorer]** kan du även filtrera, ta bort, redigera och [skapa](#create-test-profile) testprofiler.

## Skapa en testprofil {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Testa profiler Ytterligare data"
>abstract="Ange de personaliseringsdata som används för leveranser som skapas i arbetsflödena för datahantering och som du vill tilldela ett specifikt värde till."

Följ stegen nedan för att skapa en testprofil.

1. Bläddra till **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** och väljer **[!UICONTROL Test profiles]** -fliken.

1. Klicka på knappen **[!UICONTROL Create test profile]**.

   ![](assets/test-profile-create.png){zoomable=&quot;yes&quot;}

1. Fyll i informationen om testprofilen efter behov. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >The **[!UICONTROL Label]** fältet fylls automatiskt i med det förnamn och efternamn som du har definierat.

1. Som standard lagras testprofiler i **[!UICONTROL Seed addresses]** mapp. Du kan ändra den genom att bläddra till önskad plats. [Lär dig hur du arbetar med mappar](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. I **[!UICONTROL Contact information]** anger du e-postadressen och andra relevanta data. E-postadressen visas inom hakparenteser efter testprofilens etikett.

   ![](assets/test-profile-address.png){zoomable=&quot;yes&quot;}

1. Om du väljer **[!UICONTROL No longer contact (by any channel)]** är testprofilen till blockeringslista. Den här mottagaren är inte längre riktad mot någon kanal (e-post, SMS etc.).

1. I **[!UICONTROL Additional data]** Ange de personaliseringsdata som används för leveranser som skapas i arbetsflödena för datahantering och som du vill tilldela ett specifikt värde till. [Läs mer om arbetsflöden](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png){zoomable=&quot;yes&quot;}

   Se till att ytterligare måldata har definierats med ett alias som börjar med @ i **[!UICONTROL Enrichment]** arbetsflödesaktivitet. Annars kan du inte använda den korrekt med dina dirigerade adresser i leveransaktiviteten. [Läs mer om Enrichment-aktiviteten](../workflows/activities/enrichment.md)

1. Klicka på knappen **[!UICONTROL Save]**.

Testprofilen som du nyss skapade kan nu användas för att skicka ett korrektur. [Läs mer](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->
