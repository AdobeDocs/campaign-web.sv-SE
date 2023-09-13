---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa ett arbetsflöde med Adobe Campaign Web
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 0bdd138bab21fae7af0b2bdd636e719780fbc56d
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 1%

---


# Skapa arbetsflödet {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Egenskaper för arbetsflöde"
>abstract="På den här skärmen väljer du den mall som ska användas för att skapa arbetsflödet och anger en etikett. Expandera sektionen Ytterligare OPTIONS om du vill konfigurera fler inställningar, till exempel arbetsflödets interna namn, dess mapp, tidszon och övervakningsgrupp. Vi rekommenderar starkt att du väljer en grupp för ansvariga så att de får ett meddelande om ett fel inträffar."

Du kan skapa fristående arbetsflöden eller arbetsflöden inom en kampanj. Det första steget är att välja en mall och definiera dess allmänna egenskaper. Sedan kan du konfigurera ytterligare inställningar efter behov.

Gör så här:

1. Skapa en **Fristående arbetsflöde**, bläddra till **Arbetsladdar** -menyn.

   Skapa en **Arbetsflöde för kampanj**, bläddra till **Kampanjer** och öppna kampanjen som du vill skapa ett nytt arbetsflöde för.

1. Klicka på **[!UICONTROL Create workflow]** i skärmens övre högra hörn.

   ![](assets/workflow-create.png)

1. I arbetsflödet **Egenskaper** väljer du den mall som ska användas för att skapa arbetsflödet (du kan också använda den inbyggda standardmallen). Läs mer om mallar i [avsnittet nedan](#work-with-workflow-templates-workflow-templates).

1. Ange en etikett för arbetsflödet. Vi rekommenderar dessutom att du lägger till en beskrivning i arbetsflödet i det dedikerade fältet i **[!UICONTROL Additional options]** på skärmen.

1. Expandera **[!UICONTROL Additional options]** för att konfigurera fler inställningar för arbetsflödet. Lär dig hur du konfigurerar arbetsflödesegenskaperna i [den här sidan](workflow-settings.md#properties)

   ![](assets/workflow-additional-options.png)

1. Klicka på **[!UICONTROL Create workflow]** för att bekräfta att arbetsflödet har skapats.

Arbetsflödet har nu skapats och är tillgängligt i listan över arbetsflöden. Nu kan du komma åt den visuella arbetsytan och börja lägga till, konfigurera och organisera de uppgifter som ska utföras. Lär dig att samordna arbetsflödesaktiviteter i [den här sidan](orchestrate-activities.md).

## Arbeta med arbetsflödesmallar {#workflow-templates}

Arbetsflödesmallar innehåller förkonfigurerade inställningar och aktiviteter som kan återanvändas för att skapa nya arbetsflöden. Du kan välja arbetsflödets mall bland arbetsflödesegenskaperna när du skapar ett arbetsflöde. En tom mall anges som standard.

Du kan skapa en mall från ett befintligt arbetsflöde eller skapa en ny mall från början. Båda metoderna beskrivs nedan.


>[!BEGINTABS]

>[!TAB Skapa en mall från ett befintligt arbetsflöde]

Så här skapar du en arbetsflödesmall från ett befintligt arbetsflöde:

1. Öppna i **Arbetsflöden** och bläddra till arbetsflödet som du vill spara som en mall.
1. Klicka på de tre punkterna till höger om arbetsflödets namn och välj **Kopiera som mall**.

   ![](assets/wf-copy-as-template.png)

1. Bekräfta att mallen har skapats i popup-fönstret.
1. Kontrollera, lägg till och konfigurera aktiviteter efter behov på arbetsytan i arbetsflödesmallen.
1. Bläddra till inställningarna för att ändra namnet på arbetsflödesmallen och ange en beskrivning.
1. Välj mapp och körningsmapp för mallen. Mappen är den plats där arbetsflödesmallen sparas. Körningsmappen är den mapp där arbetsflöden som skapats utifrån den här mallen sparas.

   ![](assets/wf-settings-template.png)

   De andra egenskaperna är vanliga i arbetsflöden. Läs mer i [den här sidan](workflow-settings.md#properties)

1. Spara ändringarna.

Arbetsflödesmallen är nu tillgänglig i malllistan. Du kan skapa ett arbetsflöde baserat på den här mallen. Det här arbetsflödet förkonfigureras med inställningarna och aktiviteterna som är definierade i mallen.


>[!TAB Skapa en mall från grunden]


Så här skapar du en arbetsflödesmall från grunden:

1. Öppna i **Arbetsflöden** och bläddra till **Mallar** -fliken. Du kan se en lista över tillgängliga arbetsflödesmallar.
1. Klicka på **[!UICONTROL Create template]** i skärmens övre högra hörn.
1. Ange etiketten och öppna de ytterligare alternativen för att ange en beskrivning av arbetsflödesmallen.
1. Välj mapp och körningsmapp för mallen. Mappen är den plats där arbetsflödesmallen sparas. Körningsmappen är den mapp där arbetsflöden som skapats utifrån den här mallen sparas.

   ![](assets/new-wf-template.png)

   De andra egenskaperna är vanliga i arbetsflöden. Läs mer i [den här sidan](workflow-settings.md#properties)

1. Klicka på **Skapa** för att bekräfta inställningarna.
1. Lägg till och konfigurera aktiviteterna efter behov på arbetsytan i arbetsflödesmallen.

   ![](assets/wf-template-activities.png)

1. Spara ändringarna.

Arbetsflödesmallen är nu tillgänglig i malllistan. Du kan skapa ett arbetsflöde baserat på den här mallen. Det här arbetsflödet förkonfigureras med inställningarna och aktiviteterna som är definierade i mallen.

>[!ENDTABS]
