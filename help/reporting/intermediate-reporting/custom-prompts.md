---
title: Skapa egna uppmaningar
description: Lär dig vad en anpassad fråga är, hur du skapar en anpassad fråga i textläge och några exempel som du kan använda vid rapportering i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Skapa egna uppmaningar

I den här videon får du lära dig:

* Vad en anpassad fråga är
* Hur man skapar en egen fråga i textläge
* Några exempel som du kan använda i dina rapporter

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12)

## Aktivitet: Skapa egna uppmaningar

1. Skapa en anpassad fråga som visar följande projektstatus i den nedrullningsbara menyn:
   * Planering
   * Aktuell
   * Slutförd
   * Död
1. Ändra uppmaningen för att visa aktuella projekt som förfaller den här månaden.

## Svar

1. Dina anpassade uppmaningar bör se ut ungefär så här och ha följande textläge:

   ![En bild av skärmen för att skapa ett nytt filter i textläge](assets/cp-01.png)

   När du har sparat den anpassade prompten bör den nedrullningsbara menyn se ut så här:

1. Textläget i den anpassade prompten ska se ut så här:

![En bild av skärmen för att skapa ett nytt filter i textläge](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

Listruteetiketten för aktiva uppmaningar bör uppdateras för att återspegla ändringen i koden så här:

![En bild av skärmen för att skapa ett nytt filter i textläge](assets/cp-02a.png)
