---
title: Migrering av tekniska användare till Adobe Developer Console
description: Lär dig hur du migrerar hantering av användaråtkomst från Campaign Standard till Campaign V8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: cc1f89fe5a67898e0905bd2823f73aa8b9424164
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 1%

---

# Hantering av användaråtkomst från Campaign Standard till Campaign V8 {#user-management-acs}

Med både Adobe Campaign Standard och Adobe Campaign V8 kan användare definiera och hantera behörigheter för olika användare/operatorer. Dessa behörigheter består av specifika rättigheter som ger användarna tillgång till olika funktioner i produkten. De två produkterna har dock distinkta metoder och implementeringar för att hantera användaråtkomst.

Följande koncept används i Adobe Campaign Standard och Campaign V8 för att hantera användaråtkomst:

| Campaign Standard | Campaign V8 |
|---------|----------|
| Användare | Operatör |
| Roll | Namngiven höger |
| Säkerhetsgrupp | Operatorgrupp |
| Organisationsenhet | Mappbehörighet |

## Migreringsmetod från säkerhetsgrupp till operatörsgrupp

>[!CAUTION]
>
>Funktionerna för dessa roller/namngivna rättigheter kan variera i implementeringen, vilket kan ge upphov till behörighetsproblem (t.ex. upphöjd behörighet eller funktionsstörningar). Vi rekommenderar användare att granska mappningarna efter övergången för att säkerställa korrekt åtkomstkontroll. [Läs mer om behörigheter](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

Tabellen nedan visar migreringsmetoden för användarrollgrupper vid övergång från Adobe Campaign Standard till Campaign V8. I Campaign Standard används en **säkerhetsgrupp**, som kallas **Operator group** i Campaign V8, för att tilldela en uppsättning roller till en användare. Vissa säkerhetsgrupper/operatorgrupper är tillgängliga när de är klara, men användare kan skapa nya grupper eller ändra befintliga grupper om det behövs.

| | **Campaign Standard** | **Kampanj V8** |
|---------|----------|---------|
| **Terminologi**  | Säkerhetsgrupp | Operatorgrupp |

I både Adobe Campaign Standard och Campaign V8 mappas **säkerhetsgrupperna** och **Operator-grupperna** till Produktprofiler i Admin Console. Om du vill tilldela en **säkerhetsgrupp** eller **operatörsgrupp** till en användare kan du länka motsvarande **produktprofil** i Admin Console. Associationen synkroniseras när användaren loggar in. [Läs mer om produktprofilen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Campaign Standard Security Group** | **Kampanj V8, operatörsgrupp** |
|----------|---------|
| Administratörer | Administratörer |
| Leveransansvariga | Administratörer |
| Arbetsflödesansvariga | Arbetsflödesansvariga  |

## Migreringsmetod från användarroller till namngivna behörigheter

>[!CAUTION]
>
>Vid migrering från Adobe Campaign Standard till Campaign V8 får användare med rollen **Datamodell** men inte **Administration** automatiskt åtkomst till **Administration**, eftersom schemaskapandet i Campaign V8 kräver administrationsbehörighet. Du kan förhindra detta genom att ta bort deras **datamodell**-roll före migreringen.

I Adobe Campaign Standard kallas termen **användarroll** för **namngiven rättighet** i kampanj V8. Tabellen nedan visar den terminologi som används för **Namngivna rättigheter** i Campaign V8 och som motsvarar **Användarroller** i Campaign Standard.

| **Campaign Standard användarroll** | **Kampanj V8 med namnet höger** | **Beskrivning**  |
|----------|---------|---------|
| Administration | Administration | Användare med administratörsbehörighet har fullständig åtkomst till instansen. |
| Datamodell  | Administration | Rätt att köra publikationer och skapa anpassade resurser. Funktioner för att skapa scheman som är tillgängliga för administratören i kampanj V8.  |
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

### Observera varningar

Organisationsenheter i Adobe Campaign Standard utan **Alla (alla)** som direkt eller indirekt överordnad migreras inte till Campaign V8.

Användare i flera säkerhetsgrupper tilldelas organisationsenheten i den högsta säkerhetsgruppen. Om flera grupper har parallella enheter på den översta nivån väljer systemet organisationsenheten för användaren i Campaign Standard och användaren har bara åtkomst till den valda organisationsenheten och dess underordnade enheter. I Campaign v8 efter migreringen har användaren åtkomst till **alla tilldelade organisationsenheter och deras underordnade enheter**, vilket kan leda till att behörigheterna eskaleras. Du kan förhindra detta genom att undvika att tilldela användare till säkerhetsgrupper med parallella organisationsenheter. <!--Know more about parallel organizational unit assignment here (link to ' Parallel Organizational Unit Assignment' section)-->

### Organisationsenheter och mapphantering

I Adobe Campaign Standard mappas **organisationsenheten** till den befintliga **mapphierarkimodellen** i Campaign V8 för att behålla en liknande åtkomstkontroll. [Läs mer om mapphantering](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Kampanj V8** |
|---------|----------|---------|
| **Terminologi**  | Organisationsenhet | Mapp |

## Migreringsstrategi från program

I Campaign V8 representeras **Program** som **Mappar**. Med Campaign V8 kan du skapa mappar och begränsa åtkomsten till dem.

Genom att använda **Grupper** och **Namngivna behörigheter** kan **Operatorer** beviljas åtkomst till specifika **Mappar** i navigeringshierarkin, med möjlighet att tilldela läs-, skriv- och borttagningsbehörigheter. [Läs mer om mapphantering](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Eftersom ett **program** behandlas som en **mapp** i Campaign V8 kan åtkomsten hanteras på samma sätt som andra mappar. Efter migreringen kan Campaign Standard-administratörer följa dessa steg:

1. Högerklicka på en mapp i Utforskaren och välj **[!UICONTROL Properties...]**.

1. Navigera till fliken **[!UICONTROL Security]**.

1. Ändra behörigheter för operatörsgruppen enligt den önskade åtkomstmodellen. 

## Produktprofilmappning för åtkomst till REST API:er 

För att få åtkomst till transaktions-API:er från körningsinstansen i Campaign V8 krävs en ny **produktprofil**, utöver produktprofilerna **Administrator** och **Message Center**. Den nya **produktprofilen** läggs till i befintliga eller redan skapade tekniska konton i Campaign Standard.

Efter migreringen bör Campaign Standard-användare granska sina **produktprofilsmappningar** och tilldela lämplig **produktprofil** om de inte vill länka sina **tekniska konton** till **administratörens** produktprofil. För framtida integreringar rekommenderar vi att du använder Campaign V8 **Klient-ID** i **REST-URL** i stället för tidigare Campaign Standard **Klient-ID** .

## Migrering av åtkomst till inbyggda Campaign-resurser för Campaign Standard-operatörer

Operatörer som migreras från Campaign Standard får läsåtkomst till specifika inbyggda resurser i Campaign V8.

## Ej migrerade säkerhetsgrupper och roller {#non-migrated-groups-roles}

Nedan visas en lista över Campaign Standard-roller som inte har övergått:

* Standardreläkonto 

* Message Center Push 

Nedan finns en lista över Campaign Standard säkerhetsgruppsmappningar som inte har överförts.

* Meddelandecenteragenter

* Push-agenter för meddelandecenter

* Adobe Experience Manager programhanterare

* Återförsäljarkonto

Observera att anpassade roller som skapas och tilldelas användare i Adobe Campaign Standard inte migreras till Campaign V8.
