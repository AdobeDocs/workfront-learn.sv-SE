---
title: Spåra förlopp från projekttidslinjen
description: Lär dig hur du spårar arbetets förlopp från projekttidslinjen i  [!DNL  Workfront] med procent färdigt, status, tilldelningar eller begränsningar.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Beginner
jira: KT-10150
hide: true
source-git-commit: 2351b6ff9977fd8a81289ab2fad28e21322d347e
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Spåra förlopp från projekttidslinjen

Se till att arbetsmomenten går som de ska för att klara deadlines. När du skannar igenom listan [!UICONTROL Aktivitet] finns det flera funktioner i [!DNL  Workfront] som hjälper dig att övervaka förloppet och statusen för arbetet.

## Procent färdigt

Procent färdigt för varje arbetsuppgift används ibland för att mäta hur arbetet fortskrider. Det är viktigt att notera.. att det här fältet måste justeras manuellt, eftersom det är den tilldelades uppskattning av hur långt de är.

>[!TIP]
>
>Även om procent färdigt för arbetsuppgifter måste uppdateras manuellt, beräknas procentandelen färdigt för en överordnad uppgift av Workfront baserat på procentandelen färdigt och antingen varaktigheten eller planerad tid för varje underordnad uppgift. Det innebär att du får bättre precision i procent om du delar upp stora uppgifter i mindre underaktiviteter.


![Projektuppgiftslista med kolumnen [!UICONTROL Procent färdigt]](assets/planner-fund-task-percent-complete.png)

Det finns tre gånger när procentandelen ändras automatiskt:

* När aktiviteten [!UICONTROL Status] är inställd på Fullständig ändras procentandelen slutförd till 100.
* Om aktiviteten [!UICONTROL Status] återställs till Nytt återställs procentandelen slutförd till 0.
* I en överordnad aktivitet när procentandelen slutfört för en underordnad aktivitet ändras.

## Status

Inkludera kolumnen [!UICONTROL Status] i en [!UICONTROL vy] för att snabbt se vilka aktiviteter som har startats, vilka som pågår och vilka som är slutförda. Du kan till och med ställa in villkorsstyrd formatering i en [!UICONTROL vy] för att färgkoda varje status, vilket gör informationen enklare att tolka.

## Uppgiftstilldelningar

Granska uppgiftstilldelningarna när du granskar projektet. Arbetet kanske blev försenat eftersom ingen tilldelades uppdraget. Eller så hade den tilldelade personen inte rätt kompetens för att slutföra arbetet. Lägg till fler personer i en uppgift eller tilldela om uppgifter för att säkerställa att arbetet blir gjort.

## Aktivitetsbegränsning

Ibland ändras uppgiftsbegränsningarna och du inser inte det. Begränsningar kan påverka hur tidslinjen fungerar, så du bör se till att de är inställda så som du vill ha dem.

![Projektuppgiftslista med aktivitetsbegränsningskolumn](assets/planner-fund-task-constraint.png)

Skapa en anpassad vy som innehåller kolumnen [!UICONTROL Aktivitetsbegränsning] om du vill visa den här informationen i uppgiftslistan. Om du planerade projektet från ett startdatum vill du att dina aktiviteter ska ha begränsningen [!UICONTROL Så snart som möjligt] ([!UICONTROL ASAP]).

Mer information om uppgiftsbegränsningar finns i [Förstå och hantera varaktighetstyper och aktivitetsbegränsningar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).
