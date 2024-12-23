---
title: Byt modulövning
description: Lär dig hur du använder modulen Byt när du behöver utföra mer komplexa eller dynamiska dataomformningar.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
recommendations: noDisplay,catalog
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Byt modulövning

Lär dig hur du använder modulen Byt när du behöver utföra mer komplexa eller dynamiska dataomformningar.

## Översikt över övningar

Sök efter direktmeddelandeprojekt i testenheten och ändra sedan namnet på varje projekt baserat på ett värde som valts i ett anpassat fält som är kopplat till projektet.

![Byt modulbild 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Steg som ska följas

1. Skapa ett nytt scenario och ge det namnet&quot;Använda modulen Byt&quot;.
1. Använd Workfront Search-modulen för utlösarmodulen.
1. Konfigurera din Workfront-anslutning och ange posttypen till Project.
1. I sökvillkoren anger du att du bara vill visa projekt som har ett värde i det anpassade fältet Kanal.
1. För utdata väljer du ID, Namn, Referensnummer och Anpassat fält för kanal.

   ![Byt modulbild 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Lägg till modulen Byt från verktyg.
1. Mappa det anpassade kanalfältet från sökmodulen för fältet Indata.

   ![Byt modulbild 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Därefter läggs fall till för varje möjligt värde som kommer från det anpassade kanalfältet. Det möjliga värdet anges i fältet Mönster. Du vill att utdatafältet ska innehålla en specifik 3-bokstavskod följt av projektets referensnummer och sedan projektets namn.

   **Mappningspanelen ska se ut så här:**

   ![Byt modulbild 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Du kan lägga till så många fler ärenden du vill. Lägg märke till fältet Else längst ned. Detta används om indatavärdet inte matchar något av fallen.

   **Uppdatera projektnamnet i Workfront.**

   ![Byt modulbild 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Lägg till en Workfront Update Record-modul.
1. I fältet ID mappar du till ID:t från utlösarmodulen.
1. Ange Posttyp till Projekt.
1. Markera fältet Namn i avsnittet Välj fält till karta och mappa det till utdata från modulen Byt.
1. Spara ditt scenario och kör en gång. Visa de uppdaterade projektnamnen i testenheten.
