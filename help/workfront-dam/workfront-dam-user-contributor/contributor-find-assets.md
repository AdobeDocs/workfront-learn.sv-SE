---
title: Förstå att hitta resurser som medverkande
description: Lär dig hur du söker efter resurser, söker i mappar, effektiviserar sökresultat, använder metadata och nyckelord som sökfilter i [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Förstå att hitta resurser som medverkande

I den här videon får du lära dig att:

* Sök efter resurser
* Sök i mappar
* Effektivisera sökresultaten
* Använd metadata och nyckelord som sökfilter
* Visa mappinformation
* Visa och uppdatera metadata och nyckelord för resurser

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on&enablevpops)

## Grundläggande sökvillkor

En grundläggande sökning söker efter filnamn, metadatafält, nyckelord och resursinnehåll (beroende på resurstyp). Mappnamnet ingår inte.

De flesta sökresultat är exakta träffar. Ett undantag till den här&quot;exakta matchningsregeln&quot; är när [!UICONTROL Workfront DAM] söker igenom filnamnsfältet. [!UICONTROL Workfront DAM] returnerar partiella filnamnsmatchningar, i stället för bara exakta filnamnsmatchningar.

## Användaroperatorer vid sökning

Även om de grundläggande sökfunktionerna ofta hittar de resurser du behöver kan du behöva använda ytterligare sökparametrar då och då.

### Partiella matchningar

Om du vill söka efter en delvis matchning lägger du till en asterisk i söktermen. Asterisken får bara användas i slutet av ett ord.

### AND-operator

Om du vill söka efter resultat som innehåller flera söktermer anger du OCH mellan orden. Orden kan hittas i valfri ordning. När du söker i alla fält kanske båda orden inte finns i samma fält. Paris AND Tower hittar till exempel resurser som har båda dessa ord i något av fälten.

### OR-operator

Använd operatorn OR för att hitta resurser som innehåller någon av söktermerna. Exempel: Paris ELLER Arc hittar resurser som har något av orden, men inte nödvändigtvis båda.

### Fras

Om du vill hitta en exakt fras använder du citattecken runt ordet. Alla ord kommer att hittas tillsammans och i ordning. &quot;Eiffeltornet&quot; hittar till exempel orden i exakt den ordningen.

### Negativ operator

Om du vill utesluta ett ord från sökresultatet placerar du ett minustecken (-) framför ordet. Se till att det inte finns något mellanslag mellan minustecknet och ordet. Om du till exempel vill utesluta resurser som har ordet&quot;torn&quot; i metadata, kan sökningen konfigureras som Paris -tower.

### Tom fältoperator

Om du vill söka efter resurser som inte har någon information i ett specifikt metadatafält anger du det fält du vill söka i i det här formatet: ?[xxxxx]. Om du till exempel vill söka efter resurser som inte har tilldelats nyckelord anger du ?[nyckelord] i sökfältet.
