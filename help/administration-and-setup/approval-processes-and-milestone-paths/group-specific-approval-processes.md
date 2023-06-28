---
title: Förstå gruppspecifika godkännandeprocesser
description: Lär dig hur gruppadministratörer kan skapa eller redigera godkännandeprocesser för de grupper som de hanterar.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Förstå gruppspecifika godkännandeprocesser

Både system- och gruppadministratörer kan skapa godkännandeprocesser i [!DNL Workfront]. Systemadministratörer kan skapa processer som kan användas i hela [!DNL Workfront] eller bara för en viss grupp. Gruppadministratörer kan bara skapa eller redigera processer för den grupp de hanterar.

För en godkännandeprocess som kan användas av alla i [!DNL Workfront], kontrollera att [!UICONTROL &quot;Den här godkännandeprocessen kan användas av&quot;] fältet är inställt på [!UICONTROL Alla grupper].

![[!UICONTROL Redigera godkännandeprocess] fönster med gruppfält markerat](assets/admin-fund-approval-processes-1.png)

De statusvärden som är tillgängliga i [!UICONTROL &quot;Starta godkännandeprocessen när statusen är inställd på&quot;] -menyn beror på vad som har valts i fältet &quot;används av&quot;. Med [!UICONTROL Alla grupper] Om du väljer det här alternativet är endast systemomfattande låsta statusvärden tillgängliga.

Om du vill begränsa en godkännandeprocess för en viss grupp väljer du den gruppens namn i listan för [!UICONTROL &quot;Den här godkännandeprocessen kan användas av&quot;] fält.

![[!UICONTROL Redigera godkännandeprocess] fönster med gruppfält utökat](assets/admin-fund-approval-processes-2.png)

The [!UICONTROL Alla grupper] är inte tillgängligt för gruppadministratörer.

När en viss grupp är markerad visas bara de statusar som är tillgängliga för den gruppen i [!UICONTROL &quot;Starta godkännandeprocessen när statusen är inställd på&quot;] -menyn.

![[!UICONTROL Redigera godkännandeprocess] fönster med statusfältet markerat](assets/admin-fund-approval-processes-3.png)

