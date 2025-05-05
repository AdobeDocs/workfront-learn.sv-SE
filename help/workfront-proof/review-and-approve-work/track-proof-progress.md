---
title: Spåra korrekturstatus
description: Lär dig hur du använder [!UICONTROL SOCD]-indikatorer, korrekturförlopp och rapporter för att spåra förloppet för ett korrektur i  [!DNL &#x200B; Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# Spåra korrekturstatus

Som projektledare, korrekturansvarig eller andra intressenter i gransknings- och godkännandeprocessen vill du följa upp korrekturens förlopp. Du kan göra detta med [!DNL Workfront’s] inbyggda **korrekturförloppsindikatorer** på sidan [!UICONTROL Dokument] eller genom att skriva anpassade rapporter.

Om du vill visa korrekturstatus i [!DNL Workfront] måste du ha en plan-, arbets- eller granskningslicens och vara en korrekturanvändare. Om du inte är säker på om din [!DNL Workfront]-profil uppfyller dessa krav kontaktar du systemadministratören för språkkontroll i din organisation.

## Spåra korrekturstatus med [!UICONTROL SOCD]-indikatorer och korrekturstatus

Få en översikt över hur korrekturet fortskrider genom gransknings- och godkännandeprocessen med hjälp av ikonerna [!UICONTROL SOCD] i listan [!UICONTROL Dokument] . De här ikonerna anger specifika åtgärder som vidtagits för korrekturet.

![En bild av listan [!UICONTROL Dokument] i ett [!DNL &#x200B; Workfront]-projekt med ikonerna [!UICONTROL SOCD] markerade.](assets/manage-proofs-socd.png)

Ikonerna anger det arbete som utförts med ett korrektur från det att du skickar beviset till mottagarna tills de fattar ett beslut om beviset.

* **S —** Beviset har skickats till mottagarna.
* **O —** Beviset har öppnats.
* **C —** kommentarer har gjorts på korrekturet.
* **D -** Ett beslut har fattats om beviset (godkänt, avvisat, osv.).

Färgerna anger om åtgärden är fullständig eller inte.

* **Vit -** Stegen har inte utförts än.
* **Grön -** Steget har slutförts.
* **Orange -** Korrekturens deadline är inom 24 timmar och steget har inte utförts.
* **Rött -** Korrekturens deadline har passerats och steget har inte utförts.

[!UICONTROL SOCD] i listan [!UICONTROL Dokument], på sammanfattningspanelen eller i [!UICONTROL Dokumentinformation] är en sammanfattning på hög nivå av korrekturets förlopp. [!DNL Workfront] konfigurerar detta baserat på mottagaren som är &quot;längst bak&quot; i korrekturläsningsprocessen.

Om det till exempel finns tre granskare/godkännare och bara två av dem har tittat på korrekturet och gjort kommentarer, visar ikonerna [!UICONTROL SOCD] att korrekturet har skickats ([!UICONTROL S]) och öppnats ([!UICONTROL O]), men inte att kommentarer har gjorts ([!UICONTROL C]).

Om du vill veta hur varje enskild korrekturmottagare gör öppnar du korrekturarbetsflödet. Det övergripande korrekturförloppet visas högst upp i fönstret. Varje fas har en egen förloppsindikator i det grå fältet.  Och bredvid varje användare finns personens förlopp.

![En bild av avsnittet [!UICONTROL Korrekturarbetsflöde] i ett dokument.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Korrekturstatus

Korrekturstatusen baseras på statusen för scenens korrekturmottagare. Den övergripande korrekturstatusen visas på sidan [!UICONTROL Dokument] till höger om indikatorerna för [!UICONTROL SOCD] så att du enkelt kan se om du har något beslut om korrekturet.

![En bild av listan [!UICONTROL Dokument] i ett [!DNL &#x200B; Workfront]-projekt med den övergripande korrekturstatusen markerad.](assets/manage-proofs-overall-status.png)

Den här korrekturstatusen anger den övergripande statusen för beviset. Om till exempel två mottagare har godkänt korrekturet visas deras individuella status som [!UICONTROL Godkänd]. Den tredje mottagaren har dock inte fattat något beslut än, så personens status är [!UICONTROL Väntande]. Därför visas den övergripande statusen som [!UICONTROL Väntande].

Om anpassade statusvärden har konfigurerats för din organisation kommer dessa statusvärden att användas. I annat fall visas standardstatusalternativen för:

* [!UICONTROL Väntande]
* [!UICONTROL Godkänd]
* [!UICONTROL Godkänd med ändringar]
* [!UICONTROL Ändringar krävs]
* [!UICONTROL Inte relevant]

Öppna arbetsflödesfönstret för korrektur för att se korrekturstatus för mottagare som tilldelats korrekturrollerna [!UICONTROL Granskare och godkännare] eller [!UICONTROL Godkännare].

## Rapporter i [!DNL Workfront]

Du kan också utnyttja rapportfunktionerna i [!DNL Workfront’s] för att spåra korrektur när de går igenom gransknings- och godkännandeprocessen.

En rapport om godkännande av korrektur hjälper dig att spåra utestående godkännanden för att säkerställa att deadlines hålls.

![En bild av en rapport om godkännande av korrektur i [!DNL &#x200B; Workfront].](assets/proof-approval-report.png)

Med en dokumentversionsrapport kan du hantera och spåra korrekturversioner.

![En bild av en dokumentversion i [!DNL &#x200B; Workfront].](assets/document-version-report.png)

Vi rekommenderar att du samarbetar med din [!DNL Workfront]-konsult för att skapa rapporter som uppfyller organisationens krav. Vissa rapporter kräver att du är bekant med [!DNL Workfront’s]-textlägesrapportering.

## Din tur

Tala med teamet eller administratören för korrekturläsningssystemet för att ta reda på vilken typ av rapportering du kommer att använda i Workfront för att få korrekturrutorna att löpa smidigt.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
