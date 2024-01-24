---
title: Ställ in standardinställningar för korrekturkonto
description: Lär dig hur du ställer in standardkontoinställningar som ska gälla globalt för alla korrekturläsare och korrekturanvändare.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Ställ in standardinställningar för korrekturkonto

Fastställ standardkontoinställningar som gäller globalt för alla korrekturläsare och korrekturanvändare - land, språk och tidszon. Om du har användare över flera tidszoner eller länder kan du justera de här inställningarna för varje persons användarprofil, om det behövs.

![Fönstret Kontoinställningar för korrektur](assets/proof-system-setups-default-account-settings.png)

1. Välj **[!UICONTROL Korrektur]** från [!DNL Workfront's] [!UICONTROL Huvudmeny].
1. Välj **[!UICONTROL Kontoinställningar]** i det övre navigeringsfältet.
1. Välj **[!UICONTROL Information]** -fliken.
1. Gå till [!UICONTROL Land] fält och markera **[!UICONTROL Redigera]**. Välj det land där de flesta av dina korrekturläsaranvändare finns som standard.
1. Välj **[!UICONTROL Spara]** för den inställningen.
1. Gå till [!UICONTROL Standardspråk] fält och markera **[!UICONTROL Redigera]**. Välj det språk som de flesta av dina korrekturanvändare ska använda som standard.
1. Välj **[!UICONTROL Spara]** för den inställningen.
1. Gå till [!UICONTROL Standardvärde för tidszon] fält och markera **[!UICONTROL Redigera]**. Välj den tidszon som de flesta av dina korrekturanvändare ska vara i som standard. Detta är den tidszon som känns igen av korrekturarbetsflöden som ställs in manuellt. Det gäller även korrekturarbetsflödesmallar, men varje mall kan ha en tidszon angiven.
1. Välj **[!UICONTROL Spara]** för den inställningen.

## Bästa praxis


| Bästa praxis | Här är varför |
|---|---|
| Justera inställningarna så att användarna ser deadlines i 12-timmarsformat. | Välj alternativet F j, Y, gi:a i korrekturinställningarna för användare som vill se korrekturtider i AM/PM-format. För områden där en 12-timmarsklocka används är det här ett bra sätt att förtydliga tidsgränsen. <br> <br>Obs! Du hittar den här inställningen genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Användare > och redigera datumformatsfältet för varje användare. |
| Fastställ en standardkorrekturdeadline som en del av systeminställningarna. | När en standardgräns för korrektur har angetts - överföringsdatumet + x antal arbetsdagar - gäller att om den som skapat beviset glömmer att lägga till en deadline, tillämpar Workfront automatiskt denna deadline för varje korrektur som överförts. <br> <br>Obs! Du hittar den här inställningen genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Inställningar > Korrekturinställningar > Deadline (+ arbetsdagar). |
| Dölj alternativet Ej relevant bevisbeslut. | Det här beslutsalternativet orsakar ofta förvirring bland godkännare, eftersom organisationer ofta inte definierar när alternativet Ej relevant ska användas. Alternativet Ej relevant anger vanligtvis att beviset inte är relevant för bevismottagaren och att de inte behöver fatta ett godkänt eller avvisat beslut. Om du väljer Inte relevant kan korrekturarbetsflödet fortsätta.<br> <br>Alternativet Ej relevant behövs inte i de flesta korrekturarbetsflöden.<br> <br>Obs! Den här inställningen finns på Workfront huvudmeny > Korrektur > Kontoinställningar > Beslut. |
| Ändra inte ordningen på alternativen för korrekturval i korrekturinställningarna. | Varje inställning för korrekturval innehåller ett specifikt värde/vikt som, om den beställs på nytt, kan skapa förvirring i dina korrekturkonfigurationer. Beslutsordningen och värde/vikt används som styrkande fasaktiveringsutlösare och vid rapportering.<br> <br>Obs! Den här inställningen finns på Workfront huvudmeny > Korrektur > Kontoinställningar > Beslut. |
| Ange standardvärden för korrekturroller och e-postaviseringar. | Dessa inställningar fylls i automatiskt när du tilldelar ett korrekturarbetsflöde, snabbar upp processen och bidrar till att korrekturarbetsflödena blir enhetliga.<br> <br>Obs! Användarens standardinställningar hittar du genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Användare > och välja den användare som du vill ange standardinställningar för. |
