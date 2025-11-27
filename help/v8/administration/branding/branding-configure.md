---
title: Varumärke
description: Upptäck hur ni konfigurerar ert varumärke
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 17%

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

  **Exempel:** En spårad URL som `https://www.example.com` blir `https://www.example.com/?age=21&deliveryName=DM101` när de ytterligare parametrarna `age=21` och `deliveryName=DM101` konfigureras för den domänen.

## Konfigurera branding för transaktionsmeddelanden {#branding-transactional-config}

>[!IMPORTANT]
>
>Det här avsnittet gäller endast för Transactional Messaging (Message Center).
>
>Transaktionsfunktioner är tillgängliga i gränssnittet för Campaign Web, men stegen nedan måste utföras i klientkonsolen Campaign v8 (kontrollinstans).

Om du använder Transactional Messaging (Message Center) med branding krävs ytterligare konfigurering.

### Spåra formler för realtidsinstanser

När branding aktiveras på en Real-Time (RT)-kontrollinstans används särskilda spårningsalternativ för att hantera spårningsformler. Dessa formler konfigureras centralt i RT-kontrollinstansen i stället för individuellt i varje instans av RT-körning.

Följande alternativ definierar spårningsformler som används av RT-leveranser:

* **`NmsTracking_RT_ClickFormula`**: anger formeln som används för klickspårning på RT-instanser

* **`NmsTracking_RT_OpenFormula`**: anger formeln som används för att öppna spårning i RT-instanser

Om implementeringen kräver anpassade spårningsformler för transaktionsmeddelanden använder du alternativet nedan:

* **`Branding_RT_ListXtkOptions_toPublish`**: ange XTK-alternativnamnen för dina anpassade formler här (avgränsade med kommatecken). Detta garanterar att RT-leveranser kan använda anpassade spårningsformler.