---
title: Utforska körningar, cykler och paket
description: Förstå hur körningar, cykler och paket fungerar med hjälp av körningshistoriken för ett scenario.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Utforska körningar, cykler och paket

Förstå hur körningar, cykler och paket fungerar med hjälp av körningshistoriken för ett scenario.

## Översikt över övningar

Använd olika scenariokonfigurationer för att utforska körningar och cykler.

![Utforska körcykler och paket Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Steg som ska följas

1. Klona scenariot med namnet&quot;Dela variabler mellan routningssökvägar&quot;. Ge det nya scenariot namnet&quot;Dela variabler mellan routningssökvägar - Cycles test&quot;.
1. Ta bort modulen Skicka ett e-postmeddelande eftersom den inte behövs för testet.

   **Ställ in ditt scenario så att 3 cykler bearbetas per körning. Bearbeta 5 projekt i varje cykel.**

1. Klicka på utlösarmodulen och ändra fältet Maximal till 5, så att endast 5 projekt bearbetas i varje cykel.
1. I sökvillkoren tar du bort det andra filtret som begränsar sökningen till ett enda projekt.
1. Klicka på OK.

1. Öppna Scenarioinställningar i verktygsfältet Fusion och ändra fältet Max antal cykler från 1 till 3.
1. Klicka på OK.

   ![Utforska körcykler och paket Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Schemalägg att scenariot ska köras varje minut.**

1. Klicka på klockikonen i utlösarmodulen och ändra fältet Minuter till 1 minut.

   ![Utforska körcykler och paket Bild 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. Växla sedan till På under knappen Kör en gång. Spara ditt scenario.

   ![Utforska körcykler och paket Bild 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Gå till körningshistoriken för scenariot och se när en ny historikpost visas inom nästa minut. Du kan behöva uppdatera sidan.

   ![Utforska körcykler och paket Bild 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Klicka på knappen Detaljer för en körning. Klicka i den enkla loggen på den högra panelen, ungefär som i delen körningshistorik i Workfront Fusion-kursen.
1. Register över bearbetade åtgärder delas in i cykler.

   ![Utforska körcykler och paket Bild 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Med en nedrullningsbar meny längst upp till höger i fönstret kan du välja någon av de tre cykler som du har ställt in för att köras varje gång.

   ![Utforska körcykler och paket Bild 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
