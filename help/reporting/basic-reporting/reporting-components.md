---
title: Förstå rapporteringskomponenter
description: Lär dig grunderna för rapportering och hur de används i ett rapportelement i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: 3310ca62542d2cb596c6fd50a740bae2bb6345f2
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Förstå rapporteringskomponenter

I den här videon får du lära dig:

* De viktigaste komponenterna bakom Workfront rapportering
* Hur dessa komponenter används i ett rapportelement

>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&learn=on)

## Rapporteringskomponenter

[Klicka här](/help/assets/reporting-components.pdf) om du vill hämta en PDF av den här sidan.

![En bild av skärmen för att skapa ett filter](assets/reporting-components-1.png)

**A - Fältkälla**

Alternativen för fältkälla beror på den valda objekttypen. Fältkällan är ofta det objekt i Workfront som en viss del av informationen (kallas fältnamn) tillhör. Ibland är fältkällan densamma som objekttypen.
Fältkällan avgör vilka fältnamn som är tillgängliga.

Exempel: [!UICONTROL Projekt], [!UICONTROL Aktivitet], [!UICONTROL Problem], [!UICONTROL Tilldelad]

**B - Fältnamn**

Fältnamn är information som är tillgänglig om det du har valt som fältkälla.

De kan vara Workfront-fält som du har fyllt i, fält från ett anpassat formulär eller information som Workfront automatiskt hämtar.

Fältnamn styr värdefältalternativen.

Exempel: [!UICONTROL Förloppsstatus], [!UICONTROL Beskrivning], [!UICONTROL Planerat slutförandedatum], anpassade formulärfält

**C - Filterkvalificerare**

Filterkvalificerare minskar antalet möjliga resultat som kan visas under den valda fältkällan och det valda fältnamnet.

De anger hur fältkällan och fältnamnet relaterar till värdefältet.

Exempel: Equal, Contains, Null, Less than

**D - värde**

Värdet är den information som anges i fältet som anges av fältnamnet.

Alternativen för värden bestäms av fältkällan och fältnamnet.

Jokertecken för användare och datum kan användas både i värdet och i friformstext.

Exempel: Nytt, Aktuellt, $$TODAYbw, Beskrivning

>[!TIP]
>
>Mer information om fältnamn i Workfront finns i [ordlistan för Adobe Workfront-terminologi](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=en).

