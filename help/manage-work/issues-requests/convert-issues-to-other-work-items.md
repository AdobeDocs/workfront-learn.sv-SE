---
title: Konvertera ett problem/en begäran till en uppgift
description: Lär dig hur du konverterar problem till andra arbetsobjekt.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: ce044bb73f980bd7424d3a477a05cef2a8527230
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Konvertera ett problem/en begäran till en uppgift

Ett problem kan vara tillräckligt viktigt för att tiden och arbetet för att lösa det ska räknas med i projekttidslinjen och tilldela lämpliga resurser. I det här fallet kan problemet konverteras till en uppgift.

![En bild av [!UICONTROL Konvertera till aktivitet] option of an issue in [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Navigera till [!UICONTROL Problem] del av projektet eller aktiviteten som problemet är inloggat på. Eller hitta problemet i en rapport som du har tillgång till.
1. Klicka på problemnamnet för att öppna det.
1. Välj **[!UICONTROL Konvertera till uppgift]**.
1. Fyll i [!UICONTROL Konvertera till uppgift] formulär. Börja med att ge den nya aktiviteten ett namn och en beskrivning.
1. Om den nya aktiviteten ska ingå i ett annat projekt anger du projektnamnet.
1. I [!UICONTROL Alternativ] markerar du kryssrutorna för att behålla den ursprungliga utgåvan, tillåta åtkomst till den nya uppgiften och behålla slutdatumet. Följ din organisations arbetsflöde när du gör dessa val.
1. Bifoga ett anpassat formulär om du vill överföra anpassade formulärdata från utgåvan till uppgiften. (Alla fält som finns i både utgivningsformuläret och aktivitetsformuläret överförs automatiskt till aktivitetsformuläret.)
1. Klicka **[!UICONTROL Konvertera till uppgift]** till slut.

![En bild av [!UICONTROL Konvertera till aktivitet] form av en emission i [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

Beroende på din organisations [!DNL Workfront] systeminställningarna kan du ändra inställningarna i avsnittet Alternativ när du konverterar uppgiften. Dessa alternativ påverkar både den ursprungliga utgåvan och den nya aktiviteten.

* **&quot;Behåll det ursprungliga problemet och knyt lösningen till detta&quot;** bevarar den ursprungliga utgåvan och tillhörande information (timmar, dokument osv.). När det här alternativet är markerat markeras problemet som löst när aktiviteten är slutförd. Om det här alternativet är **not** markerat tas den ursprungliga utgåvan bort när uppgiften skapas. Detta kan påverka hur organisationen spårar och rapporterar problem.
* The **&quot;Tillåt (användarens namn) att ha åtkomst till den här uppgiften&quot;** kan den person som skapade problemet få åtkomst till den nya uppgiften.
* The **&quot;Behåll det planerade datumet för färdigställandet av utgåvan&quot;** kan du behålla det planerade slutförandedatumet som redan har angetts för problemet. Detta ställer in aktivitetsbegränsningen till [!UICONTROL Avsluta senast]. Om rutan inte är markerad ställs aktivitetens datum in som om en ny uppgift skapades i projektet.

Den nya uppgiften placeras längst ned i uppgiftslistan i ditt projekt. Flytta aktiviteten till önskad plats, tilldela en användare eller grupp till arbetet, lägg till planerade timmar och varaktighet osv.

>[!NOTE]
>
>Du kan inte lägga till problem i projekttidslinjen eftersom de representerar&quot;oplanerat arbete&quot;. Projektets tidslinje är för&quot;planerat arbete&quot;, dvs. uppgifter.


