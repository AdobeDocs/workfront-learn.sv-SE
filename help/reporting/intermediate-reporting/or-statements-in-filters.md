---
title: Skapa OR-programsatser i filter
description: Lär dig hur du använder en OR-sats för att tala om för Workfront att du vill se antingen den här ELLER den i din rapport.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# Skapa OR-programsatser i filter

När du skapar ett filter med flera rader med villkor placerar Workfront som standard en AND mellan varje rad. Det innebär att varje resultat i listan när du använder det här filtret uppfyller alla filterregler.

I det här exemplet har vi tre kriterier, eller regler, för ett projektfilter:

1. Projektet måste ha ett planerat slutförandedatum som infaller under den aktuella månaden.
1. Projektet måste finnas i Events Marketing-portföljen.
1. Projektet måste vara ett aktivt projekt, vilket innebär att det måste ha statusen Aktuell.

![En bild på hur du skapar ett filter med AND-programsatser i [!DNL Workfront]](assets/or-statement-1.png)

Projekten i resultatlistan uppfyller alla tre kriterierna, vilket gör att du kan begränsa sökresultaten så att du kan se exakt den information du behöver.

![En bild av en filtrerad lista i [!DNL Workfront]](assets/or-statement-2.png)

Det kan dock finnas tillfällen då du vill att filterresultaten ska uppfylla olika villkor, och det är då OR-programsatser kan vara till hjälp. Med en OR-programsats talar du om för filtret att du vill se saker som matchar någon av dina OR-programsatser i motsats till ALLA dina AND-programsatser.

## Använda OR-programsatser

ELLER-programsatser utökar eller ökar mängden information som filtret hittar, eftersom ett objekt i resultatlistan bara behöver uppfylla en av filterreglerna, inte alla.

Låt oss titta på en enkel ELLER-sats - projekt som du är projektledare (ägare) för ELLER-projekt som du har skapat.

![En bild på hur du skapar ett filter med OR-programsatser i [!DNL Workfront]](assets/or-statement-3.png)

När du har konfigurerat båda filterreglerna klickar du på OCH mellan dem och växlar till OR.

![En bild på hur du skapar ett filter med OR-programsatser i [!DNL Workfront]](assets/or-statement-4.png)

Alternativet ELLER mellan de två filterreglerna utökar sökvillkoren och anger för Workfront att hitta projekt som uppfyller det ena eller det andra av dessa alternativ. Ditt namn finns i projektägarfältet eller du är den person som skapade projektet.

## Flera filterregler med OR-satser

Nu tittar vi på en OR-sats som innehåller flera filterregler på varje sida av OR-satsen. Detta använder samma två regler som tidigare, men lägger till en regel. Projekt måste också ha statusen Aktuell.

![En bild på hur du skapar ett filter med OR-programsatser i [!DNL Workfront]](assets/or-statement-5.png)

Observera att Workfront&quot;grupperade&quot; filterreglerna på varje sida av ELLER (det finns en grå ruta runt dem). Detta innebär att Workfront kör reglerna på varje sida av OR tillsammans och söker efter projekt som uppfyller båda dessa kriterier eftersom de är förenade med AND.

I det här exemplet söker Workfront efter:

* Projekt som har ditt namn i projektägarfältet och som också har statusen Aktuell.
* **PLUS (ELLER)**
* Projekt som du har skapat som också har statusen Aktuell.

Om du placerar regeln &quot;projektstatus är lika med aktuell&quot; på varje sida av ELLER säkerställer du att regeln fungerar tillsammans med de andra reglerna. Den här vanliga regeln kallas ibland för&quot;konstant&quot;.

>[!NOTE]
>
>Du är inte begränsad till en upprepad filterregel på varje sida av OR. Beroende på dina behov kan du ha flera. Workfront rekommenderar att dessa upprepade regler minimeras för att säkerställa att filtret ger de resultat du behöver.

## Vad händer utan den vanliga filterregeln?

Utan de vanliga filterreglerna kanske du inte får de sökresultat du förväntade dig.

Om du till exempel bara placerar regeln &quot;projektstatus är lika med aktuell&quot; på en sida av ELLER, fungerar den bara med de andra filterreglerna i det avsnittet. I bilden nedan ser du att regeln &quot;projektstatus är lika med aktuell&quot; endast finns i det övre avsnittet.

![En bild på hur du skapar ett filter med OR-programsatser i [!DNL Workfront]](assets/or-statement-6.png)

Detta innebär att Workfront söker efter:

* Projekt som har ditt namn i projektägarfältet och har statusen Aktuell.
* **PLUS (ELLER)**
* Alla projekt du har skapat.

Som du ser ger den här filterinställningen dig något annorlunda resultat än filtret med den upprepade filterregeln. Därför är det viktigt att du ser till att filtret är rätt konfigurerat så att du får de resultat du vill ha och behöver.

Du kan inte använda ELLER-programsatser ofta när du skapar filter. Om du gör det kan du minska antalet filter som du behöver skapa. Se bara till att filtren inte returnerar för många resultat - en lång lista kan göra det svårare för användarna att hitta exakt information som behövs.

## OR-filteraktivitet

Du vill söka efter ofullständiga uppgifter som har tilldelats dig eller som inte har tilldelats någon. Du konfigurerar ett filter så att det ser ut som det nedan. Ger det här filtret de resultat du vill ha? Varför eller varför inte?

![En bild av en felaktigt skapad OR-programsats i [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Svar

Nej, det här filtret ger inte de resultat du vill ha - aktiviteter som inte är färdiga och som antingen är tilldelade till dig eller som inte är tilldelade någon - eftersom filterregeln för aktivitetsstatusen bara finns på en sida av ELLER.

Filtret genererar i stället en lista som visar:

* Aktiviteter som har tilldelats dig och som har statusen Pågår eller Nytt.
* **PLUS (ELLER)**
* Alla ej tilldelade uppgifter, oavsett status.

Filtret ska se ut som det nedan. Observera att det här filtret har filterregeln för uppgiftsstatus på båda sidor om OR.

![En bild av en korrekt skapad OR-programsats i [!DNL Workfront]](assets/or-statement-your-turn-2.png)
