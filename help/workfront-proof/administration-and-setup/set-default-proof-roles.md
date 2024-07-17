---
title: Ange standardkorrekturroller
description: Lär dig hur du ställer in standardkorrekturrollen som tilldelas när nya användare skapas eller när andra öppnar ett korrektur.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Ange standardkorrekturroller



Den första standardinställningen som ska slutföras är att fastställa en standardkorrekturroll som tilldelas när nya användare skapas eller personer öppnar ett korrektur.

Korrekturroller avgör vad en användare kan göra med ett korrektur - titta bara på det, kommentera, godkänna det osv. [!DNL Workfront] rekommenderar att du anger standardvärden för korrekturroller för alla användare, så att du kan lägga till mottagare i korrektur och konfigurera arbetsflöden snabbare och enklare.

![Korrekturroller kan väljas vid överföring av ett korrektur](assets/proof-system-setups-proof-role-example.png)

Den här standardkorrekturrollen kan dock ändras när enskilda korrektur överförs, så att alla kan uppfylla den roll som krävs i gransknings- och godkännandeprocessen.


## Ange standardkorrekturroller

1. Välj **Konfigurera** på [!UICONTROL huvudmenyn].
1. Välj **Granska och godkänn** på den vänstra menyn.
1. Klicka på knappen bredvid önskad standardkorrekturroll för både nya [!DNL Workfront]-användare och gästkorrekturanvändare för&quot;angivna mottagare&quot; - alla som har lagts till i korrekturarbetsflödet, antingen manuellt eller via en arbetsflödesmall.
1. Klicka på knappen bredvid önskad standardkorrekturroll för både nya [!DNL Workfront]-användare och gästkorrekturanvändare för icke-mottagare-användare. Dessa är vanligtvis [!DNL Workfront] användare som har åtkomst till ett korrektur men som inte är en av de personer som är tilldelade till arbetsflödet.
1. Spara ändringarna.

![Inställningar för granskning och godkännande i Workfront](assets/proof-system-setups-workfront-defaults.png)

Tänk på vad de flesta användare och gäster förväntas göra när de läggs till i ett korrekturarbetsflöde. Detta bör vara ditt standardvärde.

## Bästa praxis

| Bästa praxis | Här är varför |
|---|---|
| Använd bara Skrivskyddat eller Granskare för inställningen &quot;Roller för icke-mottagare som öppnar ett dokumentkorrektur&quot; i Workfront. | De andra alternativen för den här inställningen kräver att du fattar ett korrekturbeslut, vilket kan leda till att ditt korrekturarbetsflöde försämras. Vanligtvis behöver de som inte läggs till i korrekturarbetsflödet bara visa korrekturet eller göra kommentarer, inte godkänna korrekturet, så skrivskyddet eller granskningsalternativen är det bästa valet. <br> <br>Obs! Den här inställningen finns på Workfront huvudmeny > Inställningar > Granska och godkänn. |
