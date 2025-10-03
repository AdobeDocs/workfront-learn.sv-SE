---
title: Konfigurera grupper och användare
description: Lär dig skapa mappar, grupper och användare i [!UICONTROL Workfront DAM]. Förstå användarrolltyperna och tilldela behörigheter till mappar.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Konfigurera grupper och användare

I den här videon får du lära dig att:

* Förstå hur gruppinställningar påverkar åtkomsten till resurser
* Skapa mappar, grupper och användare i en viss ordning
* Förstå användarrolltyperna
* Bevilja behörigheter för mappar
* Skapa och redigera grupper
* Lägga till och redigera användare

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on&enablevpops=1)

## Grupper och användare granskar

När du konfigurerar ditt [!UICONTROL Workfront DAM]-system är det viktigt att tänka på vilka roller användare och grupper spelar i helhetsbilden.

Grupper styr åtkomst till resursmappar i [!UICONTROL Workfront DAM]. Gruppinställningarna styr också vad användare kan göra med de resurser (visa, hämta, redigera osv.) som de har behörighet att komma åt.

När du skapar grupper är det viktigt att tänka på vilka resursmappar medlemmarna i gruppen behöver åtkomst till i [!UICONTROL Workfront DAM].

Användare är de personer som har inloggningar på [!UICONTROL Workfront DAM]. En användare kan inte komma åt någonting i [!UICONTROL Workfront DAM] om de inte är tilldelade till en grupp. Användare kan tillhöra mer än en grupp, beroende på deras behov.

## Standardgrupper

Det finns två standardgrupper som medföljer [!UICONTROL Workfront DAM]. Alla användare tillhör dessa grupper automatiskt, baserat på om de har inloggningsuppgifter för [!UICONTROL Workfront DAM] eller inte. Du kan inte lägga till eller ta bort användare från dessa grupper:

* **Gästgrupp** - Används för att styra åtkomst för en anonym användare. Detta kan vara någon utan inloggningsuppgifter eller en användare som inte är inloggad.
* **Inloggad**-grupp - Alla användare som är inloggade tillhör den här gruppen.

Administratörsgruppen och dess inställningar finns också som standard. Du kan lägga till användare i den här gruppen, men du kan inte justera inställningarna.

## Rolltyper

När grupper skapas tilldelas de en rolltyp. Rolltypen avgör vilken del av [!UICONTROL Workfront DAM] -systemanvändarna får när de loggar in: [!UICONTROL Workfront DAM] eller [!UICONTROL Brand Connect].

Det finns tre rolltyper tillgängliga med [!UICONTROL Workfront DAM]-licenser:

* **[!UICONTROL Brand Portal]** - De här användarna har bara åtkomst till [!UICONTROL Brand Connect], där de kan visa och hämta godkända resurser.
* **[!UICONTROL Contributor]** - Dessa användare har tillgång till [!UICONTROL Workfront DAM] och [!UICONTROL Brand Connect]. De har fullständig behörighet till resurser och mappar - visa, ladda ned, ladda upp, redigera, flytta och ta bort.
* **[!UICONTROL Administratör]** - Systemadministratörer har tillgång till allt i [!UICONTROL Brand Connect] och [!UICONTROL Workfront DAM], plus möjligheten att skapa globala systeminställningar för varje. De kan också komma åt resurser som har gått ut eller som har angetts som inaktiva.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
