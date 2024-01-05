---
title: Övervaka och hantera profiler
description: Lär dig övervaka och hantera profiler på Campaign Web.
badge: label="Begränsad tillgänglighet"
source-git-commit: e72069956490dc0febc2835568deb99cf41ead1c
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# Övervaka och redigera profiler {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360-vy av dina profiler"
>abstract="Skapa nya profiler och övervaka dem med hjälp av kraftfulla rapporter och verktyg. Få åtkomst till attribut, interaktioner och loggar för dina profiler. Använd filtreringsalternativen för att bläddra i profillistan, redigera och uppdatera deras profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Se versionsinformation"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profiler"
>abstract="En profil är en individ som ska ta emot meddelanden från Adobe Campaign. I den här listan kan du visa profilens information utifrån dina behörigheter. Använd filteralternativen för att bläddra i den här listan. Du kan redigera och uppdatera en liten uppsättning profilattribut."

## Kom igång med profiler {#gs}

En profil på Adobe Campaign Web är en individ som lagras i databasen och som en nyckelkomponent för att skapa målgrupper för leveranser och lägga till personaliseringsdata i innehållet.

Andra typer av profiler lagras i databasen, till exempel **[!UICONTROL Test profiles]**, som är utformade för att testa era leveranser innan de skickas till slutanvändarna. [Lär dig hur du arbetar med testprofiler](test-profiles.md)

Profiler kan bara skapas från Adobe Campaign klientkonsol - [lära dig hur](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/create-profiles.html){target="_blank"}. De är dock tillgängliga och redigerbara på Adobe Campaign Web från **[!UICONTROL Customer management]** > **Profiler** inträde i det vänstra navigeringsfältet.

>[!NOTE]
>
>Beroende på dina behörigheter kanske du inte har tillgång till den fullständiga listan över profiler som lagras i databasen. Läs mer om behörigheter i [det här avsnittet](../get-started/permissions.md).

* Du kan filtrera **[!UICONTROL Profiles]** med sökfältet eller de filter som finns i **Visa filter** -knappen. Du kan begränsa resultatet till en viss [mapp](../get-started/permissions.md#folders) använda listrutan eller lägga till regler med [frågemodellerare](../query/query-modeler-overview.md).

  ![](assets/profiles-list.png)

* Om du vill ta bort en profil väljer du motsvarande alternativ i dialogrutan **[!UICONTROL More actions]** -menyn.

* Om du vill redigera en profil klickar du på önskat objekt i listan. [Läs mer](#access)

Du kan även komma åt profiler via **[!UICONTROL Explorer]** visa, från **[!UICONTROL Profiles & Targets]** > **[!UICONTROL Recipients]** nod.

Därifrån kan du bläddra, skapa och hantera mappar eller undermappar samt kontrollera tillhörande behörigheter. [Lär dig hur du skapar mappar](../get-started/permissions.md#folders)

![](assets/profiles-explorer-folder.png)

Från **[!UICONTROL Explorer]** kan du även filtrera, ta bort och [redigera](#access) profiler.

## Få åtkomst till och redigera profilattribut {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Grundläggande information"
>abstract="I det här avsnittet finns information om de grundläggande detaljerna i profilen. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Kontaktinformation"
>abstract="I det här avsnittet finns information om profilens kontaktinformation. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Adress"
>abstract="I det här avsnittet finns information om profilens postadress och adresskvalitet. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Kontoinformation"
>abstract="I det här avsnittet finns information om profilens kontoinformation. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Mottagarna kontaktar inte längre"
>abstract="I det här avsnittet finns information om kontaktinställningarna för profilen. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Anpassade fält"
>abstract="Anpassade fält är specifika attribut som är anpassade efter dina behov och som har konfigurerats för din instans. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Övriga"
>abstract="I det här avsnittet finns ytterligare inbyggda attribut. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Mottagarens prenumerationslista"
>abstract="På den här fliken visas alla tjänster som profilen prenumererar på."

Följ stegen nedan för att få tillgång till information om en profil och redigera den.

1. Bläddra till **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]**.

1. Klicka på önskat objekt på **[!UICONTROL Profiles]** lista. Detaljerad information om profilen visas.

   ![](assets/profile-details.png)

1. The **[!UICONTROL Details]** kan du bläddra igenom profilens inbyggda och anpassade attribut. Om du vill redigera ett attribut gör du ändringarna i det önskade fältet och klickar på knappen **[!UICONTROL Save]** -knappen.

   1. Som standard lagras profiler i **[!UICONTROL Recipients]** mapp. Du kan ändra den genom att bläddra till önskad plats. [Lär dig hur du arbetar med mappar](../get-started/permissions.md#folders)

      ![](assets/profile-folder.png)

   1. I **[!UICONTROL Contact information]** kan du uppdatera e-postadressen och andra relevanta data. E-postadressen visas inom hakparenteser efter profiletiketten.

      ![](assets/profile-address.png)

   1. Kontrollera **[!UICONTROL No longer contact]** och uppdatera dem vid behov. När något av dessa alternativ är markerat visas profilen till blockeringslista. Den här informationen läggs till i kontaktinformationen om mottagaren till exempel klickade på länken för att avbryta prenumerationen i ett nyhetsbrev. Den här mottagaren är inte längre riktad mot de valda kanalerna. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

      ![](assets/profile-no-longer-contact.png)

   1. Om det finns **[!UICONTROL Custom fields]** kan du uppdatera deras värden efter behov. Anpassade fält är ytterligare attribut som läggs till i **[!UICONTROL Profiles]** via Adobe Campaign-konsolen. [Läs mer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

      ![](assets/profile-custom-fields.png)

1. Klicka på **[!UICONTROL Subscriptions]** för att få tillgång till information om de tjänster som profilen prenumererar på. [Lär dig arbeta med prenumerationstjänster](manage-services.md)

1. Klicka på **[!UICONTROL Logs]** i skärmens övre högra hörn för att visa historiken för profilens interaktioner genom att skicka, exkludera och spåra loggar - samt erbjudanden som presenteras för profilen. [Läs mer om leveransloggar](../monitor/delivery-logs.md)

   ![](assets/profile-logs.png)
