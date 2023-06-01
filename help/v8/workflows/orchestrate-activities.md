---
audience: end-user
title: Skapa arbetsflöden med Adobe Campaign Web
description: Lär dig skapa arbetsflöden med Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 422f2d2cbef424a95540f359c4a5e978eace6c9f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# Organisera aktiviteter {#orchestrate}

En gång har du [skapade ett arbetsflöde](create-workflow.md), oavsett om det gäller arbetsflödesmenyn eller en kampanj, kan du börja organisera de olika uppgifter som ska utföras. För att göra detta finns en visuell arbetsyta som gör att du kan skapa ett arbetsflödesdiagram. I det här diagrammet kan du lägga till olika aktiviteter och koppla dem i en sekventiell ordning.

I det här skedet av konfigurationen visas diagrammet med en startikon som representerar början av arbetsflödet. Om du vill lägga till den första aktiviteten klickar du på plusknappen (+) som är ansluten till startikonen.

En lista över aktiviteter som kan läggas till i diagrammet visas. Vilka aktiviteter som är tillgängliga beror på var du befinner dig i arbetsflödesdiagrammet. När du till exempel lägger till din första aktivitet kan du starta arbetsflödet genom att rikta in dig på en målgrupp, dela arbetsflödessökvägen eller ange en vänteaktivitet för att fördröja arbetsflödets körning. Efter en målgruppsaktivitet kan du däremot förfina målgruppen med målinriktade aktiviteter, skicka en leverans till målgruppen med kanalaktiviteter eller ordna arbetsflödet med flödeskontrollaktiviteter.

![](assets/workflow-start.png)

När en aktivitet har lagts till i diagrammet visas en höger ruta där du kan konfigurera den nyligen tillagda aktiviteten med specifika inställningar. Detaljerad information om hur du konfigurerar varje aktivitet finns i [det här avsnittet](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Upprepa den här processen och lägg till så många aktiviteter som du vill, beroende på vilka uppgifter du vill att arbetsflödet ska utföra. Observera att du även kan infoga en ny aktivitet mellan två aktiviteter. Det gör du genom att klicka på plusknappen (+) för övergången mellan aktiviteterna, markera önskad aktivitet och konfigurera den i den högra rutan.

Om du vill ta bort en aktivitet markerar du den på arbetsytan och klickar på ikonen Ta bort i aktivitetsegenskaperna.

>[!TIP]
>
>Du kan anpassa namnet på övergångarna mellan varje aktivitet. Det gör du genom att markera övergången och ändra dess etikett i den högra rutan.

När du är klar med arbetsflödet lägger du till slutaktiviteten i slutet av diagrammet. Med den här aktiviteten kan du markera slutet av ett arbetsflöde visuellt och inte ha någon funktionell inverkan.

När du har utformat arbetsflödesdiagrammet kan du köra arbetsflödet och spåra förloppet för dess olika uppgifter. [Lär dig hur du startar ett arbetsflöde och övervakar hur det körs](start-monitor-workflows.md)
