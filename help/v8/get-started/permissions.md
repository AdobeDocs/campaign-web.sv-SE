---
audience: end-user
title: Behörighetshantering på Campaign-webben
description: Läs mer om behörigheter på Campaign-webben v8
badge: label="Beta"
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 0%

---

# Åtkomst och behörigheter {#access-and-permissions}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="Behörighet krävs"
>abstract="Din administratör måste ge dig behörighet innan du kan skapa det här objektet."


>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="Den här målgruppen är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här målgruppen. Kontakta administratören om det behövs för att ge dig åtkomst."


>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Tjänsten är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här tjänsten. Kontakta administratören om det behövs för att ge dig åtkomst."


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Den här kampanjen är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här kampanjen. Kontakta administratören om det behövs för att ge dig åtkomst."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Leveransen är skrivskyddad"
>abstract="Du har inte behörighet att redigera den här leveransen. Kontakta administratören om det behövs för att ge dig åtkomst."


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Arbetsflödet är skrivskyddat"
>abstract="Du har inte behörighet att redigera det här arbetsflödet. Kontakta administratören om det behövs för att ge dig åtkomst."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Arbetsflödet är skrivskyddat"
>abstract="Du kan inte redigera det här arbetsflödet på grund av att arbetsytan inte stöds eller är inkompatibel."

Åtkomstkontroll kan begränsa åtkomst till objekt och data från huvudlistor, till exempel leveranser, mottagare eller arbetsflöden. Dessa begränsningar gäller även för **Explorer** navigeringsträd. Dessutom behöver du behörighet att skapa, ta bort, duplicera och redigera objekt från användargränssnittet.

Åtkomstkontrollen hanteras i Campaign Client Console. Alla behörigheter på Campaign Web synkroniseras med behörigheter på Campaign Client Console. Endast kampanjadministratörer kan definiera och ändra användarbehörigheter. Läs mer om användarbehörigheter i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html){target="_blank"}.

När du surfar i användargränssnittet i Campaign kan du komma åt data, objekt och funktioner beroende på dina behörigheter. Om du till exempel inte har åtkomstbehörighet till en mapp kan du inte se den. Dina behörigheter påverkar även objekt och datahantering. Utan skrivbehörighet för en viss mapp kan du inte skapa en leverans i den mappen, även om du kan se den i användargränssnittet.

## Visa behörigheter {#view-permissions}

Från **Explorer** kan du bläddra bland behörigheter för varje mapp. Dessa behörigheter anges i klientkonsolen och används för att organisera och styra åtkomsten till Campaign-data.

Så här visar du behörigheter för en mapp:

1. Från **Explorer** vänster navigeringsmeny väljer du en mapp.
1. Klicka på de tre punkterna i det övre högra hörnet och välj **Mappbehörigheter**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. Kontrollera detaljer på skärmen enligt nedan:

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   En grupp, eller en operator, kan ha behörigheten Läs, Skriv och/eller Ta bort för data som lagras i den valda mappen.

   Om **Sprid** om du aktiverar det här alternativet används alla behörigheter som definierats för en mapp på alla dess undermappar. Dessa behörigheter kan överladdas för varje undermapp.

   Om **Systemmapp** är aktiverat, åtkomst är tillåten för alla operatorer, oavsett deras behörigheter.

Läs mer om mappbehörigheter i [Kampanjdokumentation v8 (klientkonsol)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## Arbeta med mappar {#folders}

Du kan skapa, byta namn på, ordna om och flytta mappar för att ordna dina komponenter och data. Du kan också ta bort mappar från samma meny.

>[!CAUTION]
>
>När du tar bort en mapp tas även alla data som lagras i mappen bort.

Så här skapar du en mapp:

1. Från **Explorer** vänster navigeringsmeny väljer du en mapp.
1. Klicka på de tre punkterna i det övre högra hörnet och välj **Skapa ny undermapp**.
1. Ange namnet på mappen och spara.

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   Mappen läggs till som en undermapp till den aktuella mappen. Bläddra till den nya mappen för att skapa komponenter direkt i den. Du kan också skapa en komponent från en mapp och spara den i den nya mappen från **Ytterligare alternativ** av egenskaperna enligt nedan för en leverans:

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}
