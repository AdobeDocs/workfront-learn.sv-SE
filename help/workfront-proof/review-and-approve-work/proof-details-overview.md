---
title: Förstå korrekturinformation
description: Mer om detaljerna bakom ett korrektur i [!DNL  Workfront] via sammanfattningspanelen och [!UICONTROL Dokumentinformation] sida.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 0%

---

# Förstå korrekturinformation

## Visa korrekturinformation

Som korrekturansvarig eller ägare kan du fördjupa dig i detaljerna bakom ett korrektur via sammanfattningspanelen och [!UICONTROL Dokumentinformation] sida. Börja med att hitta ditt korrektur i [!UICONTROL Dokument] del av ett projekt, en uppgift eller ett problem.

### Panelen Sammanfattning

På sammanfattningspanelen finns en översikt på hög nivå över korrekturets grundläggande information. Använd ikonen för att expandera panelen när du behöver den och komprimera den när du inte behöver den. Du kan till och med hovra över miniatyrbilden av korrekturet för att öppna eller ladda ned det.

![En bild av [!UICONTROL Dokument] del av ett projekt där ett korrektur är valt och sammanfattningspanelen utökad. Både sammanfattningspanelsikonen och sammanfattningspanelen är markerade.](assets/document-summary.png)

Obs! The [!UICONTROL Godkännanden] i sammanfattningspanelen är **dokument** godkännanden och **är inte** kopplade till den process för granskning och godkännande av intyg som du har lärt dig om i den här kursen. De två processerna är åtskilda i [!DNL Workfront].

### [!UICONTROL Dokumentinformation]

Om du behöver mer information om beviset kan du [!UICONTROL Dokumentinformation] går till korrekturens&quot;sida&quot; i [!DNL Workfront].

![En bild av korrekturets sida i [!DNL  Workfront].](assets/document-details.png)

Observera att möjligheten att se information om korrekturläsningen beror på dina korrekturbehörigheter i [!DNL Workfront].

På korrektursidan kommer du åt dessa avsnitt från den vänstra panelmenyn:

* **Uppdateringar —** Kommentarer som gjorts i korrekturläsaren visas här, med taggen &quot;korrekturkommentar&quot;. Du kan också kommentera filen, precis som du gör kommentarer för en uppgift eller ett projekt (dessa kommentarer visas inte i korrekturläsaren).
* **Godkännanden —** Det här avsnittet är avsett för dokumentgodkännanden, inte för korrektur av godkännanden. De två typerna av godkännanden är separata processer i [!DNL Workfront] och inte länka samman. Om du använder korrekturarbetsflöden för granskningar och godkännanden kommer du inte att använda det här avsnittet.
* **Alla versioner —** Spåra och hantera versionshistoriken för korrekturet. Det kan vara enklare att komma åt informationen i sammanfattningspanelen på [!UICONTROL Dokument] lista.
* **Anpassad Forms -** Anpassade formulär används vid korrektur för att samla in organisationsspecifik information. Den här informationen kan skickas med filen till integrerade dokumentlagringssystem, som [!DNL Workfront] DAM eller [!DNL Adobe’s] AEM. Anpassade formulär har konfigurerats av [!DNL Workfront] systemadministratör eller gruppadministratör. Tala med teamet eller administratörerna för att ta reda på om ni kommer att använda anpassade formulär i korrektur.
* **Korrektur -** Hantera eller ändra arbetsflödet som tilldelats korrekturet. Du kan öppna det här fönstret med [!UICONTROL Korrektur] på korrekturet i [!UICONTROL Dokument] -listan också. Lär dig hur du ändrar arbetsflödet med videon Redigera ett korrekturarbetsflöde.

Vi tittar närmare på två av avsnitten: [!UICONTROL Inställningar för korrekturläsare] och [!UICONTROL Språkkontroll].

### [!UICONTROL Inställningar för korrekturläsare]

Med de här inställningarna kan du styra åtkomsten till själva korrekturet.

![En bild av [!UICONTROL Inställningar för korrekturläsare] från korrektursidan med [!UICONTROL Inställningar för korrekturläsare] markerat alternativ på den vänstra panelmenyn.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Kräv inloggning. Det här korrekturet kan inte delas med gästanvändare] —** Beviset kan bara delas med personer som har en [!DNL Workfront] korrekturläsningslicens.
* **[!UICONTROL Kräv att beslut signeras elektroniskt] —** När du delar ett korrektur måste mottagaren ha korrekturbehörighet i [!DNL Workfront] och gör det möjligt för dem att&quot;signera&quot; beviset elektroniskt genom att ange sitt korrekturlösenord när de fattar ett beslut. (Obs! Språklösenordet skiljer sig från [!DNL Workfront] lösenord. Språklösenordet är inte lätt att komma åt, så de flesta mottagare känner inte till lösenordet.) [!DNL Workfront] rekommenderar att du pratar med [!DNL Workfront] innan du använder den här funktionen.
* **[!UICONTROL Lås korrektur när alla nödvändiga beslut har fattats]—** Detta låser beviset till eventuella ytterligare kommentarer, svar, beslut osv. när varje beslut om beviset har fattats. Då låses hela korrekturversionen, inte bara ett visst steg i korrekturarbetsflödet.
* **[!UICONTROL Tillåt hämtning av originalfilen] —** Korrekturmottagare kan hämta den ursprungliga källfilen för korrekturläsaren (alternativet finns på den högra panelmenyn).
* **[!UICONTROL Tillåt delning av korrektur via offentlig URL eller inbäddningskod] —** Korrekturmottagare kan dela en offentligt tillgänglig korrekturlänk med vem som helst.
* **[!UICONTROL Tillåt prenumerationer på korrektur via offentlig URL eller inbäddningskod] —** Alla som får den offentliga URL:en kan lägga till sig själva till beviset med sin e-postadress och sitt namn (om det inte är en korrekturanvändare) eller sin e-postadress och sitt korrekturlösenord (om det är en korrekturanvändare). (Obs! Språklösenordet är inte detsamma som [!DNL Workfront] lösenord.)

Samma inställningar kan ställas in när korrekturet överförs i [!UICONTROL Korrekturinställningar] , längst ned i överföringsfönstret.

![En bild av [!UICONTROL Korrekturinställningar] längst ned i överföringsfönstret.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Språkkontroll]

På den här sidan spåras all aktivitet som har inträffat på korrekturet, plus e-postmeddelanden som skickades angående det här korrekturet.

![En bild av [!UICONTROL Språkkontroll] på korrektursidan med [!UICONTROL Språkkontroll] markerat alternativ på den vänstra panelmenyn.](assets/proofing-activity-in-details.png)

The [!UICONTROL Aktivitet] tidsstämplar när kommentarer och beslut togs, plus vem som gjorde dem. Den spårar också när korrekturarbetsflödesfaser startas, när en mottagare först öppnade ett korrektur och annan information som en korrekturansvarig eller ägare vill veta. Den här informationen kan vara användbar när du försöker komma på saker som varför en korrekturarbetsflödesfas aldrig startats, till exempel.

The [!UICONTROL Meddelanden] när e-postaviseringar och meddelanden skickades till mottagarna, som skickade dem och meddelandets innehåll. Detta kan vara användbart vid felsökning om någon säger att de inte fått något e-postmeddelande om ett korrektur. Du kan kontrollera om och när ett e-postmeddelande har skickats.

[!DNL Workfront] rekommenderar att korrekturläsaren och korrekturläsaren bekanta sig med informationen i dessa två avsnitt. När du kombinerar den här informationen med förståelse för hur du läser [!UICONTROL SOCD] förloppsindikator kan du verkligen förstå och hantera dina korrektur, oavsett var i korrekturarbetsflödet de befinner sig.

När du är klar med arbetet i [!UICONTROL Dokumentinformation] använder du spårningsfunktionen för att gå tillbaka till [!UICONTROL Dokument] del av projektet, uppgiften eller utleveransen som beviset är kopplat till.

![En bild av det synliga spåret i sidhuvudet.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
