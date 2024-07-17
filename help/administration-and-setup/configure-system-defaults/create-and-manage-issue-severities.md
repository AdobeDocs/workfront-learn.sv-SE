---
title: Skapa och hantera problem med allvarlighetsgrad
description: Lär dig hur du konfigurerar och hanterar problemallvarliga problem.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Skapa och hantera problem

## Introduktion till allvarlighetsgrad för utfärdande

En allvarlighetsgrad kan användas för att ange hur allvarliga ett problem är eller hur det kan påverka det arbete som utförs.

![[!UICONTROL Allvarlighetsgrad] i fönstret [!UICONTROL Ärendeinformation]](assets/admin-fund-severity-issue-details.png)

Fältet [!UICONTROL Allvarlighetsgrad] finns i [!UICONTROL Ärendeinformation]. Den kan också tas med i kolumnvyer i listor och i anpassade rapporter.

[!DNL Workfront] har fem standardallvarlighetsgrader:

* [!UICONTROL Kosmetisk]
* [!UICONTROL orsakar förvirring]
* [!UICONTROL Fel med lösning]
* [!UICONTROL Fel utan någon lösning]
* [!UICONTROL Allvarligt fel]

Systemadministratörer kan vid behov ändra namn på standardserierna eller skapa nya.

Allvarlighetsgrader är bara tillgängliga för problem i [!DNL Workfront].

## Skapa och hantera problem

Som systemadministratör kan du skapa nya allvarlighetsgrader om det behövs för att slutföra problemets arbetsflöde.

![[!UICONTROL Allvarlighetsgrader] på sidan [!UICONTROL Inställningar]](assets/admin-fund-severity-section.png)

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Expandera avsnittet **[!UICONTROL Projektinställningar]** på den vänstra menypanelen.
1. Välj **[!UICONTROL Allvarlighetsgrader]**.
1. Klicka på **[!UICONTROL Lägg till en ny allvarlighetsgrad]**.
1. Ge allvarlighetsgraden ett namn som matchar dess avsedda användning.
1. Numret **[!UICONTROL Prioritet]** matchar problemets allvarlighetsgrad. Den högsta siffran motsvarar den högsta allvarlighetsgraden. [!UICONTROL Importance]-numret måste vara unikt.
1. Välj en färg som du vill prioritera. Detta används i diagramrapporter och andra platser i [!DNL Workfront].
1. Ange ett av allvarlighetsalternativen som **[!UICONTROL Standardallvarlighetsgrad]**. Detta gäller automatiskt alla nya utgåvor av Workfront.
1. Ta med en beskrivning av allvarlighetsgraden, till exempel hur den kommer att användas.
1. Klicka utanför de fält som ska sparas.

![[!UICONTROL Allvarlighetsgrader] lista](assets/admin-fund-severity-new.png)

### Ändra allvarlighetsgrad

Om en allvarlighetsgrad inte längre är relevant för dina problemarbetsflöden kan den döpas om, döljas eller tas bort.

Om en allvarlighetsgrad inte längre behövs rekommenderar [!DNL Workfront] att du döljer allvarlighetsgraden (klicka i rutan [!UICONTROL Dölj] bredvid den i inställningsområdet). Detta tar bort allvarlighetsgraden från den nedrullningsbara menyn i problemet, men det bevarar allvarlighetsgraden i historiska data så att de fortfarande är tillgängliga för rapportering.

![[!UICONTROL Dölj] kolumn markerad på sidan [!UICONTROL Allvarlighetsgrader] i [!UICONTROL Inställningar]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] rekommenderar att du **inte** tar bort en allvarlighetsgrad som har använts i tidigare utgåvor. När du tar bort en allvarlighetsgrad uppmanas du att ersätta en annan. Detta kan ändra historiska data och påverka rapporteringen.

![Ta bort allvarlighetsfönstret](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
