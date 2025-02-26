---
title: Skapa rapporter med diagram
description: Lär dig hur diagram kan förbättra visualiseringen av data och hur du använder diagramverktyg i Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Skapa rapporter med diagram

I den här videon får du lära dig:

* Hur diagram kan förbättra visualiseringen av data
* Använda Workfront diagramverktyg

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Skapa rapporter med diagram

### Aktivitet 1: Lägg till ett diagram i en rapport

Slutet av kvartalet närmar sig och du vill se hur nyligen slutförda projekt fastnade i budgeten. Skapa en rapport som visar de planerade kostnaderna kontra den faktiska kostnaden för projekt. Du vill bara visa projekt som har slutförts under det senaste kvartalet. Lägg till ett kombinationskolumndiagram med egna färger.

### Svar 1

1. Välj **[!UICONTROL Rapporter]** på **[!UICONTROL Huvudmenyn]**.
1. Klicka på menyn **[!UICONTROL Ny rapport]** och välj **[!UICONTROL Projekt]**.
1. Klicka på **[!UICONTROL Lägg till kolumn]** på fliken **[!UICONTROL Kolumner (Visa)]**.
1. Välj [!UICONTROL Projekt] > [!UICONTROL Planerad kostnad] och sammanfatta den här kolumnen med **[!UICONTROL Summa]**.
1. Klicka på **[!UICONTROL Lägg till kolumn]** igen.
1. Välj [!UICONTROL Projekt] > [!UICONTROL Verklig kostnad] och sammanfatta den här kolumnen med **[!UICONTROL Summa]**.

   ![En bild av skärmen där kolumner läggs till i en rapport](assets/chart-report-columns.png)

1. På fliken **[!UICONTROL Grupperingar]** anger du att rapporten ska grupperas efter [!UICONTROL Projekt] > [!UICONTROL Namn].

   ![En bild av skärmen där grupperingar ska läggas till i en rapport](assets/chart-report-groupings.png)

1. Lägg till två filterregler på fliken **[!UICONTROL Filter]**:

   * [!UICONTROL Projekt] > [!UICONTROL Status motsvarar med] > [!UICONTROL Fullständigt]
   * [!UICONTROL Projekt] >[!UICONTROL  Faktiskt slutförandedatum] > [!UICONTROL Sista kvartalet]

   ![En bild av skärmen där filter ska läggas till i en rapport](assets/chart-report-filters.png)

1. Välj **[!UICONTROL Kolumn]** som diagramtyp på fliken **[!UICONTROL Diagram]**.
1. Välj [!UICONTROL Projekt] > [!UICONTROL Planerad kostnad] för den [!UICONTROL vänstra (Y) axeln].
1. Välj [!UICONTROL Projekt] > [!UICONTROL Namn] för den [!UICONTROL undre (X) axeln].
1. Klicka på knappen **[!UICONTROL Kombinationsdiagram]** och välj [!UICONTROL Projekt] > [!UICONTROL Verklig kostnad] i fältet **[!UICONTROL Värde]**.
1. Klicka på pilen bredvid färgrutan för att ändra färgen [!UICONTROL Faktisk kostnad]. Välj en av färgerna som visas eller klicka på rutan i det nedre högra hörnet för att visa färgpaletten.
1. Klicka på **[!UICONTROL Spara + stäng]**. När du uppmanas att ange ett rapportnamn kallar du det&quot;Planerad kontra faktisk kostnad per projekt slutfört förra kvartalet&quot;.

   ![En bild av skärmen som lägger till ett diagram i en rapport](assets/chart-report-chart.png)
