---
audience: end-user
title: Använda en svällningsgrupp
hide: true
hidefromtoc: true
description: Lär dig hur du använder en svällningsgrupp för leverans i gränssnittet för Campaign-webben
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Använd en **[!UICONTROL trap group]** {#trap-group}

En **[!UICONTROL trap group]** används för målmottagare som inte matchar de definierade målvillkoren. På så sätt kan mottagare som ligger utanför leveransomfånget ta emot leveransen, precis som andra målmottagare gör.
En **[!UICONTROL trap group]** är en grupp av **[!UICONTROL seed addresses]**.

## Varför använda **[!UICONTROL trap group]**

Du kan använda **[!UICONTROL trap group]**:

1. **Som ett bevis**: alla medlemmar i **[!UICONTROL Trap group]** får leveransen som om de vore en del av målgruppen.


1. **För att skydda din e-postlista**: genom att ta emot det som målgruppen kommer att få, kommer varje **[!UICONTROL seed address]** i **[!UICONTROL Trap group]** att uppmärksammas om e-postlistan används av en tredje part.

## Om **[!UICONTROL Trap group]**

Seed-adresser exkluderas automatiskt från rapporter om följande leveransstatistik: **Klicka**, **Öppnar**, **Avbeställ**. Rapporterna handlar bara om den verkliga publiken.

För en e-postleverans behövs bara e-postadressen för **[!UICONTROL Trap group]**. Anpassningen av andra fält fylls i slumpmässigt av Campaign.

## Så här konfigurerar du en **[!UICONTROL Trap group]** i leveransen

Om du vill konfigurera **[!UICONTROL Trap group]** går du till **[!UICONTROL Audience]**-inställningarna för leveransen. Du har två alternativ:
- [Välj testprofiler](#select-test-profile)
- [Skapa villkor](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Välj testprofiler {#select-test-profiles}

När du väljer Välj testprofiler får du fönstret nedan där du är inbjuden till **[!UICONTROL Add test profile(s)]**:

![](assets/trap-no-test-profile.png){zoomable="yes"}

När du klickar på knappen får du tillgång till de dirigerade adresser som du kan lägga till **[!UICONTROL trap group]**. Markera de som du vill använda.
Du kan skapa nya dirigerade adresser. [Läs mer](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

När du bekräftar dina svällningsadresser kontrollerar du att du har rätt nummer under **[!UICONTROL Trap group]**.

![](assets/trap-check.png){zoomable="yes"}

### Skapa villkor {#create-condition}

Med alternativet **[!UICONTROL Create condition]** får du ett nytt fönster där du kan anpassa en fråga för att definiera de dirigerade adresser som du vill använda:

![](assets/trap-create-condition.png){zoomable="yes"}

Din fråga visas under **[!UICONTROL Trap group]**.

![](assets/trap-custom.png){zoomable="yes"}

## Så här skapar du en ny **[!UICONTROL seed address]** {#create-seed}

Du kan skapa en ny **[!UICONTROL seed address]** i **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**

![](assets/trap-create.png){zoomable="yes"}

Du kan fylla i all information om din dirigerade medlem som om det vore en målgruppsprofil:

![](assets/trap-create-contact.png){zoomable="yes"}