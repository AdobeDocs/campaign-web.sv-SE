---
audience: end-user
title: Hantera varumärke
description: Lär dig skapa och hantera riktlinjer för ert varumärke
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# Skapa och hantera varumärken {#brands}

Varumärkesriktlinjerna är en omfattande uppsättning regler och standarder som definierar ett varumärkes visuella och verbala identitet. De fungerar som referens för att säkerställa en enhetlig varumärkesrepresentation i alla marknadsförings- och kommunikationskanaler.

I [!DNL Adobe Campaign Web] kan användare ange och ordna varumärkesinformation manuellt eller överföra varumärkesstöddokument för automatisk dataextrahering.

## Få tillgång till varumärken {#generative-access}

För att få åtkomst till menyn **[!UICONTROL Brands]** i [!DNL Adobe Campaign Web] måste användarna tilldelas produktprofilerna **[!UICONTROL Administrator (admin)]** och **[!UICONTROL Brand kit]** för att kunna skapa och hantera varumärken. För skrivskyddad åtkomst behöver användarna produktprofilen [!UICONTROL AI assistant]. [Läs mer](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

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

1. Klicka på **[!UICONTROL Brands]** på menyn **[!UICONTROL Create brand]**.

   ![Varumärkesmenyn med alternativet Skapa varumärke](assets/brands-1.png)

1. Ange en **[!UICONTROL Name]** för ditt varumärke.

1. Dra och släpp eller markera filen för att ladda upp varumärkesriktlinjerna och extrahera automatiskt relevant varumärkesinformation. Klicka på **[!UICONTROL Create brand]**.

   Processen för informationsextrahering börjar nu. Observera att det kan ta flera minuter att slutföra.

   ![Filöverföring för extrahering av varumärkesriktlinjer](assets/brands-2.png)

1. Standarderna för att skapa innehåll och visuellt innehåll är nu automatiskt ifyllda. Bläddra bland de olika flikarna för att anpassa informationen efter behov. [Läs mer](#personalize)

1. På den avancerade menyn i varje avsnitt eller kategori kan du lägga till referenser för att extrahera relevant varumärkesinformation automatiskt.

   Använd alternativen **[!UICONTROL Clear section]** eller **[!UICONTROL Clear category]** om du vill ta bort befintligt innehåll.

   ![](assets/brands-15.png)

1. När konfigurationen är klar klickar du på **[!UICONTROL Save]** och sedan på **[!UICONTROL Publish]** för att göra din varumärkesriktlinje tillgänglig i AI Assistant.

1. Klicka på **[!UICONTROL Edit brand]** om du vill ändra det publicerade varumärket.

   >[!NOTE]
   >
   >Detta skapar en temporär kopia i redigeringsläge och ersätter den publicerade versionen.

   ![Alternativet Redigera varumärke på menyn Varumärken](assets/brands-8.png)

1. Öppna den avancerade menyn på din **[!UICONTROL Brands]**-kontrollpanel genom att klicka på ikonen ![](assets/do-not-localize/Smock_More_18_N.svg) för att:

   * Visa varumärke
   * Redigera
   * Markera som standardmärke
   * Duplicera
   * Publicera
   * Avpublicera
   * Ta bort

   ![Avancerade menyalternativ på kontrollpanelen för varumärken](assets/brands-6.png)

Riktlinjerna för ditt varumärke finns nu i listrutan **[!UICONTROL Brand]** i AI Assistant-menyn. På så sätt kan AI Assistant generera innehåll och resurser som är anpassade efter dina specifikationer. [Läs mer om AI Assistant](../content/generative-gs.md)

Ni kan också använda varumärkesriktlinjerna för att utvärdera er innehållskvalitet och varumärkesanpassning. [Läs mer om validering av innehållskvalitet](brands-score.md#validate-quality)

![AI-assistentmeny med listrutan Märke](assets/brands_6.png)

### Ange ett standardmärke {#default-brand}

Du kan ange att ett standardvarumärke ska tillämpas automatiskt när du genererar innehåll och beräknar justeringspoäng när kampanjer skapas.

Om du vill ange ett standardmärke går du till **[!UICONTROL Brands]**-instrumentpanelen. Öppna den avancerade menyn genom att klicka på ikonen ![](assets/do-not-localize/Smock_More_18_N.svg) och välja **[!UICONTROL Mark as default brand]**.

![Avancerade menyalternativ på kontrollpanelen för varumärken](assets/brands-6.png)

