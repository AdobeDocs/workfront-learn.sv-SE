---
title: Filter
description: Lär dig hur du använder filtret mellan moduler för att bara tillåta vissa typer av paket genom.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Filter

Lär dig hur du använder filtret mellan moduler för att bara tillåta vissa typer av paket genom.

## Översikt över övningar

Lägg till ett filter mellan de två modulerna i Beyond Basic-mappningsscenariot för att endast skapa projekt som har en röd projektfärg i CSV-filen.

![Filterbild 1](../12-exercises/assets/filters-walkthrough-1.png)

## Steg som ska följas

1. Skapa en klon av scenariot&quot;Beyond basic mapping&quot; och ge det namnet&quot;Using the mäktige filter&quot;.

   **Lägg till ett filter före modulen Skapa Workfront-projekt så att endast röda projekt kan skapas.**

   ![Filterbild 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Lägg till ett filter genom att klicka på den prickade linjen som förbinder modulerna eller klicka på skiftnyckeln och välja Konfigurera ett filter.
1. Använd fältet Etikett för att ge filtret namnet&quot;Endast röda projekt&quot;.
1. Mappa fältet Projektfärg (kolumn 3 i CSV-filen) i fältet Villkor. Välj operatorn Lika med (skiftlägesokänslig) och skriv sedan &quot;red&quot;.
1. Klicka på OK.

   ![Filtrera bild 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Testa filtret och verifiera resultatet.**

1. Klicka på Spara för att spara scenariot och sedan på Kör en gång.
1. Klicka på filtrets körningskontroll för att se hur varje paket granskades av filtret och antingen gick vidare eller inte gick vidare till modulen Skapa Workfront-projekt.

   ![Filterbild 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Hitta de projekt du har skapat i din Workfront-instans.
