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
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Skapa en utleveransstatus

[!DNL Workfront] rekommenderar att du ändrar de befintliga utgivningsstatusarna i systemet innan du börjar skapa nya statusar. Detta begränsar antalet statusar som behöver underhållas.

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Expandera avsnittet **[!UICONTROL Projektinställningar]** på den vänstra menypanelen.
1. Välj **[!UICONTROL Status]**.
1. Välj fliken **[!UICONTROL Problem]**.
1. Kontrollera att fältet i det övre högra hörnet är inställt på [!UICONTROL Systemstatus]. Detta garanterar att den nya statusen är tillgänglig globalt i din [!DNL Workfront]-instans.
1. Välj **[!UICONTROL Huvudlista]** om du vill visa alla utgivningsstatus. Här skapar eller ändrar du en status.
1. Klicka på **[!UICONTROL Lägg till en ny status]**.
1. Fyll i fälten efter behov för din organisation - namn, beskrivning, färg, motsvarar, nyckel osv.
1. Markera rutorna för den typ av problem som den här statusen kan användas med.
1. Klicka på **[!UICONTROL Spara]**.

![Nytt statusfönster på sidan [!UICONTROL Status] &#x200B;](assets/admin-fund-create-issue-status.png)

## Utfärda status och gruppadministratörer

Gruppadministratörer kan skapa och anpassa utgivningsstatus för de grupper som de hanterar. Detta ger en viss självständighet för deras grupp och ger dem de statusar de behöver för att fortsätta arbeta. Det eliminerar också behovet av en lång lista med systemomfattande status.

Gruppadministratörer kan redigera befintliga statusvärden om systemadministratören har konfigurerat dem för att tillåta anpassning.

Systemadministratörer kan hantera status för grupper genom att markera gruppnamnet i det övre högra hörnet av fönstret [!UICONTROL Status] .

![Menyn Grupplista på sidan [!UICONTROL Status] &#x200B;](assets/admin-fund-change-group-master-list.png)

Gruppadministratörer kan klicka i avsnittet [!UICONTROL Grupper] i området [!UICONTROL Inställningar], öppna gruppen genom att klicka på namnet och sedan välja [!UICONTROL Status] på den vänstra panelmenyn. Se till att du väljer fliken Problem.

![[!UICONTROL Status] avsnitt av [!UICONTROL Grupp] sida](assets/admin-fund-group-issue-statuses.png)

<!--
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
-->

<!--
learn more URLs
Issue statuses
Create and customize system-wide statuses
-->
