---
audience: end-user
title: Använda en svällningsgrupp
hide: true
hidefromtoc: true
description: Lär dig hur du använder en svällningsgrupp för leverans i gränssnittet för Campaign-webben
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Använd en **[!UICONTROL trap group]** {#trap-group}

En **[!UICONTROL trap group]** (kallas även **[!UICONTROL Seed list]**) används för att inkludera specifika adresser i leveranser för att övervaka och verifiera distributionsprocessen genom att rikta profiler som inte matchar de definierade målvillkoren. På så sätt kan mottagare som ligger utanför leveransomfånget ta emot leveransen, precis som andra målmottagare gör.
En **[!UICONTROL trap group]** är en grupp av **[!UICONTROL seed addresses]** med namnet **[!UICONTROL Test profile]** i AC-webbgränssnittet.

## Varför använda **[!UICONTROL Trap group]**

Du kan använda **[!UICONTROL trap group]**:

1. **Som ett bevis**: alla medlemmar i **[!UICONTROL Trap group]** får leveransen som om de vore en del av målgruppen.


1. **För att skydda din e-postlista**: genom att ta emot det som målgruppen kommer att få, kommer varje **[!UICONTROL test profile]** i **[!UICONTROL Trap group]** att uppmärksammas om e-postlistan används av en tredje part.

>[!NOTE]
>
>Svällningsgruppen skiljer sig från [att skicka korrektur när leveransen ](../email/create-email.md#preview-test) skapas och från [kontrollgruppen](control-group.md).


## Om **[!UICONTROL Trap group]**

Testprofiler exkluderas automatiskt från rapporter om följande leveransstatistik: **Klicka**, **Öppnar**, **Avbeställ**. Rapporterna handlar bara om den verkliga publiken.

För en e-postleverans behövs bara e-postadressen för **[!UICONTROL Trap group]**. Anpassningen av andra fält fylls i slumpmässigt av Campaign.

## Så här konfigurerar du en **[!UICONTROL Trap group]** i leveransen

Om du vill konfigurera **[!UICONTROL Trap group]** går du till **[!UICONTROL Audience]**-inställningarna för leveransen. Du har två alternativ:
- [Välj testprofiler](#select-test-profile)
- [Skapa villkor](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Välj testprofiler {#select-test-profiles}

När du väljer Välj testprofiler får du fönstret nedan där du är inbjuden till **[!UICONTROL Add test profile(s)]**:

![](assets/trap-no-test-profile.png){zoomable="yes"}

När du klickar på knappen får du tillgång till de testprofiler du kan lägga till **[!UICONTROL trap group]**. Markera de som du vill använda.
Du kan skapa nya testprofiler. [Läs mer](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

När du bekräftar testprofilerna kontrollerar du att du har rätt nummer under **[!UICONTROL Trap group]**.

![](assets/trap-check.png){zoomable="yes"}

### Skapa villkor {#create-condition}

Med alternativet **[!UICONTROL Create condition]** får du ett nytt fönster där du kan anpassa en fråga för att definiera de testprofiler som du vill använda:

![](assets/trap-create-condition.png){zoomable="yes"}

Din fråga visas under **[!UICONTROL Trap group]**.

![](assets/trap-custom.png){zoomable="yes"}

## Så här skapar du en ny **[!UICONTROL Test profile]** {#create-seed}

Du kan skapa en ny **[!UICONTROL test profile]** i **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**

![](assets/trap-create.png){zoomable="yes"}

Du kan slutföra all information om din **[!UICONTROL test profile]** som om det var en målgruppsprofil:

![](assets/trap-create-contact.png){zoomable="yes"}