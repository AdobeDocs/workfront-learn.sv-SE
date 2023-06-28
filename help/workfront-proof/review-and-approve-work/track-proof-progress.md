---
title: Spåra korrekturstatus
description: Lär dig använda [!UICONTROL SOCD] indikatorer, korrekturrundor och rapporter för att följa upp korrekturens förlopp i [!DNL  Workfront].
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
source-wordcount: '674'
ht-degree: 0%

---

# Spåra korrekturstatus

Som projektledare, korrekturansvarig eller andra intressenter i gransknings- och godkännandeprocessen vill du följa upp korrekturens förlopp. Du kan göra det här med [!DNL Workfront’s] inbyggd **visa förloppsindikatorer** på [!UICONTROL Dokument] sida eller genom att skriva anpassade rapporter.

Visa korrekturförloppet [!DNL Workfront]måste du ha en plan-, Work- eller Review-licens och vara en korrekturanvändare. Om du inte är säker på att [!DNL Workfront] profilen uppfyller dessa krav, kontakta systemadministratören för korrektur på din organisation.

## Spåra korrekturrundor med [!UICONTROL SOCD] indikatorer och korrekturstatus

Få en översikt över hur korrekturet fortskrider genom gransknings- och godkännandeprocessen med [!UICONTROL SOCD] ikoner i [!UICONTROL Dokument] lista. De här ikonerna anger specifika åtgärder som vidtagits för korrekturet.

![En bild av [!UICONTROL Dokument] lista i en [!DNL  Workfront] projektet med [!UICONTROL SOCD] ikoner är markerade.](assets/manage-proofs-socd.png)

Ikonerna anger det arbete som utförts med ett korrektur från det att du skickar beviset till mottagarna tills de fattar ett beslut om beviset.

* **S -** Beviset har skickats till mottagarna.
* **O —** Beviset har öppnats.
* **C —** Beviset innehåller kommentarer.
* **D -** Ett beslut har fattats om beviset (godkänt, avvisat osv.).

Färgerna anger om åtgärden är fullständig eller inte.

* **Vit -** Stegen har inte utförts än.
* **Grön -** Stegen har slutförts.
* **Orange -** Tidsgränsen för korrektur är inom 24 timmar och steget har inte utförts.
* **Röd -** Tidsgränsen för korrektur har passerats och steget har inte utförts.

The [!UICONTROL SOCD] på [!UICONTROL Dokument] i sammanfattningspanelen eller i [!UICONTROL Dokumentinformation], är en sammanfattning av korrekturens förlopp på hög nivå. [!DNL Workfront] konfigurerar detta baserat på mottagaren som är den&quot;mest bakomliggande&quot; i korrekturläsningsprocessen.

Om det till exempel finns tre granskare/godkännare och bara två av dem har tittat på korrekturet och gjort kommentarer, så är [!UICONTROL SOCD] -ikonerna visar att beviset har skickats ([!UICONTROL S]) och öppnad ([!UICONTROL O]) men inte att kommentarer har gjorts ([!UICONTROL C]).

Om du vill veta hur varje enskild korrekturmottagare gör öppnar du korrekturarbetsflödet. Det övergripande korrekturförloppet visas högst upp i fönstret. Varje fas har en egen förloppsindikator i det grå fältet.  Och bredvid varje användare finns personens förlopp.

![En bild av [!UICONTROL Korrektur] i ett dokument.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Korrekturstatus

Korrekturstatusen baseras på statusen för scenens korrekturmottagare. Den övergripande korrekturstatusen visas på [!UICONTROL Dokument] till höger om sidan [!UICONTROL SOCD] så att du enkelt kan se om du har något beslut om beviset.

![En bild av [!UICONTROL Dokument] lista i en [!DNL  Workfront] projekt med den övergripande korrekturstatusen markerad.](assets/manage-proofs-overall-status.png)

Den här korrekturstatusen anger den övergripande statusen för beviset. Om till exempel två mottagare har godkänt korrekturet visas deras individuella status [!UICONTROL Godkänd]. Den tredje mottagaren har dock inte fattat något beslut än, så personens status är [!UICONTROL Väntande]. Den övergripande statusen är därför [!UICONTROL Väntande].

Om anpassade statusvärden har konfigurerats för din organisation används dessa statusvärden. I annat fall visas standardstatusalternativen för:

* [!UICONTROL Väntande]
* [!UICONTROL Godkänd]
* [!UICONTROL Godkänd med ändringar]
* [!UICONTROL Ändringar krävs]
* [!UICONTROL Ej relevant]

Öppna arbetsflödesfönstret för korrektur för att se korrekturstatus för mottagare som tilldelats [!UICONTROL Granskare och godkännare] eller [!UICONTROL Godkännare]korrekturroller.

## Rapporter i [!DNL Workfront]

Du kan också utnyttja [!DNL Workfront’s] möjlighet att spåra korrektur när de går igenom gransknings- och godkännandeprocessen.

En rapport om godkännande av korrektur hjälper dig att spåra utestående godkännanden för att säkerställa att deadlines hålls.

![En bild av en rapport om godkännande av korrektur i [!DNL  Workfront].](assets/proof-approval-report.png)

Med en dokumentversionsrapport kan du hantera och spåra korrekturversioner.

![En bild av en dokumentversionsrapport i [!DNL  Workfront].](assets/document-version-report.png)

Vi rekommenderar att du arbetar med [!DNL Workfront] för att skapa rapporter som uppfyller organisationens krav. Vissa rapporter kräver att man känner till [!DNL Workfront’s] textlägesrapportering.

## Din tur

Tala med teamet eller administratören för korrekturläsningssystemet för att ta reda på vilken typ av rapportering du kommer att använda i Workfront för att få korrekturrutorna att löpa smidigt.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
