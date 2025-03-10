---
audience: end-user
title: Hantera varumärke
description: Lär dig skapa och hantera riktlinjer för ert varumärke
hide: true
hidefromtoc: true
badge: label="Beta" type="Informative"
source-git-commit: e6e23a758cce657b582174e522d61193dc7326cf
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Skapa och hantera varumärken {#brands}

>[!AVAILABILITY]
>
>Den här funktionen är en privat betaversion. Den kommer att finnas tillgänglig successivt för alla kunder i framtida versioner.

Varumärkesriktlinjerna är en omfattande uppsättning regler och standarder som definierar ett varumärkes visuella och verbala identitet. De fungerar som referens för att säkerställa en enhetlig varumärkesrepresentation i alla marknadsförings- och kommunikationskanaler.

I [!DNL Adobe Campaign Web] kan du nu ange och ordna din varumärkesinformation manuellt eller överföra varumärkesstöddokument för automatisk dataextrahering.

## Få tillgång till varumärken {#generative-access}

För att få åtkomst till menyn **[!UICONTROL Brands]** i [!DNL Adobe Campaign Web] måste användarna tilldelas produktprofilerna **[!UICONTROL Administrator (admin)]** och **[!UICONTROL Brand kit]** för att kunna skapa och hantera varumärken. För skrivskyddad åtkomst behöver användarna produktprofilen [!UICONTROL AI assistant].

[Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++  Lär dig hur du tilldelar varumärkesrelaterade behörigheter

1. Gå till din Campaign-produkt på startsidan för [Admin Console](https://adminconsole.adobe.com/enterprise).

   ![](assets/brands_admin_1.png)

1. Välj **[!DNL Product profile]** beroende på vilken behörighetsnivå du vill ge användaren.

   ![](assets/brands_admin_2.png)

1. Klicka på **[!DNL Add users]** för att tilldela den valda produktprofilen.

   ![](assets/brands_admin_3.png)

1. Ange användarens namn, användargrupp eller e-postadress.

1. Klicka på **Spara** om du vill använda ändringarna.

Alla användare som redan har tilldelats den här rollen får sina behörigheter automatiskt uppdaterade.

+++

## Skapa ert varumärke {#create-brand-kit}

Följ stegen nedan om du vill skapa och hantera riktlinjer för ditt varumärke.

Om du vill skapa och hantera din varumärkesriktlinje kan du antingen ange detaljerna själv eller överföra ditt varumärkesriktlinjer så att informationen extraheras automatiskt:


1. Välj **[!UICONTROL Brands]** på menyn **[!UICONTROL Content management]**.

1. Klicka på **[!UICONTROL Create brand]** på menyn **[!UICONTROL Brands]**.

   ![](assets/brands_1.png)

1. Ange en **[!UICONTROL Name]** för ditt varumärke.

1. Dra och släpp eller markera filen för att ladda upp varumärkesriktlinjerna och extrahera automatiskt relevant varumärkesinformation. Klicka på **[!UICONTROL Create brand]**.

   Processen för informationsextrahering börjar nu. Observera att det kan ta flera minuter att slutföra.

   ![](assets/brands_7.png)

1. Standarderna för att skapa innehåll och visuellt innehåll är nu automatiskt ifyllda. Bläddra bland de olika flikarna för att anpassa informationen efter behov.

1. Klicka på ![](assets/do-not-localize/Smock_Add_18_N.svg) på fliken **[!UICONTROL Writing Style]** om du vill lägga till en stödlinje eller ett undantag, inklusive exempel.

   ![](assets/brands_2.png)

1. Klicka på ![](assets/do-not-localize/Smock_Add_18_N.svg) på fliken **[!UICONTROL Visual content]** om du vill lägga till ytterligare en stödlinje eller ett undantag.

1. Om du vill lägga till en bild som visar korrekt användning väljer du **[!UICONTROL Examples]** och klickar på **[!UICONTROL Select image]**. Du kan också lägga till en bild som visar felaktig användning som ett exkluderingsexempel.

   ![](assets/brands_3.png)

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]** och sedan på **[!UICONTROL Publish]** för att göra din varumärkesriktlinje tillgänglig i AI-assistenten.

1. Klicka på **[!UICONTROL Edit brand]** om du vill ändra det publicerade varumärket.

   >[!NOTE]
   >
   >Detta skapar en temporär kopia i redigeringsläge och ersätter den publicerade versionen.

   ![](assets/brands_4.png)

1. Öppna den avancerade menyn på din **[!UICONTROL Brands]**-kontrollpanel genom att klicka på ikonen ![](assets/do-not-localize/Smock_More_18_N.svg) för att:

   * Visa varumärke
   * Redigera
   * Duplicera
   * Publicera
   * Avpublicera
   * Ta bort

   ![](assets/brands_5.png)

Riktlinjerna för ditt varumärke är nu tillgängliga från listrutan **[!UICONTROL Brand]** i AI-assistentmenyn, vilket gör att det kan generera innehåll och resurser som är anpassade till dina specifikationer. [Läs mer om AI-assistenten](gs-generative.md)

![](assets/brands_6.png)
