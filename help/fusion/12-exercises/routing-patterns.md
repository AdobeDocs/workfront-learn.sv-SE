---
title: Routningsmönster
description: Stärk konceptet med routning och reservvägar utan att behöva använda några andra API:er.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Routningsmönster

Stärk konceptet med routning och reservvägar utan att behöva använda några andra API:er.

## Översikt över övningar

Använd modulen Ange variabel för att skicka ett tal genom flera banor för att se hur filter och reservlösningar fungerar vid routning.

![Routningsmönster Bild 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Steg som ska följas

1. Skapa ett nytt scenario och kalla det&quot;Routningsmönster och reservlösningar&quot;.
1. För utlösaren lägger du till modulen Ange variabel. Skriv&quot;Mitt nummer&quot; som variabelnamn, lämna variabelns livstid som en cykel och ställ in variabelfältet på&quot;75&quot;.

   ![Routningsmönster Bild 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Lägg till en annan modul och välj modulen Router. För båda banorna väljer du verktyget Öka och klickar på OK utan att göra några ändringar för var och en av dem.

   + Skapa ett filter för den första banan, ge den namnet&quot;Mindre än 100&quot; och ange villkoret till [Mitt nummer] Mindre än 100.

   + Skapa ett filter för den andra sökvägen, ge den namnet&quot;Mindre än 1000&quot; och ange villkoret till [Mitt nummer] Mindre än 1000. Se till att du använder operatorn Numerisk för båda.

   ![Routningsmönster Bild 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Routningsmönster Bild 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Klicka på Kör en gång och se hur paketet passerar ned sökvägen&quot;Mindre än 100&quot;.
1. Ändra sedan fältet Ange variabel till 950 och kör en gång till. Se den köra ned den andra banan.
1. Klicka på routern och lägg till en till sökväg. Lägg till funktionsverktygsmodulen Öka. För filtret klickar du på kryssrutan &quot;Resursflöde&quot;. Lägg märke till hur pilen som pekar på den banan ändras till ett cirkumflex, vilket anger att det är reservvägen.

   ![Routningsmönster Bild 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Ändra variabelvärdet Set till 9500 och Run once. Eftersom antalet inte är mindre än 100 eller mindre än 1000, färdas paketet längs reservvägen.

Om du lägger till ytterligare en bana med en stegningsverktygsmodul, men inte anger något filter, vad händer när du klickar på Kör en gång till? Kommer ett paket någonsin att gå ner på reservlinjen med den fjärde rutten tillagd?

+ Nej, eftersom utan ett filter inställt kommer varje paket alltid att gå längs den här vägen i stället för reservvägen.
