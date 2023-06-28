---
title: Introduktion till iteratorövning
description: Lär dig att använda appar av iterationstyp och utföra åtgärder på varje informationspaket.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Introduktion till iteratorer

Lär dig att använda appar av iterationstyp och utföra åtgärder på varje informationspaket.

## Översikt över övningar

Titta på ett specifikt projekt i Workfront och titta sedan på alla uppgifter i det projektet. Du använder stegningsverktyget för att räkna antalet uppgifter i projektet. Slutligen använder du variabeln Set för att subtrahera antalet underordnade från Antal öppna ärenden för att skapa ett numeriskt värde för varje aktivitetspaket.

![Introduktion till iteratorer Bild 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Steg som ska följas

**Läs ett projekt och relaterade uppgifter.**

1. Starta ett nytt scenario. Kalla det&quot;Introduktion till iteration&quot;.
1. Välj Workfront som utlösarmodul, Läs en post.
1. Välj Projekt under Posttyp.
1. För Utdata väljer du ID, Namn och Beskrivning.
1. I fältet ID ställer du in projekt-ID:t för projektet Northstar Fashibitors Booth från din testenhetsinstans i Workfront.
1. Byt namn på den här modulen till&quot;Sök efter WF-projekt&quot;.
1. Lägg till en annan Workfront-modul för att läsa uppgifter som hör till det här projektet. Välj modulen Läs relaterade poster.
1. Välj Projekt under Posttyp.
1. För ID för överordnad post väljer du ID i modulen Läs en post.
1. För Samlingar väljer du Åtgärder.
1. För Utdata väljer du ID, Namn, Beskrivning, Antal underordnade, Antal öppna ärenden och Arbete.
1. Byt namn på den här modulen till&quot;Läs projektets uppgifter&quot;.
1. Spara scenariot och klicka sedan på Kör en gång för att visa utdata.

   + Klicka på körningskontrollen så ser du ett paket som indata (projektet) och 28 paket som utdata (åtgärderna).

   **Räkna och bearbeta itererade paket.**

1. Lägg till en annan modul efter Läs relaterade poster. Välj en verktygsmodul för Öka-funktion.

   + Låt fältet Återställ ett värde vara Aldrig och klicka på OK.

1. Byt namn på den här modulen till Antal uppgifter.
1. Lägg till en Set-variabelmodul. Ange variabelnamnet till &quot;Slumpmässig matematik&quot;.
1. I fältet Variabelvärde subtraherar du antalet öppna underordnade från antalet öppna opTasks.

   **Det borde se ut så här:**

   ![Introduktion till iteratorer Bild 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Byt namn på den här modulen till &quot;Slumpmässig matematik&quot;.
1. Spara scenariot och klicka på Kör en gång.

Workfront Fusion utförde 28 exekveringar för varje åtgärd som gjordes i iteratormodulen Läs relaterade poster. Dessa 28 paket kommer att fortsätta att bearbetas i hela scenariot, såvida inte en aggregator läggs till för att stänga slingan.
