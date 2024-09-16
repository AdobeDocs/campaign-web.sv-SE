---
title: Anslut till Adobe Campaign webbgränssnitt
description: Lär dig hur du ansluter till Adobe Campaign webbgränssnitt
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
source-git-commit: 581b5ae12d7e1ca2a68e51923b765e0366e84b66
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Anslut till Adobe Campaign {#connect-to-campaign}

Experience Cloud är en integrerad familj av program, produkter och tjänster för digital marknadsföring i Adobe. Från det intuitiva gränssnittet får du snabbt tillgång till dina molnprogram, produktfunktioner och tjänster. Lär dig hur du ansluter till Adobe Experience Cloud och kommer åt Adobe Campaign webbgränssnitt på den här sidan.

## Logga in på Adobe Experience Cloud {#sign-in-to-exc}

Du kan bara använda enkel inloggning (SSO) för att ansluta till Campaign. Administratörer i Experience Cloud ger vanligtvis tillgång till program och tjänster. Följ stegen i din e-postinbjudan till Experience Cloud.

Så här loggar du in på Adobe Experience Cloud:

1. Gå till [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}.

1. Logga in med ditt Adobe ID eller Enterprise ID. Läs mer om identitetstyper på Adobe i [den här artikeln](https://helpx.adobe.com/enterprise/using/identity.html){target="_blank"}.

   När du har loggat in på Experience Cloud får du snabbt tillgång till alla dina lösningar och appar.

   ![](assets/exc-home.png){zoomable="yes"}

1. Kontrollera att du är i rätt organisation.

   ![](assets/exc-orgs.png){zoomable="yes"}{width="50%" align="left"}

   Läs mer om organisationer i Adobe Experience Cloud i [den här artikeln](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=sv){target="_blank"}.


## Tillgång till Adobe Campaign {#access-to-campaign}

Om du vill komma åt din Campaign-miljö väljer du **Campaign** i avsnittet **Snabbåtkomst** på Adobe Experience Cloud hemsida.

Om du redan är ansluten till en annan Adobe Experience Cloud-lösning kan du även bläddra till Campaign-miljön från lösningsväljaren längst upp till höger på skärmen.

![](assets/solution-switcher.png){zoomable="yes"}

Om du har tillgång till flera miljöer, inklusive Campaign Control Panel, klickar du på knappen **Launch** för att få rätt instans.

![](assets/launch-campaign.png){zoomable="yes"}

Du är nu ansluten till Campaign. Lär dig hur du börjar använda användargränssnittet på [den här sidan](user-interface.md).

### Åtkomstkontroll {#access-control}

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
>id="acw_recipients_readonlyprofile"
>title="Mottagarna har skrivskyddad profil"
>abstract="Du har inte behörighet att redigera den här profilen. Kontakta administratören om det behövs för att ge dig åtkomst."

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

Åtkomstkontroll kan begränsa åtkomst till objekt och data från huvudlistor, till exempel leveranser, mottagare eller arbetsflöden. Dessa begränsningar gäller även i Utforskarens navigeringsträd. Dessutom behöver du behörighet att skapa, ta bort, duplicera och redigera objekt från användargränssnittet.

Alla behörigheter på Campaign Web synkroniseras med behörigheter på Campaign Client Console. Endast kampanjadministratörer kan definiera och ändra användarbehörigheter.

När du surfar i användargränssnittet i Campaign kan du komma åt data, objekt och funktioner beroende på dina behörigheter. Om du till exempel inte har åtkomstbehörighet till en mapp kan du inte se den. Dina behörigheter påverkar även objekt och datahantering. Utan skrivbehörighet för en viss mapp kan du inte skapa en leverans i den mappen, även om du kan se den i användargränssnittet.

Du kan lära dig att [visa och hantera behörigheter här](permissions.md).

## Adobe Experience Cloud toppnavigering {#top-bar}

Bläddra i gränssnittets övre fält till:

* dela feedback om gränssnittet i Campaign Web
* växla mellan olika organisationer
* växla mellan era Adobe Experience Cloud-lösningar och appar
* sök efter hjälp om [Adobe Experience League](https://experienceleague.adobe.com/docs/){target="_blank"}
* kontrollera produktmeddelanden
* redigera din Adobe-profil och hantera inställningar, till exempel [uppdatera ditt favoritspråk](#language-pref) eller [växla till ljust/mörkt tema](#dark-theme)

![](assets/do-not-localize/unified-shell.png){zoomable="yes"}{width="50%" align="left"}

## Webbläsare som stöds {#browsers}

Adobe Campaign Web är utformat för att fungera optimalt i den senaste versionen av Google Chrome, Safari och Microsoft Edge. Du kan ha problem med att använda vissa funktioner i äldre versioner eller i andra webbläsare.

## Språkinställningar {#language-pref}

Adobe Campaign Web finns på följande språk:

* Engelska (USA) - EN-US
* Franska - FR
* Tyska - DE
* Italienska - IT
* Spanska - ES
* Portugisiska (Brasilien) - PTBR
* Japanska - JP
* Koreanska - KR
* Förenklad kinesiska - CHS
* Traditionell kinesiska - CHT


Ditt standardspråk för Campaign Web avgörs av det språk du föredrar i din användarprofil. Det gäller inte språket för er Campaign-server och kundkonsol.

Så här byter du språk:

1. Klicka på din profilikon längst upp till höger och välj sedan **Inställningar**.
1. Klicka sedan på den språklänk som visas under din e-postadress.
1. Välj önskat språk och klicka på **Spara**. Du kan välja ett andra språk om komponenten som du använder inte är lokaliserad till ditt första språk.

<!--
>[!CAUTION]
>
>If you plan to use [AI-powered contextual help](-using-ai.md) capabilities, you must set your prefered language to English. Other languages are not supported.
>
-->

## Mörka och ljusa teman {#dark-theme}

Adobe Campaign finns i ljusa och mörka teman. Som standard är användargränssnittet aktiverat i ljust tema. Om du vill växla till det mörka temat klickar du på din profilikon och använder **det mörka temat** för att aktivera/inaktivera det.

Användarprofilsinställningar och kontoinställningar beskrivs i [det här avsnittet](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html#preferences){target="_blank"}.

Läs mer om gränssnittskomponenter i Experience Cloud Central i [den här dokumentationen](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html){target="_blank"}.
