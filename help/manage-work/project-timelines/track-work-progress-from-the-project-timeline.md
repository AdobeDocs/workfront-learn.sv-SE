---
title: Spåra förlopp från projekttidslinjen
description: Lär dig hur du spårar arbetets förlopp från tidslinjen i projektet i [!DNL  Workfront] med procent färdigt, status, tilldelningar eller begränsningar.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Intermediate
jira: KT-10150
exl-id: c8793f49-24b8-48cc-af84-5239234ead0e
source-git-commit: e25a7c0119567c068504edcb8c3ddd29622d52c5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# Spåra förlopp från projekttidslinjen

Se till att arbetsmomenten går som de ska för att klara deadlines. När du skannar genom [!UICONTROL Uppgift] finns det flera funktioner i [!DNL  Workfront] som hjälper dig att övervaka arbetets förlopp och status.

## Procent färdigt

Procent färdigt för varje arbetsuppgift används ibland för att mäta hur arbetet fortskrider. Det är viktigt att notera.. att det här fältet måste justeras manuellt, eftersom det är den tilldelades uppskattning av hur långt de är.

>[!TIP]
>
>Även om procent färdigt för arbetsuppgifter måste uppdateras manuellt, beräknas procentandelen färdigt för en överordnad uppgift av Workfront baserat på procentandelen färdigt och antingen varaktigheten eller planerad tid för varje underordnad uppgift. Det innebär att du får bättre precision i procent om du delar upp stora uppgifter i mindre underaktiviteter.


![Lista över projektuppgifter som visas [!UICONTROL Procent färdigt] kolumn](assets/planner-fund-task-percent-complete.png)

Det finns tre gånger när procentandelen ändras automatiskt:

* När uppgiften [!UICONTROL Status] är inställt på Fullständig, ändras procentandelen till 100.
* Om uppgiften [!UICONTROL Status] återgår till Nytt, procentandelen slutförd återställs till 0.
* I en överordnad aktivitet när procentandelen slutfört för en underordnad aktivitet ändras.

## Status

Inkludera [!UICONTROL Status] kolumn i en [!UICONTROL Visa] för att snabbt se vilka åtgärder som har startats, vilka som pågår och vilka som är slutförda. Du kan till och med ställa in villkorsstyrd formatering i en [!UICONTROL Visa] om du vill färgkoda varje status, vilket gör informationen enklare att tolka.

## Uppgiftstilldelningar

Granska uppgiftstilldelningarna när du granskar projektet. Arbetet kanske blev försenat eftersom ingen tilldelades uppdraget. Eller så hade den tilldelade personen inte rätt kompetens för att slutföra arbetet. Lägg till fler personer i en uppgift eller tilldela om uppgifter för att säkerställa att arbetet blir gjort.

## Aktivitetsbegränsning

Ibland ändras uppgiftsbegränsningarna och du inser inte det. Begränsningar kan påverka hur tidslinjen fungerar, så du bör se till att de är inställda så som du vill ha dem.

![Projektuppgiftslista som visar aktivitetsbegränsningskolumn](assets/planner-fund-task-constraint.png)

Skapa en anpassad vy som innehåller [!UICONTROL Aktivitetsbegränsning] om du vill visa den här informationen i uppgiftslistan. Om du har planerat projektet från ett startdatum vill du att dina aktiviteter ska ha [!UICONTROL Så snart som möjligt] ([!UICONTROL ASAP]).

Mer information om uppgiftsbegränsningar finns i [Förstå och hantera varaktighetstyper och uppgiftsbegränsningar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html).
