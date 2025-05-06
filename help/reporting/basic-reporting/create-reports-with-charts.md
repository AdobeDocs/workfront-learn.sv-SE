---
title: Skapa rapporter med diagram
description: Diagrammen förbättrar datavisualiseringen genom att organisera datainsikter med hjälp av anpassningsbara filter, grupperingar och staplade kolumnformat, vilket gör analysen tydligare och mer användbar.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
last-substantial-update: 2025-05-06T00:00:00Z
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: c9eb5f9077f1e9ba90d5ebccc9d3b19575667717
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Skapa rapporter med diagram

I videon förklaras hur du använder diagram för att visualisera data effektivt, särskilt för att spåra projektuppgifter. &#x200B; Här visas två typer av rapporter i Workfront:

**Sena aktiviteter efter projektrapport:**

* Börja med en listrapport och använd filter för att visa endast ofullständiga, sena uppgifter i aktuella projekt. &#x200B;
* Gruppera uppgifter efter projektnamn och skapa ett cirkeldiagram för att visualisera fördelningen av sena uppgifter mellan projekt. &#x200B;
* Ange diagrammet som standardflik för enkel åtkomst. &#x200B;

**Aktiviteter efter projekt och statusrapport för förlopp:**

* Kopiera den första rapporten och lägg till en annan gruppering för status för uppgiftsförloppet.
* Ta bort filter för att inkludera alla uppgifter och visa deras förlopp under projektkörningen.
* Använd ett staplat stapeldiagram för att visa det totala antalet uppgifter per projekt, med stackar som representerar olika förloppsstatusar.
* Anpassa färger vid behov och spara rapporten.

Videon visar hur diagram som cirkeldiagram och skiktade stapeldiagram kan ge insikter om uppgiftsdistribution och projektprestanda, vilket hjälper användarna att jämföra projekt och förstå uppgiftsförloppet visuellt. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Viktiga uppgifter

* **Diagram förbättrar dataskärpan**: Genom att data visas med diagram, till exempel cirkeldiagram och kolumndiagram, blir det enklare att förstå aktivitetsdistribution och projektförlopp jämfört med listrapporter. &#x200B;
* **Filtrering för specifika insikter**: Genom att använda filter (t.ex. ofullständiga, sena aktiviteter i aktuella projekt) kan du fokusera på relevanta data för riktad analys. &#x200B;
* **Gruppering för bättre organisation**: Genom att gruppera uppgifter efter projektnamn eller förloppsstatus ordnas data effektivt, vilket ger meningsfulla jämförelser mellan projekt. &#x200B;
* **Anpassningsalternativ för diagram**: Användare kan välja diagramtyper (t.ex. paj, spalt, fält) och anpassa färger efter inställningar eller varumärke. &#x200B;
* **Staplade stapeldiagram för detaljerade insikter**: Staplade stapeldiagram ger en heltäckande bild av uppgiftsförloppet i projekt, som visar både totala aktiviteter och deras status i en enda visualisering.


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
