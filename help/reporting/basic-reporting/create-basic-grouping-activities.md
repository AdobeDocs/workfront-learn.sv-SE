---
title: Skapa grundläggande grupperingsaktiviteter
description: Skapa enkelt grupperingar steg för steg.
activity: use
feature: Reports and Dashboards
thumbnail: 335147.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8853
hidefromtoc: true
exl-id: 36f196ac-ad14-4075-9835-30f777572fdf
source-git-commit: 8a033140307527fbd7c4f9298353ba88cab66c86
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Aktivitet: Skapa en grundläggande gruppering

Skapa en ärendegruppering som ska användas i en rapport för att spåra begäranden som kommer via en begärandekö. Den här grupperingen gör det enkelt att se liknande typer av problem/förfrågningar grupperade efter prioritet. Namnge grupperingen &quot;Begär kö, Köämne, Prioritet&quot;.

Gruppera problemrapporten utifrån:

1. Namnet på begärandekön (det här blir projektnamnet)
1. Köämnet
1. Förfrågans prioritet

## Svar

![En bild av skärmen för att skapa en ny gruppering](assets/grouping-exercise.png)

1. Gå till menyn **[!UICONTROL Gruppering]** i en problemlistrapport och välj **[!UICONTROL Ny gruppering]**.
1. Namnge din gruppering&quot;Begär kön, Köämne, Prioritet&quot;.
1. Klicka på **[!UICONTROL Lägg till gruppering]**.
1. I fältet [!UICONTROL First By]. Skriv&quot;projektnamn&quot; och välj sedan **[!UICONTROL Namn]** under Projektfältets källa.
1. Klicka på **[!UICONTROL Lägg till en annan gruppering]**.
1. I fältet [!UICONTROL Och sedan av] skriver du &quot;queue&quot; och väljer sedan **[!UICONTROL Name]** under fältkällan [!UICONTROL Queue Topic].
1. Klicka på **[!UICONTROL Lägg till en annan gruppering]**.
1. I fältet [!UICONTROL Och sedan av] skriver du&quot;priority&quot; och väljer sedan **[!UICONTROL Priority]** under fältkällan [!UICONTROL Issue].
1. Klicka på **[!UICONTROL Spara gruppering]**
