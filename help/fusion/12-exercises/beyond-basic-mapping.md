---
title: Bortom grundläggande mappning
description: Lär dig hur du använder mappningspanelens formler för att ändra eller konvertera fält som skickas till en modul.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,noCatalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Bortom grundläggande mappning

Lär dig hur du använder mappningspanelens formler för att ändra eller konvertera fält som skickas till en modul.

## Översikt över övningar

Ändra projektnamn, planerat startdatum och prioritet från genomgången av Beyond Basic Mapping med hjälp av mappningspanelens formler.

![Bortom grundläggande mappningsbild 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Steg som ska följas

**Gör en klon av ditt designscenario för första scenario.**

1. Välj alternativet Klona till höger om den inledande scenariodesignen i scenarioavsnittet, som visas nedan. Ge den namnet&quot;Bortom grundläggande mappning&quot;.

   ![Bortom grundläggande mappningsbild 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Nu ska vi använda mappningspanelen i modulen Skapa Workfront-projekt för att konfigurera projektnamn, planerat startdatum och prioritetsfält.**

1. Klicka på modulen Skapa Workfront-projekt för att redigera inställningarna. Använd mappningspanelen och ändra fältet Namn till [Mitt projektnamn] av [Sponsorn].

   + [Mitt projektnamn] är kolumn 1 från CSV-modulen Parse och [Sponsorn] är kolumn 6. Ordet &quot;by&quot; skrivs precis mellan de två.

1. Gå sedan till planerat startdatum och använd formeln addDays för att lägga till 15 dagar i fältet, vilket beskrivs i Beyond basic mapping-genomgången.
1. Hitta fältet Prioritet och växla knappen Karta längst upp till höger i fältet. Menyn med en lista ändras till ett tal. Skapa en if-programsats för att ge ett projekt etiketten High(4)-prioritet om CSV-filens konfidensgrad är mindre än 100, annars kan den vara Normal(2).

   + Konfidensklassificeringen anges i kolumn 4.

   **Mappningspanelen bör nu se ut så här:**

   ![Bortom grundläggande mappningsbild 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Klicka på OK och sedan på Kör en gång.
1. Hitta projektet i din Workfront-instans för att se till att allt är korrekt mappat.
1. Spara ditt scenario.
