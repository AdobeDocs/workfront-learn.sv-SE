---
title: Skapa OR-programsatser i filter
description: Med Workfront flexibla filterlogik kan man förfina rapportvyer med standardreglerna"AND", valfria"OR"-villkor och ordnade filtergrupper för komplexa kriterier.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Skapa OR-programsatser i filter

I videon förklaras hur du skapar och använder filter med flera regler i Workfront. &#x200B; Som standard använder Workfront&quot;AND&quot; mellan filterregler, vilket innebär att alla villkor måste vara true för att ett objekt ska kunna visas i listan.
Du kan också ändra filterlogiken till &quot;OR&quot;, som visar objekt som uppfyller något av villkoren.
I videon visas även hur du skapar filter för åtgärder med filtergrupper. &#x200B; Du kan till exempel skapa två grupper: en för ofullständiga uppgifter som tilldelats det kreativa teamet som är sena och en annan för ofullständiga uppgifter som tilldelats det kreativa teamet som inte är tilldelade. &#x200B; Inom varje grupp gäller&quot;AND&quot;-logik, vilket innebär att alla villkor i gruppen måste vara uppfyllda. &#x200B; Logiken&quot;OR&quot; mellan grupper säkerställer att uppgifter som uppfyller villkoren för någon av grupperna visas.

>[!VIDEO](https://video.tv.adobe.com/v/3470697/?quality=12&learn=on&captions=swe)

## OR-filteraktivitet

Du vill söka efter ofullständiga uppgifter som har tilldelats dig eller som inte har tilldelats någon. Du konfigurerar ett filter så att det ser ut som det nedan. Ger det här filtret de resultat du vill ha? Varför eller varför inte?

![En bild av en felaktigt skapad OR-programsats i [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Svar

Nej, det här filtret ger inte de resultat du vill ha - aktiviteter som inte är färdiga och som antingen är tilldelade till dig eller tilldelade till ingen - eftersom filterregeln för uppgiftens fullständighet bara finns på en sida av ELLER.

Filtret genererar i stället en lista som visar:

* Uppgifter som du tilldelats och som inte är fullständiga.
* **PLUS (ELLER)**
* Alla ej tilldelade uppgifter, oavsett status.

Filtret ska se ut som det nedan. Observera att det här filtret har filterregeln för slutförande av uppgifter på båda sidor om OR.

![En bild av en korrekt skapad OR-programsats i [!DNL Workfront]](assets/or-statement-your-turn-2.png)
