---
title: Förstå grupper och användare i [!UICONTROL Workfront DAM]
description: Lär dig hur du skapar mappar, grupper och användare i [!UICONTROL Workfront DAM]. Förstå användarrolltyperna och tilldela behörigheter till mappar.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Systemkonfiguration: grupper och användare

I den här videon får du lära dig att:

* Förstå hur gruppinställningar påverkar åtkomsten till resurser
* Skapa mappar, grupper och användare i en viss ordning
* Förstå användarrolltyperna
* Bevilja behörigheter för mappar
* Skapa och redigera grupper
* Lägga till och redigera användare

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## Grupper och användare granskar

När du konfigurerar [!UICONTROL Workfront DAM] är det viktigt att tänka på vilka roller användare och grupper spelar i helheten.

Grupper styr åtkomst till resursmappar i [!UICONTROL Workfront DAM]. Gruppinställningarna styr också vad användare kan göra med resurserna (visa, hämta, redigera osv.) de har åtkomstbehörighet.

När du skapar grupper är det viktigt att tänka på vilka resursmappar medlemmarna i gruppen behöver åtkomst till i [!UICONTROL Workfront DAM].

Användarna är de personer som har inloggningar på [!UICONTROL Workfront DAM]. En användare kan inte komma åt någonting i [!UICONTROL Workfront DAM] såvida de inte har tilldelats en grupp. Användare kan tillhöra mer än en grupp, beroende på deras behov.

## Standardgrupper

Det finns två standardgrupper [!UICONTROL Workfront DAM]. Alla användare tillhör dessa grupper automatiskt, baserat på om de har [!UICONTROL Workfront DAM] inloggningsuppgifter. Du kan inte lägga till eller ta bort användare från dessa grupper:

* **Gästgrupp**—Används för att styra åtkomst för en anonym användare. Detta kan vara någon utan inloggningsuppgifter eller en användare som inte är inloggad.
* **Loggade**-In group - Alla användare som är inloggade tillhör den här gruppen.

Administratörsgruppen och dess inställningar finns också som standard. Du kan lägga till användare i den här gruppen, men du kan inte justera inställningarna.

## Rolltyper

När grupper skapas tilldelas de en rolltyp. Rolltypen avgör vilken del av [!UICONTROL Workfront DAM] systemanvändare får när de loggar in — [!UICONTROL Workfront DAM] sig själv eller [!UICONTROL Brand Connect].

Det finns tre rolltyper tillgängliga med [!UICONTROL Workfront DAM] licenser:

* **[!UICONTROL Brand Portal]**—De här användarna har endast åtkomst till [!UICONTROL Brand Connect], där de kan visa och hämta godkända mediefiler.
* **[!UICONTROL Medarbetare]**—Dessa användare har åtkomst [!UICONTROL Workfront DAM] och [!UICONTROL Brand Connect]. De har fullständig behörighet till resurser och mappar - visa, ladda ned, ladda upp, redigera, flytta och ta bort.
* **[!UICONTROL Administratör]**—Systemadministratörer har tillgång till allt i [!UICONTROL Brand Connect] och [!UICONTROL Workfront DAM], plus möjligheten att ange globala systeminställningar för varje. De kan också komma åt resurser som har gått ut eller som har angetts som inaktiva.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
