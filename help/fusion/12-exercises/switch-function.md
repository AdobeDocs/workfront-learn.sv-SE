---
title: Växlingsfunktion
description: Lär dig hur du använder switchfunktionen med funktionen Switch.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Växlingsfunktion

Lär dig hur du använder switchfunktionen med funktionen Switch.

## Översikt över övningar

För enkla dataändringar använder du funktionen Växla för att omforma ett värde till ett annat inom ett modulfält. I den här övningen ändrar du nyckeln med två bokstäver till det faktiska namnet på projektets förloppsstatus för att skicka i ett e-postmeddelande.

![Byt funktion bild 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Steg som ska följas

1. Klona scenariot med namnet&quot;Dela variabler mellan routningssökvägar&quot;.
1. Ge det nya scenariot namnet&quot;Dela variabler mellan routningssökvägar - växla&quot;.
1. Klicka på utlösarmodulen och lägg till förloppsstatus i utdataavsnittet.
1. Lägg till förloppsstatus i fältet Innehåll i modulen Skicka ett e-postmeddelande.

   + Om du bara mappar över värdet som kommer från modulen Sök finns det en kod med två bokstäver för förloppsstatusen.
   + Om du vill växla koden för det fullständiga namnet för varje möjlig förloppsstatus använder du växlingsfunktionen på fliken Allmänna funktioner.

1. Switchfunktionen använder värdet eller uttrycket Progress Status som en nyckel och returnerar sedan utdatavärdet baserat på den nyckeln.

   + Ett nyckelvärde definieras på den första positionen efter Progress Status (&quot;LT&quot;) med motsvarande utdata definierat på den andra positionen (&quot;Late&quot;).
   + Nästa nyckelvärde definieras på den tredje positionen, med motsvarande utdata definierat på den fjärde positionen, osv., för så många tangenter som önskas.

     ![Byt funktion bild 2](../12-exercises/assets/switch-function-walkthrough-2.png)
