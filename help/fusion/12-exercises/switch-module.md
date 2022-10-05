---
title: Växla modul
description: Lär dig hur du använder modulen Byt när du behöver utföra mer komplexa eller dynamiska dataomformningar.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11052
thumbnail: KT11052.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# Växla modul

Lär dig hur du använder modulen Byt när du behöver utföra mer komplexa eller dynamiska dataomformningar.

## Översikt över övningar

Sök efter direktmeddelandeprojekt i testenheten och ändra sedan namnet på varje projekt baserat på ett värde som valts i ett anpassat fält som är kopplat till projektet.

![Byt modul, bild 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## Steg som ska följas

1. Skapa ett nytt scenario och ge det namnet&quot;Använda modulen Byt&quot;.
1. Använd Workfront Search-modulen för utlösarmodulen.
1. Konfigurera din Workfront-anslutning och ange posttypen till Project.
1. I sökvillkoren anger du att du bara vill visa projekt som har ett värde i det anpassade fältet Kanal.
1. För utdata väljer du ID, Namn, Referensnummer och Anpassat fält för kanal.

   ![Byt modul, bild 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Lägg till modulen Byt från verktyg.
1. Mappa det anpassade kanalfältet från sökmodulen för fältet Indata.

   ![Byt modul, bild 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. Därefter läggs fall till för varje möjligt värde som kommer från det anpassade kanalfältet. Det möjliga värdet anges i fältet Mönster. Du vill att utdatafältet ska innehålla en specifik 3-bokstavskod följt av projektets referensnummer och sedan projektets namn.

   **Mappningspanelen bör se ut så här:**

   ![Byt modul, bild 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Du kan lägga till så många fler ärenden du vill. Lägg märke till fältet Else längst ned. Detta används om indatavärdet inte matchar något av fallen.

   **Uppdatera projektnamnet i Workfront.**

   ![Byt modul, bild 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Lägg till en Workfront Update Record-modul.
1. I fältet ID mappar du till ID:t från utlösarmodulen.
1. Ange Posttyp till Projekt.
1. Markera fältet Namn i avsnittet Välj fält till karta och mappa det till utdata från modulen Byt.
1. Spara ditt scenario och kör en gång. Visa de uppdaterade projektnamnen i testenheten.
