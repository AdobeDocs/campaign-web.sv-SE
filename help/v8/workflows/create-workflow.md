---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa ett arbetsflöde med Adobe Campaign Web
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 1%

---


# Skapa arbetsflödet {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista över arbetsflöden i kampanjen"
>abstract="Fliken **Arbetsflöden** visar alla arbetsflöden som är länkade till den aktuella kampanjen. Klicka på namnet på ett arbetsflöde för att redigera det. Använd knappen **Skapa arbetsflöde** för att lägga till ett nytt arbetsflöde för kampanjen."

Du kan skapa fristående arbetsflöden eller arbetsflöden inom en kampanj. Det första steget är att välja en mall och definiera dess allmänna egenskaper. Sedan kan du konfigurera ytterligare inställningar efter behov.

Gör så här:

1. Bläddra till menyn **Arbetsflöden** om du vill skapa ett **fristående arbetsflöde**. Om du vill skapa ett **kampanjarbetsflöde** går du till menyn **Kampanjer** och öppnar kampanjen som du vill skapa ett nytt arbetsflöde för.

1. Klicka på knappen **[!UICONTROL Create workflow]** i skärmens övre högra hörn.

   ![](assets/workflow-create.png){zoomable="yes"}

1. I arbetsflödets dialogruta **Egenskaper** väljer du den mall som ska användas för att skapa arbetsflödet (du kan också använda den inbyggda standardmallen). [Läs mer om arbetsflödesmallar](#workflow-templates).

1. Ange en etikett för arbetsflödet. Dessutom rekommenderar vi att du lägger till en beskrivning i arbetsflödet i det dedikerade fältet i avsnittet **[!UICONTROL Additional options]** på skärmen.

1. Expandera avsnittet **[!UICONTROL Additional options]** om du vill konfigurera fler inställningar för arbetsflödet. Lär dig konfigurera arbetsflödesegenskaperna på [den här sidan](workflow-settings.md#properties)

   ![](assets/workflow-additional-options.png){zoomable="yes"}

1. Klicka på knappen **[!UICONTROL Create workflow]** för att bekräfta att arbetsflödet har skapats.

Arbetsflödet har nu skapats och är tillgängligt i listan över arbetsflöden. Nu kan du komma åt den visuella arbetsytan och börja lägga till, konfigurera och organisera de uppgifter som ska utföras. [Lär dig att samordna arbetsflödesaktiviteter](orchestrate-activities.md).

## Arbeta med arbetsflödesmallar {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Arbetsflödesmallar"
>abstract="Arbetsflödesmallar innehåller förkonfigurerade inställningar och aktiviteter som kan återanvändas för att skapa nya arbetsflöden."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="Egenskaper för arbetsflöde"
>abstract="Arbetsflödesmallar innehåller förkonfigurerade inställningar och aktiviteter som kan återanvändas för att skapa nya arbetsflöden. På den här skärmen anger du arbetsflödesmallens etikett och konfigurerar dess inställningar, t.ex. dess interna namn, mapp och körningsmappar, tidszon och övervakargrupp."

Arbetsflödesmallar innehåller förkonfigurerade inställningar och aktiviteter som kan återanvändas för att skapa nya arbetsflöden. Du kan välja arbetsflödets mall bland arbetsflödesegenskaperna när du skapar ett arbetsflöde. En tom mall anges som standard.

Du kan skapa en mall från ett befintligt arbetsflöde eller skapa en ny mall från början. Båda metoderna beskrivs nedan.

>[!BEGINTABS]

>[!TAB Skapa en mall från ett befintligt arbetsflöde]

Så här skapar du en arbetsflödesmall från ett befintligt arbetsflöde:

1. Öppna menyn **Arbetsflöden** och bläddra till arbetsflödet som du vill spara som en mall.
1. Klicka på de tre punkterna till höger om arbetsflödets namn och välj **Kopiera som mall**.

   ![](assets/wf-copy-as-template.png){zoomable="yes"}

1. Bekräfta att mallen har skapats i popup-fönstret.
1. Kontrollera, lägg till och konfigurera aktiviteter efter behov på arbetsytan i arbetsflödesmallen.
1. Bläddra till inställningarna från knappen **Inställningar** för att ändra namnet på arbetsflödesmallen och ange en beskrivning.
1. Markera mallens **mapp** och **körningsmapp**. Mappen är den plats där arbetsflödesmallen sparas. Körningsmappen är den mapp där arbetsflöden som skapats utifrån den här mallen sparas.

   ![](assets/wf-settings-template.png){zoomable="yes"}

   De andra egenskaperna är vanliga i arbetsflöden. Läs mer på [den här sidan](workflow-settings.md#properties)

1. Spara ändringarna.

Arbetsflödesmallen är nu tillgänglig i malllistan. Du kan skapa ett arbetsflöde baserat på den här mallen. Det här arbetsflödet förkonfigureras med inställningarna och aktiviteterna som är definierade i mallen.


>[!TAB Skapa en mall från grunden]


Så här skapar du en arbetsflödesmall från grunden:

1. Öppna menyn **Arbetsflöden** och gå till fliken **Mallar**. Du kan se en lista över tillgängliga arbetsflödesmallar.
1. Klicka på knappen **[!UICONTROL Create template]** i skärmens övre högra hörn.
1. Ange etiketten och öppna de ytterligare alternativen för att ange en beskrivning av arbetsflödesmallen.
1. Välj mapp och körningsmapp för mallen. Mappen är den plats där arbetsflödesmallen sparas. Körningsmappen är den mapp där arbetsflöden som skapats utifrån den här mallen sparas.

   ![](assets/new-wf-template.png){zoomable="yes"}

   De andra egenskaperna är vanliga i arbetsflöden. Läs mer på [den här sidan](workflow-settings.md#properties)

1. Klicka på knappen **Skapa** för att bekräfta inställningarna.
1. Lägg till och konfigurera aktiviteterna efter behov på arbetsytan i arbetsflödesmallen.

   ![](assets/wf-template-activities.png){zoomable="yes"}

1. Spara ändringarna.

Arbetsflödesmallen är nu tillgänglig i malllistan. Du kan skapa ett arbetsflöde baserat på den här mallen. Det här arbetsflödet förkonfigureras med inställningarna och aktiviteterna som är definierade i mallen.

>[!ENDTABS]
