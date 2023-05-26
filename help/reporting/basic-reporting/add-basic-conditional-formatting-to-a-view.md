---
title: Lägga till grundläggande villkorsstyrd formatering
description: Lär dig hur du använder kolumnregler för att ändra textfärg, formatering och bakgrundsfärger i en rapport eller vy, baserat på villkor som du anger.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 0ee80dceb8208bd0360fd8c9ab68fb8a73677a9d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Lägga till grundläggande villkorsstyrd formatering i en vy

Villkorsstyrd formatering görs genom att kolumnregler skapas. Med kolumnregler kan du formatera en kolumn på ett specifikt sätt baserat på villkor som du anger.

I den här videon får du lära dig:

* Vilken villkorsstyrd formatering finns i en vy
* Skapa och ändra villkorsstyrd formatering

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## Sammanfattning

Så här skapar du villkorsstyrd formatering:

1. Välj den kolumn där du vill att formateringen ska visas
1. Bestäm vilka villkor du vill att formateringen ska ändras
1. Bestäm vilken typ av formateringsändring som fungerar bäst

   * bakgrundsfärg
   * textfärg
   * ersättningstext
   * visa en ikon

## Aktivitet: Lägga till villkorsstyrd formatering i en vy

Skapa en uppgiftsvy med namnet&quot;Standard + Progress&quot; genom att använda den befintliga standardvyn och lägga till den villkorliga formateringen i [!UICONTROL Namn] kolumn.

1. Lägg till en kolumnregel som ändrar fältets bakgrund till rött när aktivitetens förloppsstatus är Sent.
1. Lägg till en kolumnregel som ändrar fältets bakgrundsfärg till gult när förloppsstatusen är Bakom eller Vid risk.

Detta hjälper dig att hitta problematiska uppgifter utan att inkludera kolumnen för förloppsstatus som en del av vyn.

## Svar

![En bild av skärmen för att skapa en ny kolumnregel](assets/conditional-formatting-exercise.png)

1. Gå till **[!UICONTROL Visa]** nedrullningsbar meny och välj **[!UICONTROL Ny vy]**.
1. Ge din vy namnet&quot;Standard + Progress&quot;.
1. Använd de standardkolumner som anges.
1. Välj [!UICONTROL Aktivitetsnamn] kolumn. Det här är kolumnen som du vill använda villkorsstyrd formatering på, så den visas som röd eller gul om aktivitetens förloppsstatus inte är I tid.
1. Klicka **[!UICONTROL Avancerade alternativ]** i det övre högra hörnet i fönstret för Report builder.
1. Klicka **[!UICONTROL Lägg till en regel för den här kolumnen]**.
1. Starta kolumnregeln genom att ändra [!UICONTROL Uppgift] > [!UICONTROL Namn] längst upp i fönstret till [!UICONTROL Uppgift] > [!UICONTROL Status för förlopp]. Klicka bara på **[!UICONTROL X]** ikon bredvid [!UICONTROL Uppgift] > [!UICONTROL Namn] för att ta bort den från fältet.
1. Skriv&quot;progress&quot; i fältet och välj sedan [!UICONTROL Status för förlopp] under [!UICONTROL Uppgift] fältkälla.
1. Välj **[!UICONTROL Sena]** i fältet till höger om [!UICONTROL Jämn] kvalificerare.
1. Välj en bakgrund med rött i [!UICONTROL Textfärg] rad.
1. Klicka **[!UICONTROL Lägg till regel]** för att spara kolumnregeln.
1. Klicka nu **[!UICONTROL Lägg till kolumnregel]** igen för att lägga till en annan regel.
1. Precis som tidigare, ta bort [!UICONTROL Uppgift] > [!UICONTROL Namn] från villkorsfältet. Ersätt den med [!UICONTROL Status för förlopp] under [!UICONTROL Uppgift] fältkälla.
1. Markera båda [!UICONTROL Risk] och [!UICONTROL Bakom] i fältet till höger om kvalificeraren.
1. Välj en bakgrund med gult i dialogrutan [!UICONTROL Textfärg] rad.
1. Klicka **[!UICONTROL Lägg till regel]** för att spara kolumnregeln.
1. Klicka **[!UICONTROL Spara vy]** för att spara vyn.
