---
title: Lägga till grundläggande villkorsstyrd formatering i en visningsaktivitet
description: Öva dig att lägga till grundläggande villkorsstyrd formatering till vyer, med stegvisa instruktioner.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8855
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Lägga till grundläggande villkorsstyrd formatering i en visningsaktivitet

Öva dig att lägga till grundläggande villkorsstyrd formatering till vyer, med stegvisa instruktioner.

## Sammanfattning

Så här skapar du villkorlig formatering:

1. Välj den kolumn där du vill att formateringen ska visas
1. Bestäm vilka villkor du vill att formateringen ska ändras
1. Bestäm vilken typ av formateringsändring som fungerar bäst

   * bakgrundsfärg
   * textfärg
   * ersättningstext
   * visa en ikon

## Aktivitet 1: Lägga till villkorsstyrd formatering i en vy

Skapa en uppgiftsvy med namnet &quot;Standard + Progress&quot; genom att använda den befintliga standardvyn och lägga till den här villkorsstyrda formateringen i kolumnen [!UICONTROL Name].

1. Lägg till en kolumnregel som ändrar fältets bakgrund till rött när aktivitetens förloppsstatus är Sent.
1. Lägg till en kolumnregel som ändrar fältets bakgrundsfärg till gult när förloppsstatusen är Bakom eller Vid risk.

Detta hjälper dig att hitta problematiska uppgifter utan att inkludera kolumnen för förloppsstatus som en del av vyn.

## Svar 1

![En bild av skärmen för att skapa en ny kolumnregel](assets/conditional-formatting-exercise.png)

1. I en uppgiftslistrapport går du till listrutan **[!UICONTROL Visa]** och väljer **[!UICONTROL Ny vy]**.
1. Ge din vy namnet&quot;Standard + Progress&quot;.
1. Använd de standardkolumner som anges.
1. Markera kolumnen [!UICONTROL Aktivitetsnamn]. Det här är kolumnen som du vill använda villkorsstyrd formatering på, så den visas som röd eller gul om aktivitetens förloppsstatus inte är I tid.
1. Klicka på **[!UICONTROL Avancerade alternativ]** i det övre högra hörnet i rapportbyggarfönstret.
1. Klicka på **[!UICONTROL Lägg till en regel för kolumnen]**.
1. Starta kolumnregeln genom att ändra [!UICONTROL Aktivitet] > [!UICONTROL Namn] överst i fönstret till [!UICONTROL Aktivitet] > [!UICONTROL Förloppsstatus]. Klicka bara på ikonen **[!UICONTROL X]** bredvid [!UICONTROL Aktivitet] > [!UICONTROL Namn] för att ta bort den från fältet.
1. Skriv progress i fältet och välj sedan [!UICONTROL Progress Status] under fältkällan [!UICONTROL Task].
1. Välj **[!UICONTROL Sena]** i fältet till höger om kvalificeraren [!UICONTROL Jämn].
1. Välj en röd bakgrund i raden [!UICONTROL Textfärg].
1. Klicka på **[!UICONTROL Lägg till regel]** för att spara kolumnregeln.
1. Klicka nu på **[!UICONTROL Lägg till kolumnregel]** igen om du vill lägga till en annan regel.
1. Precis som tidigare tar du bort [!UICONTROL Aktivitet] > [!UICONTROL Namn] från villkorsfältet. Ersätt den med [!UICONTROL Förloppsstatus] under fältkällan [!UICONTROL Aktivitet].
1. Markera både [!UICONTROL Vid risk] och [!UICONTROL Bakom] i fältet till höger om kvalificeraren.
1. Välj en gul bakgrund på raden [!UICONTROL Textfärg].
1. Klicka på **[!UICONTROL Lägg till regel]** för att spara kolumnregeln.
1. Klicka på **[!UICONTROL Spara vy]** för att spara vyn.
