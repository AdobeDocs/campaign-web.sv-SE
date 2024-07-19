---
title: Anpassade fält
description: Lär dig konfigurera anpassade fält
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Konfigurera anpassade fält {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Anpassade fält"
>abstract="Anpassade fält är ytterligare attribut som läggs till i färdiga scheman via Adobe Campaign-konsolen. De finns nu i webbgränssnittet."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Se versionsinformation"



Anpassade fält är ytterligare attribut som läggs till i färdiga scheman via Adobe Campaign-konsolen. Läs mer i [Adobe Campaign v8-dokumentationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

Dessa anpassade fält visas på olika skärmar, till exempel information om en profil eller en testprofil.

I webbanvändargränssnittet kan du inte skapa anpassade fält, men du kan ändra hur de visas. Ändringarna gäller för alla Campaign-användare.

>[!NOTE]
>
>Du måste ha administratörsbehörighet för att kunna ändra anpassade fält.

Anpassade fält är tillgängliga i följande scheman:

* Mottagare (nms)
* Kampanjer (nms)
* Leveranser (nms)
* Fröadresser (nms)

Så här konfigurerar du anpassade fält:

1. Klicka på **Scheman** under **Administration**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. Leta reda på det önskade schemat, till exempel schemat **Mottagare (nms)**.

   ![](assets/custom-fields2.png){zoomable="yes"}

1. Klicka på knappen **Fler åtgärder** och välj **Redigera anpassad information**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   Skärmen **Redigera anpassad detalj** visar alla anpassade fält och deras typ.

   ![](assets/custom-fields4.png){zoomable="yes"}

   På den här skärmen kan du utföra följande åtgärder:

   * ändra ordningen på de olika fälten med upp- och nedpilarna.
   * gör fältet obligatoriskt: markera kryssrutan **Obligatoriskt**.
   * gör fältet synligt eller dolt: klicka på knappen **Synligt** .
   * lägg till ett synlighetsvillkor: klicka på knappen **Synligt om** och skriv xtk-uttrycket med de tillgängliga xtk-funktionerna.

1. Navigera till skärmen som visar det anpassade fältet. I vårt exempel är det profilinformationsskärmen.

   ![](assets/custom-fields5.png){zoomable="yes"}
