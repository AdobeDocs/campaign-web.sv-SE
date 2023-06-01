---
audience: end-user
title: Versionsinformation för Campaign Web v8
description: Versionsinformation för Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: 8a6d5d0144d3efd5bcf7f6a20fa4d5a6bc13d12d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---


# Versionsinformation {#release-notes}

Den här sidan innehåller alla de senaste funktionerna och förbättringarna för Campaign Web v8.

## Alfaversion{#alpha-release}

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

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Uppdateringar om terminologi{#terminology-updates}

Som befintlig Campaign-användare bör du tänka på att vissa koncept har bytt namn för att passa in i de senaste terminologinställningarna. De här ändringarna gäller bara för Campaign Web-gränssnittet och återspeglas inte i klientkonsolen. De sammanfattas nedan.

* Korrektur är nu **Testa e-post**: om du vill skicka ett korrektur använder du **Testa** i e-postleveransgränssnittet. Målet för korrekturmålet kallas nu **Testprofiler**
* Seed-adresser används nu som **Testprofiler**: skicka testmeddelandet till dirigerade adresser, som är ytterligare och fiktiva mottagare i databasen
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

