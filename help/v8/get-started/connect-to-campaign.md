---
title: Anslut till Adobe Campaign webbgränssnitt
description: Lär dig hur du ansluter till Adobe Campaign webbgränssnitt
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
source-git-commit: 11bad3c29ebeb4e81187ae2c1786262b6ac89a70
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Anslut till Adobe Campaign {#connect-to-campaign}

Experience Cloud är Adobe integrerade program, produkter och tjänster för digital marknadsföring. Från det intuitiva gränssnittet får du snabbt tillgång till dina molnprogram, produktfunktioner och tjänster. Lär dig hur du ansluter till Adobe Experience Cloud och kommer åt Adobe Campaign webbgränssnitt på den här sidan.

## Logga in på Adobe Experience Cloud {#sign-in-to-exc}

Du kan bara använda enkel inloggning (SSO) för att ansluta till Campaign. Vanligtvis ger Experience Cloud-administratörer tillgång till program och tjänster. Följ stegen i din e-postinbjudan till Experience Cloud.

De grundläggande stegen för att logga in på Adobe Experience Cloud är:

1. Bläddra till [Adobe Experience Cloud](https://experience.adobe.com/).

1. Logga in med din Adobe ID eller Enterprise ID. Läs mer om identitetstyper på Adobe i [den här artikeln](https://helpx.adobe.com/enterprise/using/identity.html).

   När du har loggat in på Experience Cloud får du snabbt tillgång till alla dina lösningar och appar.

   ![](assets/exc-home.png)

1. Kontrollera att du är i rätt organisation.

   ![](assets/exc-orgs.png)

   Läs mer om organisationer i Adobe Experience Cloud i [den här artikeln](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=sv).


## Tillgång till Adobe Campaign {#access-to-campaign}

Om du vill komma åt din Campaign-miljö väljer du **Campaign** i avsnittet **Snabbåtkomst** på Adobe Experience Cloud hemsida.

Om du redan är ansluten till en annan Adobe Experience Cloud-lösning kan du även bläddra till Campaign-miljön från lösningsväljaren längst upp till höger på skärmen.

![](assets/solution-switcher.png)

Om du har tillgång till flera miljöer, inklusive Campaign Control Panel, klickar du på knappen **Launch** för att få rätt instans.

![](assets/launch-campaign.png)

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
>title="Mottagarens skrivskyddade profil"
>abstract="Du har inte behörighet att redigera detta prodike. Om det behövs kontaktar du administratören för att ge dig åtkomst."

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Denna kampanj är skrivskyddad"
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

## Övre navigering i Adobe Experience Cloud {#top-bar}

Bläddra i det övre fältet i gränssnittet för att:

* dela feedback om användargränssnittet i Campaign Web
* växla mellan olika organisationer
* växla mellan era Adobe Experience Cloud-lösningar och appar
* sök efter hjälp om [Adobe Experience League](https://experienceleague.adobe.com/docs/)
* kontrollera produktmeddelanden
* redigera din Adobe-profil och hantera inställningar, till exempel [uppdatera ditt favoritspråk](#language-pref) eller [växla till ljust/mörkt tema](#dark-theme)

![](assets/do-not-localize/unified-shell.png)

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


Ditt standardspråk för Campaign Web bestäms av det språk som anges i din användarprofil. Den är inte relaterad till språket på Campaign-servern och klientkonsolen.

Så här ändrar du språk:

1. Klicka på din profilikon längst upp till höger och välj sedan **Inställningar**.
1. Klicka sedan på den språklänk som visas under din e-postadress.
1. Välj önskat språk och klicka på **Spara**. Du kan välja ett andra språk om komponenten som du använder inte är lokaliserad till ditt första språk.

## Mörka och ljusa teman {#dark-theme}

Adobe Campaign finns i ljusa och mörka teman. Som standard är användargränssnittet aktiverat i ljust tema. Om du vill växla till det mörka temat klickar du på din profilikon och använder **det mörka temat** för att aktivera/inaktivera det.

Användarprofilsinställningar och kontoinställningar beskrivs i [det här avsnittet](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html#preferences).

Läs mer om Experience Cloud Central Interface Components i [den här dokumentationen](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html).
