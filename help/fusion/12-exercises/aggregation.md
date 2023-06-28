---
title: Aggregering
description: Lär dig sammanställa olika informationspaket till ett enda värde.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Aggregering

Lär dig sammanställa olika informationspaket till ett enda värde.

## Översikt över övningar

Använd scenariot&quot;Introduktion till upprepning&quot; som du skapade i den senaste övningen för att sammanställa de planerade timmarna för varje arbetsuppgift i projektet och skicka ett e-postmeddelande till dig själv med den informationen.

![Sammanställningsbild 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Steg som ska följas

**Lägg till ett filter och SUM de planerade timmarna.**

1. Klona scenariot&quot;Introduktion till upprepning&quot; som du skapade i föregående övning och kalla det&quot;Introduktion till aggregering&quot;.
1. Lägg till ett filter mellan modulen Läs projekt och modulen Antal uppgifter. Ge filtret namnet&quot;Endast arbetsuppgifter&quot;.
1. Ange villkoret till Antal underordnade [Numerisk operator: Lika med] 0.

   ![Sammanställningsbild 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Efter modulen Slumpmässig matematik lägger du till en verktygsmodul för Numerisk aggregator.
1. Ange att projektets uppgifter ska läsas i källmodulen.
1. Ställ in funktionen Aggregate på SUM.
1. Ange värdet i fältet Arbete från modulen Läs projekt.
1. Byt namn på den här modulen till SUM för alla timmar för aktivitetsplanering.

   ![Sammanställningsbild 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Observera skuggan som visar att aggregeringen avslutar iteration.**

   ![Sammanställningsbild 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Skicka ett e-postmeddelande med aggregerade timmar.**

1. Lägg till en Skicka en e-postmodul från e-postappen, efter den numeriska aggregatorn.
1. Skicka e-postmeddelandet till dig själv.
1. Ämnesraden är &quot;Projektinformation&quot;.
1. I fältet Innehåll skriver du&quot;Det finns ett projekt som kallas&quot; [projektnamn] som har ett totalt antal [resultat] planerade timmar.&quot; The &quot;[projektnamn]&quot; tas från modulen Läs en post och &quot;[resultat]&quot; tas från aggregeringsmodulen.

   ![Sammanställningsbild 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Spara och kör en gång. Hitta e-postmeddelandet i din inkorg.

I iteration kan man komma åt de enskilda paketen. Men utanför iterationen går det bara att komma åt aggregerade fält i modulen Skicka ett e-postmeddelande.
