---
audience: end-user
title: Använda en svällningsgrupp
description: Lär dig hur du använder en svällningsgrupp för leverans i gränssnittet för Campaign-webben
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Använda en svällningsgrupp {#trap-group}

En **[!UICONTROL trap group]** (kallas även **[!UICONTROL Seed list]**) används för att inkludera specifika adresser i leveranser för att övervaka och verifiera distributionsprocessen genom att rikta profiler som inte matchar de definierade målvillkoren. På så sätt kan mottagare som befinner sig utanför leveransområdet ta emot leveransen, precis som andra målmottagare.

En **[!UICONTROL trap group]** är en grupp av **[!UICONTROL seed addresses]** med namnet **[!UICONTROL Test profile]** i webbanvändargränssnittet för Campaign.

## Varför använda en svällningsgrupp {#why-trap-group}

Du kan använda en **[!UICONTROL trap group]**:

1. **Som ett bevis**: Alla medlemmar i **[!UICONTROL trap group]** får leveransen som om de vore en del av målgruppen.

1. **För att skydda din e-postlista**: Genom att ta emot det som målgruppen kommer att få, kommer varje **[!UICONTROL Test profile]** i **[!UICONTROL Trap group]** att uppmärksammas om e-postlistan används av en tredje part.

>[!NOTE]
>
>Förutom att [skicka korrektur när leveransen ](../email/create-email.md#preview-test) skapas och från [kontrollgruppen](control-group.md) är det bra att lägga till en svällningsgrupp för att testa målgruppen.

## Om svällningsgrupper {#about-trap-group}

Testprofiler exkluderas automatiskt från rapporter om följande leveransstatistik: **Klicka**, **Öppnar**, **Avbeställ**. Rapporterna fokuserar bara på den verkliga publiken.

För en e-postleverans krävs bara e-postadressen för **[!UICONTROL Trap group]**. Personaliseringen av andra fält fylls i slumpmässigt av Campaign.

## Lägg till en svällningsgrupp i en leverans {#trap-group-in-delivery}

Om du vill konfigurera **[!UICONTROL Trap group]** går du till **[!UICONTROL Audience]**-inställningarna för leveransen. Det finns två alternativ:

* [Välj testprofiler](#select-test-profiles)
* [Skapa villkor](#create-condition)

[Gränssnitt för svällningsgruppinställningar, bild](assets/trap-group.png){zoomable="yes"}

### Välj testprofiler {#select-test-profiles}

När du väljer **Välj testprofiler** använder du knappen **Lägg till testprofiler** enligt nedan:

[Knappen Lägg till testprofil, bild](assets/trap-no-test-profile.png){zoomable="yes"}

När du klickar på knappen har du tillgång till testprofilerna som ska läggas till i **[!UICONTROL trap group]**. Markera de som du vill använda.

Du kan också skapa nya testprofiler. [Läs mer](#create-seed)

[Välj testprofilgränssnitt, bild](assets/trap-select-test-profiles.png){zoomable="yes"}

När du har bekräftat testprofilerna kontrollerar du att rätt nummer visas under **[!UICONTROL Trap group]**.

[Bekräftelse av svällningsgrupp, bild](assets/trap-check.png){zoomable="yes"}

### Skapa villkor {#create-condition}

Med alternativet **[!UICONTROL Create condition]** skapar du en fråga för att definiera de testprofiler som du vill använda:

[Skapa villkorsgränssnitt, bild](assets/trap-create-condition.png){zoomable="yes"}

Din fråga visas under **[!UICONTROL Trap group]**.

[Visning av svällningsgruppfråga, bild](assets/trap-custom.png){zoomable="yes"}

## Skapa en ny testprofil {#create-seed}

Du kan skapa en ny **[!UICONTROL test profile]** från mappen **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**.

[Skapa testprofilnavigering, bild](assets/trap-create.png){zoomable="yes"}

Konfigurera alla inställningar för din **[!UICONTROL test profile]** på samma sätt som för alla profiler:

[Testa profilens konfiguration, bild](assets/trap-create-contact.png){zoomable="yes"}