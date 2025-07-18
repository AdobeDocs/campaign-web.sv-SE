---
title: Varumärke
description: Upptäck hur ni konfigurerar ert varumärke
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 2b4a818c819ae598d5555c1a2d64447b0793b5b8
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 27%

---

# Konfigurera varumärken {#branding-configure}

>[!IMPORTANT]
>
>Varumärken kan inte skapas eller ändras av slutanvändare: dessa åtgärder måste utföras av den tekniska administratören för Adobe Campaign. Kontakta Adobes kundtjänst om du har frågor.

I Adobe Campaign V8 finns varumärkena på menyn **[!UICONTROL Administration > Platform > Branding]**.

En **[!UICONTROL Brand]** definieras av följande egenskaper:

* En **[!UICONTROL Identity]** som definierar och personaliserar ert varumärke. Det här avsnittet innehåller följande fält:

   * **[!UICONTROL Label]** visas i gränssnittet
   * **[!UICONTROL ID]**
   * **[!UICONTROL Brand name]**
   * **[!UICONTROL Website URL]** och **[!UICONTROL Website label]** av varumärket
   * **[!UICONTROL Brand logo]**

  ![](assets/branding_1.png)

* **[!UICONTROL Header parameters of sent emails]** som anpassar vad mottagarna av dina kampanjer kommer att se. Det här avsnittet innehåller följande fält:

   * **[!UICONTROL Sender (email address)]** med varumärkets e-postadress.
   * **[!UICONTROL Sender (name)]** med varumärkets namn.
   * **[!UICONTROL Reply to (email address)]** med den e-postadress som kunden kan svara på.
   * **[!UICONTROL Reply to (name)]** med varumärkets namn.
   * **[!UICONTROL Error (email address)]** med den e-postadress som ska användas om ett fel uppstår.

  >[!IMPORTANT]
  >
  >Om avsändarens namn och e-postadress inte har ändrats i det e-postmeddelande som skapas från mallen ska du kontrollera mallens avancerade inställningar när du har uppdaterat rubrikparametrarna för e-postmeddelandena.

  ![](assets/branding_2.png)

* **[!UICONTROL Brand configs]** definierar de servrar som används för att spåra även för åtkomst till landningssidor. Det här avsnittet innehåller följande fält:

   * **[!UICONTROL Brand subdomain]** refererar till den angivna URL-adressen för underdomänen som är specifik för det här varumärket och som har begärts för delegering från Adobe.

  Observera att konfigurationen för spårning, spegling och programservrar lagras i separata externa konton som är kopplade till routning. De här inställningarna används under etableringen och bör inte ändras. Om du vill visa URL:er går du till fliken **[!UICONTROL Branding prefixes]** från ditt externa konto.

  ![](assets/branding_3.png)

* Med menyn **[!UICONTROL Tracking URL configs]** kan du förbättra URL-spårningen genom att definiera ytterligare parametrar för integrering med webbanalysverktyg som Adobe Analytics och Google Analytics.

  Använd menyn **[!UICONTROL Additional URL Parameters]** om du vill skapa ytterligare parametrar som nyckelvärdepar tillsammans med deras tillämplighetsvillkor. Varje parameternamn måste vara unikt och inte tomt, och varje parametervärde måste vara icke-tomt. Tillämplighetsvillkoret kan vara tomt, men inget av dessa värden kan innehålla JST-taggar.

  De här parametrarna kommer att användas för spårade URL:er som matchar alla domännamn som anges i **[!UICONTROL List of Domain Names]**, som kan innehålla reguljära uttryck.
