---
title: Skapa en profil
description: Lär dig hur du skapar en profil på Campaign Web.
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 1%

---

# Skapa en profil {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Grundläggande information"
>abstract="I det här avsnittet finns information om de grundläggande detaljerna i profilen. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Kontaktinformation"
>abstract="I det här avsnittet finns information om profilens kontaktinformation. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Adress"
>abstract="I det här avsnittet finns information om profilens postadress och adresskvalitet. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Kontoinformation"
>abstract="I det här avsnittet finns information om profilens kontoinformation. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Kontakten är inte längre"
>abstract="I det här avsnittet finns information om kontaktinställningarna för profilen. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Anpassade fält"
>abstract="Anpassade fält är specifika attribut som är anpassade efter dina behov och som har konfigurerats för din instans. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Övriga"
>abstract="I det här avsnittet finns ytterligare inbyggda attribut. Om du vill ändra någon information gör du ändringarna direkt i respektive fält och klickar på knappen **Spara** i skärmens övre högra hörn."

Så här skapar du en profil:

1. Navigera till **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** och klicka på knappen **[!UICONTROL Create profile]** i skärmens övre högra hörn.

1. Listan med tillgängliga attribut för profilvisningen, ordnade i olika avsnitt som anges i tabellen nedan.

   ![](assets/create-profile.png){zoomable="yes"}

   | Avsnittet Attribut | Beskrivning |
   |  ---  |  ---  |
   | **Grundläggande information** | Grundläggande information om profilen, t.ex. födelsedatum eller namn.<br/>Som standard lagras profiler i mappen **[!UICONTROL Recipients]**. Du kan ändra den genom att bläddra till önskad plats. [Lär dig arbeta med mappar](../get-started/permissions.md#folders) |
   | **Kontaktinformation** | Profilens kontaktinformation, till exempel e-postadress eller telefonnummer. |
   | **Adress** | Profilens postadress. I det här avsnittet finns även en utvärdering av adresskvaliteten. En profils adress anses vara giltig om fälten Efternamn, Ort och Postnummer har angetts. |
   | **Kontoinformation** | Information om profilens konto, t.ex. dess status eller kontonummer. |
   | **Kontakten tas inte längre** | Profilens kontaktinställningar. När något av dessa alternativ är markerat visas profilen till blockeringslista.<br/>Om mottagaren till exempel klickade på en länk för att avbryta prenumerationen i ett nyhetsbrev läggs den här informationen till i kontaktinformationen. Den här mottagaren är inte längre riktad mot de valda kanalerna. Läs mer om karantänhantering i [Adobe Campaign v8-dokumentationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"} |
   | **Anpassade fält** | Om anpassade fält har konfigurerats visas de i det här avsnittet. Anpassade fält är ytterligare attribut som har lagts till i schemat **[!UICONTROL Profiles]** via Adobe Campaign-konsolen. Läs mer i [Adobe Campaign v8-dokumentationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"} |
   | **Övriga** | Ytterligare inbyggda attribut. |

1. När du har konfigurerat profilen klickar du på **[!UICONTROL Create]** för att spara den i databasen.

   När du är klar kan du redigera profilen när som helst genom att öppna den från listan över profiler. [Lär dig utforska profilinformation](profile-view.md)
