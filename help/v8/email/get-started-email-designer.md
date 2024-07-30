---
audience: end-user
title: Redigera e-postinnehållet
description: Lär dig hur du börjar bygga innehåll med e-post-Designer i webbgränssnittet i Campaign
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 7%

---

# Komma igång med e-postdesignern {#get-started-email-designer}


När du har skapat ett e-postmeddelande i Adobe Campaign måste du definiera dess innehåll.

Med e-post-Designer kan du skapa engagerande, individuellt anpassade e-postmeddelanden via ett intuitivt dra-och-släpp-gränssnitt. Vare sig du börjar från en tom sida, importerar ett befintligt innehåll eller använder befintliga mallar kan du utforma och förfina allt innehåll för varje e-postmeddelande, oavsett om det är en reklam eller en transaktion.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Använd e-postdesignfunktionerna i [!DNL Campaign] för att enkelt skapa responsiva e-postmeddelanden. [Läs mer](create-email-content.md)

* Förbättra kundernas upplevelse genom att skapa personaliserade utifrån deras profilattribut. [Läs mer](../personalization/personalize.md)

* Konfigurera fält för villkorligt innehåll för att skapa dynamisk personalisering baserat på mottagarens profil. [Läs mer](../personalization/conditions.md)

## Bästa praxis för e-postdesign {#best-practices}

När du skickar e-postmeddelanden är det viktigt att tänka på att mottagarna kan vidarebefordra dem, vilket ibland kan orsaka problem med e-postens återgivning. Detta gäller särskilt när du använder CSS-klasser som kanske inte stöds av e-postleverantören som används för vidarebefordran, till exempel om du använder CSS-klassen&quot;is-desktop-hidden&quot; för att dölja en bild på mobila enheter.

För att minimera dessa återgivningsproblem rekommenderar vi att du håller e-postdesignstrukturen så enkel som möjligt. Försök använda en enda design som fungerar bra för både datorer och mobila enheter, och undvik att använda komplexa CSS-klasser eller andra designelement som kanske inte stöds fullt ut av alla e-postklienter. Genom att följa dessa rutiner kan du se till att dina e-postmeddelanden återges korrekt, oavsett hur mottagarna visar eller vidarebefordrar dem.

## Börja skapa ditt innehåll {#start-authoring}

Gå igenom skärmen [Redigera innehåll](edit-content.md) på kontrollpanelen för e-postleverans för att öppna Designer hemsida. Därifrån kan du välja hur du vill utforma e-postmeddelanden bland följande alternativ:

* **Designa din e-post från grunden** via e-postdesignerns gränssnitt. Lär dig hur du utformar ditt e-postinnehåll i [det här avsnittet](create-email-content.md).

* **Kod eller klistra in Raw-HTML** direkt i e-postdesignern. Lär dig hur du kodar ditt eget innehåll i [det här avsnittet](code-content.md).

* **Importera befintligt HTML-innehåll** från en fil eller en ZIP-mapp. Lär dig hur du importerar ett e-postinnehåll i [det här avsnittet](existing-content.md).

* **Välj ett befintligt innehåll** i en lista med inbyggda eller anpassade mallar. Lär dig hur du arbetar med e-postmallar [det här avsnittet](create-email-templates.md).

  ![](assets/email_designer_create_options.png){zoomable="yes"}
