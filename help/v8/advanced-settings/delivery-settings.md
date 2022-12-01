---
audience: end-user
title: Avancerade inställningar
description: Webbdokumentation för Campaign v8
source-git-commit: c90d8a5eff6169945d381f3250cb3e4d06194d31
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 1%

---

# Avancerade inställningar {#advanced-settings}

>[!NOTE]
>
>Dokumentationen håller på att byggas och uppdateras ofta. Den slutliga versionen av detta innehåll är klar i januari 2023.

De här inställningarna är tekniska leveransparametrar som definieras i e-postmallen. Om du vill ändra någon av dem för en viss leverans, ska du vara försiktig.

## Inställningar för e-postleverans {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Alla tekniska leveransparametrar från mallen.
Ändra bara parametrar, ingen generering här.
Enligt behörigheter ska de inte ändra detta med försiktighet. Kontrollera och ändra endast typologiregeln -> rest som är definierad i mallen

## Typologi {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologi"
>abstract="Med typologi kan du styra, filtrera och övervaka leveransen."

### Tryckparameter {#pressure-parameter}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Leveransvikt"
>abstract="Med leveransvikter kan ni identifiera leveranser med högsta prioritet inom ramen för tryckhantering. Meddelanden med högst vikt har prioritet."

### Kapacitetsinställningar {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Mottagarens betydelse"
>abstract="TBC"


## Målgrupp {#audience}

## Leverans {#delivery}

### Återförsök {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximalt antal återförsök"
>abstract="Om ett meddelande misslyckas på grund av ett tillfälligt fel, kommer nya försök att utföras under leveransens varaktighet."

## Godkännande {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Godkännandeläge"
>abstract="Varje steg i en leverans kan godkännas för att säkerställa full övervakning och kontroll av de olika processerna."

## Giltighet {#validity}

### Giltighetsperiod {#validity-period}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Leveransens varaktighet"
>abstract="I fältet Leveransvaraktighet kan du ange gränsen för globala leveransförsök. Detta innebär att Adobe Campaign skickar meddelanden som börjar på startdatumet och sedan, för meddelanden som bara returnerar ett fel, kommer regelbundna, konfigurerbara försök att utföras tills giltighetsgränsen nås."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Giltighetsgräns för resurser"
>abstract="Fältet Giltighetsgräns används för överförda resurser, huvudsakligen för spegelsidan och bilder. Resurserna på den här sidan är giltiga under en begränsad tid."


### Spåra {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Giltighetsperiod"
>abstract="Det här alternativet anger hur länge spårningen ska aktiveras på URL-adresserna."














