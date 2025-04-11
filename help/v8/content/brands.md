---
audience: end-user
title: Hantera varumärke
description: Lär dig skapa och hantera riktlinjer för ert varumärke
hide: true
hidefromtoc: true
badge: label="Beta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Skapa och hantera varumärken {#brands}

>[!AVAILABILITY]
>
>Den här funktionen är en privat betaversion. Den kommer att bli allt mer tillgänglig för alla kunder i kommande versioner.

Varumärkesriktlinjerna är en omfattande uppsättning regler och standarder som definierar ett varumärkes visuella och verbala identitet. De fungerar som referens för att säkerställa en enhetlig varumärkesrepresentation i alla marknadsförings- och kommunikationskanaler.

I [!DNL Adobe Campaign Web] kan användare ange och ordna varumärkesinformation manuellt eller överföra varumärkesstöddokument för automatisk dataextrahering.

## Få tillgång till varumärken {#generative-access}

För att få åtkomst till menyn **[!UICONTROL Brands]** i [!DNL Adobe Campaign Web] måste användarna tilldelas produktprofilerna **[!UICONTROL Administrator (admin)]** och **[!UICONTROL Brand kit]** för att kunna skapa och hantera varumärken. För skrivskyddad åtkomst behöver användarna produktprofilen [!UICONTROL AI assistant].

[Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Lär dig hur du tilldelar varumärkesrelaterade behörigheter

1. Gå till din Campaign-produkt på startsidan för [Admin Console](https://adminconsole.adobe.com/enterprise).

   ![Admin Console hemsida med tillgång till Campaign-produkter](assets/brands_admin_1.png)

1. Välj **[!DNL Product profile]** baserat på den behörighetsnivå du vill ge användaren.

   ![Val av produktprofil i Admin Console](assets/brands_admin_2.png)

1. Klicka på **[!DNL Add users]** för att tilldela den valda produktprofilen.

   ![Alternativet Lägg till användare i Admin Console](assets/brands_admin_3.png)

1. Skriv användarens namn, användargrupp eller e-postadress.

1. Klicka på **Spara** om du vill använda ändringarna.

Användare som redan har tilldelats den här rollen får sina behörigheter automatiskt uppdaterade.

+++

## Skapa ert varumärke {#create-brand-kit}

Följ stegen nedan om du vill skapa och hantera riktlinjer för ditt varumärke.

Användarna kan antingen ange detaljerna manuellt eller ladda upp ett varumärkesdokument för att extrahera informationen automatiskt:

1. Välj **[!UICONTROL Brands]** på menyn **[!UICONTROL Content management]**.

1. Klicka på **[!UICONTROL Create brand]** på menyn **[!UICONTROL Brands]**.

   ![Varumärkesmenyn med alternativet Skapa varumärke](assets/brands_1.png)

1. Ange en **[!UICONTROL Name]** för ditt varumärke.

1. Dra och släpp eller markera filen för att ladda upp varumärkesriktlinjerna och extrahera relevant varumärkesinformation automatiskt. Klicka på **[!UICONTROL Create brand]**.

   Informationsextraheringsprocessen börjar. Observera att det kan ta flera minuter att slutföra.

   ![Filöverföring för extrahering av varumärkesriktlinjer](assets/brands_7.png)

1. Standarderna för innehåll och visuellt skapande fylls i automatiskt. Bläddra bland de olika flikarna för att anpassa informationen efter behov.

1. Klicka på ![Lägg till ikon](assets/do-not-localize/Smock_Add_18_N.svg) på fliken **[!UICONTROL Writing Style]** om du vill lägga till en stödlinje eller ett undantag, inklusive exempel.

   ![Fliken Skriver format med alternativet Lägg till stödlinje](assets/brands_2.png)

1. Klicka på ![Lägg till ikon](assets/do-not-localize/Smock_Add_18_N.svg) på fliken **[!UICONTROL Visual content]** om du vill lägga till ytterligare en stödlinje eller ett undantag.

1. Om du vill lägga till en bild som visar korrekt användning väljer du **[!UICONTROL Examples]** och klickar på **[!UICONTROL Select image]**. Du kan också lägga till en bild som visar felaktig användning som ett exkluderingsexempel.

   ![Fliken Visuellt innehåll med exempelbildalternativ](assets/brands_3.png)

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]** och sedan på **[!UICONTROL Publish]** för att göra din varumärkesriktlinje tillgänglig i AI-assistenten.

1. Klicka på **[!UICONTROL Edit brand]** om du vill ändra det publicerade varumärket.

   >[!NOTE]
   >
   >Detta skapar en temporär kopia i redigeringsläge och ersätter den publicerade versionen.

   ![Alternativet Redigera varumärke på menyn Varumärken](assets/brands_4.png)

1. Öppna den avancerade menyn på din **[!UICONTROL Brands]**-kontrollpanel genom att klicka på ikonen ![Fler alternativ](assets/do-not-localize/Smock_More_18_N.svg) för att:

   * Visa varumärke
   * Redigera
   * Duplicera
   * Publicera
   * Avpublicera
   * Ta bort

   ![Avancerade menyalternativ på kontrollpanelen för varumärken](assets/brands_5.png)

Riktlinjerna för ditt varumärke finns nu i listrutan **[!UICONTROL Brand]** i AI-assistentmenyn. På så sätt kan AI-assistenten generera innehåll och resurser som är anpassade efter dina specifikationer. [Läs mer om AI-assistenten](../email/generative-gs.md)

![AI-assistentmeny med listrutan Märke](assets/brands_6.png)