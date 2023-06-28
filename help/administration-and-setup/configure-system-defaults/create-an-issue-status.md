---
title: Skapa en ärendestatus
description: Lär dig hur du skapar en problemstatus som uppfyller behoven i din organisations arbetsflöden.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Skapa en utleveransstatus

[!DNL Workfront] rekommenderar att du ändrar befintliga problem i systemet innan du börjar skapa nya statusar. Detta begränsar antalet statusar som behöver underhållas.

1. Klicka **[!UICONTROL Inställningar]** i **[!UICONTROL Huvudmeny]**.
1. Expandera **[!UICONTROL Projektinställningar]** i den vänstra menypanelen.
1. Välj **[!UICONTROL Status]**.
1. Välj **[!UICONTROL Problem]** -fliken.
1. Kontrollera att fältet i det övre högra hörnet är inställt på [!UICONTROL Systemstatus]. Detta garanterar att den nya statusen är tillgänglig globalt i din [!DNL Workfront] -instans.
1. Välj **[!UICONTROL Överordnad lista]** för att se alla status för utgåvor. Här skapar eller ändrar du en status.
1. Klicka **[!UICONTROL Lägg till en ny status]**.
1. Fyll i fälten efter behov för din organisation - namn, beskrivning, färg, motsvarar, nyckel osv.
1. Markera rutorna för den typ av problem som den här statusen kan användas med.
1. Klicka **[!UICONTROL Spara]**.

![Nytt statusfönster på [!UICONTROL Status] page](assets/admin-fund-create-issue-status.png)

## Utfärda status och gruppadministratörer

Gruppadministratörer kan skapa och anpassa utgivningsstatus för de grupper de hanterar. Detta ger en viss självständighet för deras grupp och ger dem de statusar de behöver för att fortsätta arbeta. Det eliminerar också behovet av en lång lista med systemomfattande status.

Gruppadministratörer kan redigera befintliga statusvärden om systemadministratören har konfigurerat dem för att tillåta anpassning.

Systemadministratörer kan hantera status för grupper genom att välja gruppnamnet i det övre högra hörnet i [!UICONTROL Status] -fönstret.

![Grupplistmeny på [!UICONTROL Status] page](assets/admin-fund-change-group-master-list.png)

Gruppadministratörer kan klicka på [!UICONTROL Grupper] i [!UICONTROL Inställningar] öppnar du gruppen genom att klicka på namnet och sedan markera [!UICONTROL Status] i den vänstra panelmenyn. Se till att du väljer fliken Problem.

![[!UICONTROL Status] avsnitt i [!UICONTROL Grupp] page](assets/admin-fund-group-issue-statuses.png)

<!---
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
--->

<!---
learn more URLs
Issue statuses
Create and customize system-wide statuses
--->
