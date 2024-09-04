---
title: Förstå gruppspecifika godkännandeprocesser
description: Lär dig hur gruppadministratörer kan skapa eller redigera godkännandeprocesser för de grupper som de hanterar.
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
hide: true
source-git-commit: c675114a7f82521a59072f80a64d314be4cd335d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Förstå gruppspecifika godkännandeprocesser

Både system- och gruppadministratörer kan skapa godkännandeprocesser i [!DNL Workfront]. Systemadministratörer kan skapa processer som ska användas i hela [!DNL Workfront]-systemet, eller processer som bara ska användas för en viss grupp. Gruppadministratörer kan bara skapa eller redigera processer för den grupp de hanterar.

För en godkännandeprocess som kan användas av alla i [!DNL Workfront] kontrollerar du att fältet [!UICONTROL &quot;Den här godkännandeprocessen kan användas av&quot;]&quot; är inställt på [!UICONTROL Alla grupper].

Fönstret ![[!UICONTROL Redigera godkännandeprocess] med gruppfältet markerat](assets/admin-fund-approval-processes-1.png)

Vilka statusar som är tillgängliga i [!UICONTROL &quot;Starta godkännandeprocess när statusen är inställd på&quot;]&quot; beror på valet i fältet&quot;används av&quot;. Om [!UICONTROL Alla grupper] är markerade är endast systemomfattande låsta statusar tillgängliga.

Om du vill begränsa en godkännandeprocess för en viss grupp väljer du den gruppens namn i listan för fältet [!UICONTROL &quot;Den här godkännandeprocessen kan användas av&quot;]&quot;.

Fönstret ![[!UICONTROL Redigera godkännandeprocess] med gruppfältet utökat](assets/admin-fund-approval-processes-2.png)

Alternativet [!UICONTROL Alla grupper] är inte tillgängligt för gruppadministratörer.

När en viss grupp har valts visas endast de statusar som är tillgängliga för den gruppen i [!UICONTROL &quot;Starta godkännandeprocess när statusen är inställd på&quot;]&quot;.

Fönstret ![[!UICONTROL Redigera godkännandeprocess] med statusfältet markerat](assets/admin-fund-approval-processes-3.png)

