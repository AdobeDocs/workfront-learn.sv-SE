---
title: Förstå prestandamått
description: Lär dig hur du använder prestandamätningar - [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) och [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]).
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Förstå prestandamått

Två prestandamått som används av projektledare är [!UICONTROL Performance Index Method] ([!UICONTROL PIM]) och [!UICONTROL Estimate at Completion] ([!UICONTROL EAC]). Standardvärden för hela systemet kan anges i [!DNL Workfront] och tillämpas på nya projekt. [!UICONTROL PIM] kan sedan ändras i enskilda projekt.

**[!UICONTROL PIM]**

Inställningarna för [!UICONTROL PIM] styr hur [!DNL Workfront] beräknar andra resultatmått för projekt, till exempel [!UICONTROL Kostnadsprestandaindex] ([!UICONTROL CPI]), [!UICONTROL Resultatindex för kostnadsschema] ([!UICONTROL CSI]), [!UICONTROL Schemaläggningsprestandaindex] ([!UICONTROL SPI]) och [!UICONTROL  15}Uppskattning vid slutförande] ([!UICONTROL EAC]).

Alternativen för [!UICONTROL PIM] är timbaserade och kostnadsbaserade.

* **Timbaserad** - Workfront använder de planerade timmarna för att beräkna projektets CPI och EAC. Projektets EAC visas i antal timmar.
* **Kostnadsbaserad** - Workfront använder den planerade arbetskostnaden vid beräkning av projektets CPI och EAC. EAC visas som ett valutavärde. När du använder det här alternativet måste du se till att uppgiftstilldelningar (användare och/eller jobbroller) är kopplade till kostnadstariffer.

**[!UICONTROL EAC]**

[!UICONTROL EAC] representerar den beräknade totala kostnaden för aktiviteten eller projektet när den är klar. Alternativen beräknas på projektnivå och summeras från aktiviteter/underaktiviteter.

* **Beräkna på projektnivå** — [!UICONTROL EAC] för den överordnade aktiviteten och projektet bestäms med hjälp av faktiska timmar/faktiska arbetskostnader i [!UICONTROL EAC]-formler. Beräkningen inkluderar faktiska timmar/kostnader och utgifter som lagts till direkt i den överordnade uppgiften eller projektet.
* R **Samla in från aktiviteter/underaktiviteter** — [!UICONTROL EAC] för den överordnade aktiviteten och projektet bestäms genom att lägga till [!UICONTROL EAC] för varje underordnad aktivitet. Den här beräkningen exkluderar faktiska timmar/kostnader som lagts till direkt i en överordnad uppgift eller ett överordnat projekt.

Beräkningarna för [!UICONTROL EAC] visas i [Beräkna beräkning vid slutförande (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Resultatmått: Inställningar**

Så här anger du standardvärden för [!UICONTROL PIM] och [!UICONTROL EAC]:

1. Välj **[!UICONTROL Konfigurera]** på huvudmenyn.
1. Klicka på **[!UICONTROL Projektinställningar]** på den vänstra panelmenyn och klicka sedan på **[!UICONTROL Projekt]**
1. I avsnittet [!UICONTROL Projektstatus] söker du efter [!UICONTROL Resultatindexmetod]. Välj Timbaserad eller Kostnadsbaserad.
1. För [!UICONTROL Uppskattning vid slutförande] väljer du Beräkna på projektnivå eller Samla in uppgifter/underaktiviteter.
1. Klicka på **[!UICONTROL Spara]** längst ned i fönstret.

![En bild av skärmen [!UICONTROL Projektinställningar]](assets/setting-up-finances-1.png)

**Ange [!UICONTROL PIM] för enskilda projekt**

1. Gå till startsidan för ett projekt.
1. Klicka på **[!UICONTROL Projektinformation]** i den vänstra panelen.
1. Öppna avsnittet **[!UICONTROL Ekonomi]**.
1. Dubbelklicka på texten under **[!UICONTROL Resultatindexmetod]** för att redigera den.
1. Välj Timbaserad eller Kostnadsbaserad.
1. Klicka på **[!UICONTROL Spara]** ändringar för att slutföra.

![En bild av skärmen [!UICONTROL Projektinformation]](assets/setting-up-finances-2.png)

[!UICONTROL PIM] kan anges för en projektmall i avsnittet [!UICONTROL Ekonomi] i mallinformationen.
