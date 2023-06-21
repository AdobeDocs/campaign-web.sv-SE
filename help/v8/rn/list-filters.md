---
audience: end-user
title: Nyheter i Campaign Web v8
description: Upptäck nya funktioner i Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha"
source-git-commit: 0a4d4295f8c460298dcc61fcfc78e8cb09fe963e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---


# Nyheter? {#new}

## Alpha 2.0{#alpha-release}

Det nya webbgränssnittet för Campaign är för närvarande bara tillgängligt för **Alfahandledare** med följande funktioner:

**Modern, intuitiv och enhetlig upplevelse**

Campaign new Web UI erbjuder en ny användarupplevelse som är anpassad efter alla Adobe Experience Cloud lösningar och appar. Det erbjuder:

* Tillgång till det nya gränssnittet och dina andra Adobe-lösningar med en enda delad användarsession
* Ny navigeringsupplevelse med alla menyer och mappar tillgängliga från den vänstra listen
* Lösnings- och organisationsväljare från det övre fältet
* Integrering med Enhetligt gränssnitt, med direktåtkomst till communityn, hjälpcentret och supporten

**Nya kraftfulla funktioner och smidiga processer**

* Omdesignat gränssnitt för arbetsyta för att utforma och hantera processer
* Dynamiskt innehåll för att leverera målinriktade och personaliserade upplevelser till er målgrupp
* Inbyggd integrering med Adobe Experience Platform målgrupper
* Mallhantering för arbetsflöden, leveranser, kampanjer och innehåll

Läs mer om det nya användargränssnittet i [den här sidan](../get-started/user-interface.md).

**Skapa, lansera och mät er kampanj**

Använd det nya webbgränssnittet för Campaign för att:

* Designa skräddarsytt e-postinnehåll med e-postdesignern - [Läs mer](../content/edit-content.md)
* Skicka flerkanalskampanjer, inklusive SMS och push-meddelanden.
* Definiera målgrupper med regelbyggaren - [Läs mer](../audience/about-audiences.md)
* Förhandsgranska, testa och skicka e-postmeddelanden - [Läs mer](../monitor/prepare-send.md)
* Övervaka sändning och mätning av resultat med inbyggda rapporter - [Läs mer](../reporting/delivery-reports.md)


## Övergång till Campaign Web UI

Som Campaign-användare har du fortfarande tillgång till klientkonsolen för att skapa och hantera resurser och komponenter i Campaign. Data och inställningar synkroniseras från en miljö till en annan. Läs mer i [det här avsnittet](../get-started/get-started.md#about-campaign-client-consoleac-client).

Dessutom visas alla data och inställningar som redan är tillgängliga i klientkonsolen i gränssnittet för Campaign-webben, från vänster navigering i Utforskaren. Läs mer om Utforskaren i [det här avsnittet](../get-started/user-interface.md#explorer-user-interface-explorer).


## Uppdateringar om terminologi {#terminology-updates}

Som befintlig Campaign-användare bör du tänka på att vissa koncept har bytt namn för att passa in i de senaste terminologinställningarna. De här ändringarna gäller bara för Campaign Web UI och återspeglas inte i klientkonsolen. De sammanfattas nedan.

* Korrektur är nu **Testa e-post**: om du vill skicka ett korrektur använder du **Testa** i e-postleveransgränssnittet. Målet för korrekturmålet kallas nu **Testprofiler**
* Seed-adresser används nu som **Testprofiler**: skicka testmeddelandet till dirigerade adresser, som är ytterligare mottagare i databasen
* Leveransanalysen är nu **färdigställande av leverans**. När du behöver starta analysen klickar du på **Förbered** knapp
* E-postförhandsgranskning är nu tillgänglig via **Simulera innehåll** knapp
* Listor finns nu **Målgrupper**

## Begränsningar{#limitations-alpha}

Begränsningarna nedan gäller denna alfaversion:

* De enda redigerbara objekten är leveranser, kampanjer, arbetsflöden, målgrupper och mallar. De andra är skrivskyddade. Använd filter för att bläddra bland alla.
* Det går inte att spara publikerna för framtida bruk.
* Användargränssnittet Administration är inte tillgängligt.
* Rapporteringsstatistik (som öppnings- och spårningsdata) uppdateras varje timme.
* KPI:er för kontrollpanelen för leverans uppdateras var femte minut. - men färdigställandet av leveransen är i realtid.
* Adobe Experience Cloud Notifications and Unified Help available in the top bar are not integrated.

