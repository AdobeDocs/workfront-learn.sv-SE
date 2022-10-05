---
title: Skapa och hantera problem med allvarlighetsgrad
description: Lär dig hur du konfigurerar och hanterar problemallvarliga problem.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Skapa och hantera problem

## Introduktion till allvarlighetsgrad för utfärdande

En allvarlighetsgrad kan användas för att ange hur allvarliga ett problem är eller hur det kan påverka det arbete som utförs.

![[!UICONTROL Allvarlighetsgrad] i [!UICONTROL Ärendeinformation] window](assets/admin-fund-severity-issue-details.png)

The [!UICONTROL Allvarlighetsgrad] kan öppnas i [!UICONTROL Ärendeinformation]. Den kan också tas med i kolumnvyer i listor och i anpassade rapporter.

[!DNL Workfront] har fem standardallvarlighetsgrader:

* [!UICONTROL Kosmetisk]
* [!UICONTROL Orsakar förvirring]
* [!UICONTROL Fel med tillfälliga lösningar]
* [!UICONTROL Fel utan någon lösning]
* [!UICONTROL Allvarligt fel]

Systemadministratörer kan vid behov ändra namn på standardserierna eller skapa nya.

Allvarlighetsgrader är endast tillgängliga för problem i [!DNL Workfront].

## Skapa och hantera problem

Som systemadministratör kan du skapa nya allvarlighetsgrader om det behövs för att slutföra problemets arbetsflöde.

![[!UICONTROL Allvarlighetsgrader] sida in [!UICONTROL Inställningar]](assets/admin-fund-severity-section.png)

1. Klicka **[!UICONTROL Inställningar]** i **[!UICONTROL Huvudmeny]**.
1. Expandera **[!UICONTROL Projektinställningar]** i den vänstra menypanelen.
1. Välj **[!UICONTROL Allvarlighetsgrader]**.
1. Klicka **[!UICONTROL Lägg till en ny allvarlighetsgrad]**.
1. Ge allvarlighetsgraden ett namn som matchar dess avsedda användning.
1. The **[!UICONTROL Prioritet]** talet motsvarar problemets allvarlighetsgrad. Den högsta siffran motsvarar den högsta allvarlighetsgraden. The [!UICONTROL Prioritet] talet måste vara unikt.
1. Välj en färg som du vill prioritera. Detta används i diagramrapporter och på andra platser i [!DNL Workfront].
1. Ange ett av allvarlighetsgraden som **[!UICONTROL Standardallvarlighetsgrad]**. Detta gäller automatiskt alla nya utgåvor av Workfront.
1. Ta med en beskrivning av allvarlighetsgraden, till exempel hur den kommer att användas.
1. Klicka utanför de fält som ska sparas.

![[!UICONTROL Allvarlighetsgrader] list](assets/admin-fund-severity-new.png)

### Ändra allvarlighetsgrad

Om en allvarlighetsgrad inte längre är relevant för dina problemarbetsflöden kan den döpas om, döljas eller tas bort.

Om en allvarlighetsgrad inte längre behövs, [!DNL Workfront] rekommenderar att du döljer allvarlighetsgraden (klicka på [!UICONTROL Dölj] -rutan bredvid den i inställningsområdet). Detta tar bort allvarlighetsgraden från den nedrullningsbara menyn i problemet, men det bevarar allvarlighetsgraden i historiska data så att de fortfarande är tillgängliga för rapportering.

![[!UICONTROL Dölj] kolumn markerad på [!UICONTROL Allvarlighetsgrader] sida in [!UICONTROL Inställningar]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] rekommenderar att du **inte** ta bort en allvarlighetsgrad som har använts på tidigare utgåvor. När du tar bort en allvarlighetsgrad uppmanas du att ersätta en annan. Detta kan ändra historiska data och påverka rapporteringen.

![Ta bort allvarlighetsgraden i fönstret](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
