---
title: Skapa villkorsstyrt innehåll
description: Lär dig hur du definierar villkor för att anpassa ditt innehåll i Adobe Campaign webbgränssnitt
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 5598a82bf745659b8c1db8cb51b1a82cfd184093
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# Skapa villkorsstyrt innehåll{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Skapa villkorsstyrt innehåll"
>abstract="Skapa villkorsstyrt innehåll för att definiera dynamisk personalisering baserat på mottagarens profil och ersätt automatiskt textblock och bilder när vissa villkor uppfylls. Den här funktionen kan lyfta era kampanjer till nya höjder och leverera målinriktade, personaliserade upplevelser till er målgrupp."


Villkorligt innehåll är en kraftfull funktion som gör att du kan skapa dynamisk personalisering baserat på mottagarens profil och automatiskt ersätta textblock och bilder när vissa villkor uppfylls. Den här funktionen kan lyfta era kampanjer till nya höjder och leverera målinriktade, personaliserade upplevelser till er målgrupp.

Genom att konfigurera fält för villkorligt innehåll kan du skapa avancerad dynamisk personalisering som till exempel baseras på mottagarens profil. Textblock, länkar, ämnesrader och/eller bilder ersätts i meddelandeinnehållet när ett visst villkor är uppfyllt. Du kan t.ex. visa&quot;Herr&quot; eller&quot;fru&quot; enligt värdet i fältet Kön i Adobe Campaign-databasen, eller inkludera en annan länk baserat på vilket mottagarspråk som föredras.

## Anpassningssyntax{#perso-syntax}



## Arbeta med villkor i personaliseringsredigeraren{#condition-perso-editor}

Så här definierar du ett villkorligt innehåll för en leverans:

1. Öppna en leverans och redigera innehållet.
1. Klicka på **[!UICONTROL Open personalization dialog]** ikon, till exempel för SMS, till höger om meddelandefältet.

   ![](assets/open-perso-editor-sms.png)

1. I personaliseringsredigeraren går du till **[!UICONTROL Helper functions]**.
1. Klicka på plustecknet (+) bredvid ikonen **If** funktion. Följande rad ska läggas till på den centrala skärmen:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Ersätt `<FIELD>` av ett personaliseringsfält. Exempel: mottagarens företag: `recipient.company`.
1. Ersätt `<VALUE>` med det värde som ska uppfyllas. Exempel, `ADOBE`.




## Exempel: villkorlig SMS-ämnesrad{#condition-subject-line}

Följ stegen nedan för att skapa en villkorlig ämnesrad för ett SMS-meddelande:

1. Öppna en leverans och redigera innehållet.
1. Klicka på ikonen Öppna personalisering till höger om ämnesraden.
1. I personaliseringsredigeraren går du till


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
