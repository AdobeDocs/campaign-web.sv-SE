---
title: Migrering av tekniska användare till Adobe Developer Console
description: Lär dig hur du migrerar hantering av användaråtkomst från Campaign Standard till Campaign v8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 1%

---

# Hantering av användaråtkomst från Campaign Standard till Campaign v8 {#user-management-acs}

Med både Adobe Campaign Standard och Adobe Campaign v8 kan användare definiera och hantera behörigheter för olika användare/operatorer. Dessa behörigheter består av specifika rättigheter som ger användarna tillgång till olika funktioner i produkten. De två produkterna har dock distinkta metoder och implementeringar för att hantera användaråtkomst.

Följande koncept används i Adobe Campaign Standard och Campaign v8 för att hantera användaråtkomst:

| Campaign Standard | Campaign v8 |
|---------|----------|
| Användare | Operatör |
| Roll | Namngiven höger |
| Säkerhetsgrupp | Operatorgrupp |
| Organisationsenhet | Mappbehörighet |

## Migreringsmetod från säkerhetsgrupp till operatörsgrupp

>[!IMPORTANT]
>
>Funktionerna för dessa roller/namngivna rättigheter kan variera i implementeringen, vilket kan ge upphov till behörighetsproblem (t.ex. upphöjd behörighet eller funktionsstörningar). Vi rekommenderar användare att granska mappningarna efter övergången för att säkerställa korrekt åtkomstkontroll. [Läs mer om behörigheter](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

Tabellen nedan visar migreringsmetoden för användarrollgrupper vid övergång från Adobe Campaign Standard till Campaign v8. I Campaign Standard används en **säkerhetsgrupp**, som kallas **Operator group** i Campaign v8, för att tilldela en uppsättning roller till en användare. Vissa säkerhetsgrupper/operatorgrupper är tillgängliga när de är klara, men användare kan skapa nya grupper eller ändra befintliga grupper om det behövs.

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologi**  | Säkerhetsgrupp | Operatorgrupp |

I både Adobe Campaign Standard och Campaign v8 mappas **säkerhetsgrupperna** och **Operator-grupperna** till Produktprofiler i Admin Console. Om du vill tilldela en **säkerhetsgrupp** eller **operatörsgrupp** till en användare kan du länka motsvarande **produktprofil** i Admin Console. Associationen synkroniseras när användaren loggar in. [Läs mer om produktprofilen](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Campaign Standard Security Group** | **Kampanj v8, operatörsgrupp** |
|----------|---------|
| Administratörer | Administratörer |
| Leveransansvariga | Administratörer |
| Arbetsflödesansvariga | Arbetsflödesansvariga  |

## Migreringsmetod från användarroller till namngivna behörigheter

>[!IMPORTANT]
>
>Vid migrering från Adobe Campaign Standard till Campaign v8 får användare med rollen **Datamodell** men inte **Administration** automatiskt åtkomst till **Administration**, eftersom schemaskapandet i Campaign v8 kräver administrationsbehörighet. Du kan förhindra detta genom att ta bort deras **datamodell**-roll före migreringen.

I Adobe Campaign Standard kallas termen **användarroll** för **namngiven rättighet** i Campaign v8. Tabellen nedan visar den terminologi som används för **Namngivna rättigheter** i Campaign v8 och som motsvarar **Användarroller** i Campaign Standard.

| **Campaign Standard användarroll** | **Kampanj v8 - namngiven höger** | **Beskrivning**  |
|----------|---------|---------|
| Administration | Administration | Användare med administratörsbehörighet har fullständig åtkomst till instansen. |
| Datamodell  | Administration | Rätt att köra publikationer och skapa anpassade resurser. Funktioner för att skapa scheman som är tillgängliga för administratören i Campaign v8.  |
| Leverans  | Administration  | Rätt att godkänna tidigare analyserade leveranser.  |
| Exportera | Exportera | Rätt att exportera data.  |
| Filåtkomst  | Filåtkomst  | Rätt att godkänna tidigare analyserade leveranser.  |
| Allmän import  | Importera  | Rätt till allmän dataimport |
| Förbered leveranser | Förbered leveranser | Rätt att skapa, ändra, förbereda och ta bort leveranser.  |
| SQL Script-körning | SQL Script-körning | Rätt att köra ett SQL-kommando direkt i databasen. |
| Starta leveranser  | Starta leveranser  | Rätt att godkänna tidigare analyserade leveranser.  |
| Körning av systemkommando | Programkörning | Rätt att köra systemkommandon på servern. |
| Arbetsflöde | Arbetsflöde | Rätt att hantera körningen av arbetsflöden: start, stopp, paus osv. |

## Migreringsmetod från organisationsenhet

>[!IMPORTANT]
>
>Organisationsenheter i Adobe Campaign Standard utan **Alla (alla)** som direkt eller indirekt överordnad migreras inte till Campaign v8.
></br>
>Användare i flera säkerhetsgrupper tilldelas organisationsenheten i den högsta säkerhetsgruppen. Om flera grupper har parallella enheter på den översta nivån väljer systemet organisationsenheten för användaren i Campaign Standard och användaren har bara åtkomst till den valda organisationsenheten och dess underordnade enheter. I Campaign v8 efter migreringen har användaren åtkomst till **alla tilldelade organisationsenheter och deras underordnade enheter**, vilket kan leda till att behörigheterna eskaleras. Du kan förhindra detta genom att undvika att tilldela användare till säkerhetsgrupper med parallella organisationsenheter. Läs mer om [tilldelning av parallella organisationsenheter](#parallel-assignments).


I Adobe Campaign Standard mappas **organisationsenheten** till den befintliga **mapphierarkimodellen** i Campaign v8 för att behålla en liknande åtkomstkontroll. [Läs mer om mapphantering](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologi**  | Organisationsenhet | Mapp |


### Om enhetstilldelning för parallell organisation {#parallel-assignments}

En parallell tilldelning av organisationsenheter inträffar när en användare har åtkomst till flera enheter (tilldelade via säkerhetsgrupper) som finns i separata grenar i hierarkin utan åtkomst till en gemensam överordnad organisationsenhet. Detta skapar en säkerhetsrisk under migreringen.

Ta till exempel följande hierarki för organisationsenheter:

![Samplingsdiagram för parallell organisationstilldelning](assets/do-not-localize/parallel-org-units-sample.png){width="50%" zoomable="yes"}

Ett uppdrag utan parallella organisationsenheter skulle se ut så här:

![Utan ett parallellt exempeldiagram över organisationsenheter](assets/do-not-localize/without-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

Här har användaren tillgång till organisationsenheterna A, A1 och A2-1, som alla är anslutna under den överordnade organisationsenheten A. Användaren har åtkomst till allt under A.

Följande tilldelning innehåller parallella organisationsenheter:

![Med exempeldiagram för parallell organisationsenhet](assets/do-not-localize/with-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

Användaren har åtkomst till A1-1, A2 och A2-1, som finns i separata grenar utan gemensam tilldelad överordnad.


**Säkerhetskonsekvenser**

* I Campaign Standard väljer systemet en organisationsenhet på den översta nivån (A1-1 eller A2) för användaren och begränsar åtkomsten till endast den enheten och dess underordnade enheter.
* Efter migrering till Campaign V8 får användaren tillgång till resurser i alla tilldelade organisationsenheter och deras barn.

**Upplösning**

Parallell tilldelning av organisationsenheter kan åtgärdas genom att säkerställa att alla organisationsenheter som tilldelats en användare faller under en gemensam, överordnad enhet som också tilldelats användaren.

Nedan beskrivs några sätt att uppnå detta:

1. Ta bort åtkomst till flera grenar: Återkalla åtkomst till flera parallella grenar och se till att all åtkomst är under en enda överordnad.
1. Tilldela en gemensam överordnad: Bevilja åtkomst till en lämplig överordnad organisationsenhet som innehåller alla nödvändiga åtkomstpunkter.
1. Strukturera om hierarkin: Ändra organisationsenhetens struktur för att placera all nödvändig åtkomst under en enskild gren.

I exemplet ovan, där en användare har åtkomst till A1-1, A2 och A2-1, är specifika upplösningssteg:

1. Ta bort åtkomst till flera grenar:

   1. Återkalla åtkomst till A1-1, och endast ge åtkomst till A2 (inklusive A2-1), eller
   1. Återkalla åtkomst till A2 och A2-1, och ge endast åtkomst till A1-1

1. Tilldela en gemensam överordnad:

   1. Bevilja åtkomst till organisationsenhet A, som är den gemensamma överordnade till både A1-1 och A2, eller
   1. Bevilja åtkomst till Alla, som omfattar hela hierarkin

1. Strukturera om hierarkin:

   1. Flytta A1-1 under A2, eller
   1. Flytta A2 och A2-1 under A1-1


## Migreringsstrategi från program

I Campaign v8 representeras **Program** som **Mappar**. Med Campaign v8 kan du skapa mappar och begränsa åtkomsten till dem.

Genom att använda **Grupper** och **Namngivna behörigheter** kan **Operatorer** beviljas åtkomst till specifika **Mappar** i navigeringshierarkin, med möjlighet att tilldela läs-, skriv- och borttagningsbehörigheter. [Läs mer om mapphantering](https://experienceleague.adobe.com/sv/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Eftersom ett **program** behandlas som en **mapp** i Campaign v8 kan åtkomsten hanteras på samma sätt som andra mappar. Efter migreringen kan Campaign Standard-administratörer följa dessa steg:

1. Högerklicka på en mapp i Utforskaren och välj **[!UICONTROL Properties...]**.

1. Navigera till fliken **[!UICONTROL Security]**.

1. Ändra behörigheter för operatörsgruppen enligt den önskade åtkomstmodellen. 

## Produktprofilmappning för åtkomst till REST API:er 

För att få åtkomst till transaktions-API:er från körningsinstansen i Campaign v8 krävs en ny **produktprofil**, utöver produktprofilerna **Administrator** och **Message Center**. Den nya **produktprofilen** läggs till i befintliga eller redan skapade tekniska konton i Campaign Standard.

Efter migreringen bör Campaign Standard-användare granska sina **produktprofilsmappningar** och tilldela lämplig **produktprofil** om de inte vill länka sina **tekniska konton** till **administratörens** produktprofil. För framtida integreringar rekommenderar vi att du använder Campaign v8 **Klient-ID** i **REST-URL** i stället för tidigare Campaign Standard **Klient-ID** .

## Migrering av åtkomst till inbyggda Campaign-resurser för Campaign Standard-operatörer

Operatörer som migreras från Campaign Standard får läsåtkomst till specifika inbyggda resurser i Campaign v8.

## Ej migrerade säkerhetsgrupper och roller {#non-migrated-groups-roles}

Nedan visas en lista över Campaign Standard-roller som inte har övergått:

* Standardreläkonto 

* Message Center Push 

Nedan finns en lista över Campaign Standard säkerhetsgruppsmappningar som inte har överförts.

* Meddelandecenteragenter

* Push-agenter för meddelandecenter

* Adobe Experience Manager programhanterare

* Återförsäljarkonto

>[!NOTE]
>
>Anpassade roller som skapas och tilldelas användare i Adobe Campaign Standard migreras inte till Adobe Campaign v8.
