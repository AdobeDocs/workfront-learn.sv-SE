---
title: Sammanställningsövning
description: Lär dig sammanställa olika informationspaket till ett enda värde.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
recommendations: noDisplay,noCatalog
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Sammanställningsövning

Lär dig sammanställa olika informationspaket till ett enda värde.

## Översikt över övningar

Använd scenariot&quot;Introduktion till upprepning&quot; som du skapade i den senaste övningen för att sammanställa de planerade timmarna för varje arbetsuppgift i projektet och skicka ett e-postmeddelande till dig själv med den informationen.

![Sammanställningsbild 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Steg som ska följas

**Lägg till ett filter och SUM de planerade timmarna.**

1. Klona scenariot&quot;Introduktion till upprepning&quot; som du skapade i föregående övning och kalla det&quot;Introduktion till aggregering&quot;.
1. Lägg till ett filter mellan modulen Läs projekt och modulen Antal uppgifter. Ge filtret namnet&quot;Endast arbetsuppgifter&quot;.
1. Ange villkoret till Antal underordnade [Numerisk operator: lika med ] 0.

   ![Sammanställningsbild 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Efter modulen Slumpmässig matematik lägger du till en verktygsmodul för Numerisk aggregator.
1. Ange att projektets uppgifter ska läsas i källmodulen.
1. Ställ in sammanställningsfunktionen på SUM.
1. Ange värdet i fältet Arbete från modulen Läs projekt.
1. Byt namn på den här modulen till SUM för alla timmar för aktivitetsplanering.

   ![Sammanställningsbild 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Observera skuggan som visar att aggregeringen avslutar iterationen.**

   ![Sammanställningsbild 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Skicka ett e-postmeddelande med aggregerade timmar.**

1. Lägg till en Skicka en e-postmodul från e-postappen, efter den numeriska aggregatorn.
1. Skicka mejlet till dig själv.
1. Ämnesraden är &quot;Projektinformation&quot;.
1. Ange&quot;Det finns ett projekt med namnet [projektnamn] i fältet Innehåll som har totalt [resultat] planerade timmar.&quot; [projektnamnet] hämtas från modulen Läs en post och [result] hämtas från aggregeringsmodulen.

   ![Sammanställningsbild 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Spara och kör en gång. Hitta e-postmeddelandet i din inkorg.

I iteration kan man komma åt de enskilda paketen. Men utanför iterationen går det bara att komma åt aggregerade fält i modulen Skicka ett e-postmeddelande.
