---
title: Hantering av tidszoner
description: Läs om hur Adobe Campaign Web UI visar datum- och tidsvärden baserat på tidszoner för webbläsare, operatör, arbetsflöde och server.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 2%

---

# Hantering av tidszoner {#timezone-management}

Adobe Campaign Web UI visar alla datum- och tidsvärden enligt den **lokala tidszonen i användarens webbläsare**. Detta kan leda till skillnader vid jämförelse av tidsstämplar mellan webbgränssnittet och klientkonsolen.

I det här avsnittet förklaras förväntade skillnader mellan tidszonerna för körning av **webbgränssnittet**, **klientkonsolen** och **arbetsflödet**.

>[!NOTE]
>
>Inga data som lagras på servern har ändrats. Endast visningen i gränssnittet ändras.

## Viktiga begrepp

* **Serverns tidszon**: Serverns tidszon motsvarar den tidszon som konfigurerats på serverns operativsystem. Alla tidsstämplar lagras internt i UTC på servern.

* **Klientkonsolens beteende**: Klientkonsolen visar tidsstämplar med **operatorns tidszon**, som definieras i operatorns inställningar. Som standard motsvarar detta **serverns tidszon**.

* **Webbgränssnittsbeteende**: Webbgränssnittet visar tidsstämplar med **webbläsarens lokala tidszon**. När en användare ändrar webbläsarens eller systemets tidszon uppdateras de datum/tid-värden som visas automatiskt.

* **Arbetsflödesbeteende**: arbetsflöden tolkar lokala tidsstämplar baserat på arbetsflödets konfigurerade tidszon **.** Om inget anges används **serverns tidszon** som standard.

## Exempel

| Gränssnitt | Tidszon används | Exempelvisning |
|------------|----------------|-----------------|
| Klientkonsol | Operatörens (standard = server) | `2025-10-20 14:00:00` |
| Webbgränssnitt | Webbläsarens lokala tidszon | `2025-10-20 21:00:00` (för webbläsare i UTC +7) |

I det här exemplet refererar båda gränssnitten till samma underliggande UTC-tidsstämpel, men varje gränssnitt återger den med en annan tidszon.

## Effekt

Skillnader i visningstider kan visas i:

* Profil eller datafält som innehåller `datetime` värden
* Leveransloggar eller kontaktdatum
* Körning av arbetsflöde och import av tidsstämplar

De underliggande data förblir identiska. Skillnaden är bara i **återgivning**.

>[!NOTE]
>
>Om användare från flera regioner samarbetar i samma instans kan tydliga skillnader mellan tidsstämplar för webbgränssnitt och konsol uppstå.

## Rekommendationer

Om du vill justera visningsvärden mot gränssnitt kan du:

* Ändra **webbläsarens tidszon** så att den matchar **operatorn eller serverns tidszon**.
* När du exporterar data (exporterar med UTC) måste du säkerställa en konsekvent konvertering i rapporteringsverktygen.
* När du utformar arbetsflöden anger du uttryckligen **arbetsflödets tidszon** i aktivitetsegenskaperna för förutsägbar schemaläggning och importbeteende.
* Kommunicera till företagsanvändare om att tidsstämpelskillnader mellan webbgränssnitt och klientkonsolvyer är **normala och förväntade**.
