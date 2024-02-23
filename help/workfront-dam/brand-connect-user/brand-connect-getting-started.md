---
title: Förstå navigering och sökning som användare
description: Läs om vad varumärket ansluter till [!UICONTROL WORKFRONT DAM] och navigera.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8984
exl-id: 6a7350cf-c9e3-4af6-a1bf-0f159e8eaf09
doc-type: video
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Förstå navigering och sökning som användare

I den här videon får du lära dig:

* Vad du ser när du loggar in
* Navigera till Brand Connect
* Söka efter resurser

>[!VIDEO](https://video.tv.adobe.com/v/335246/?quality=12&learn=on)

## Grundläggande sökvillkor

En grundläggande sökning söker efter filnamn, metadatafält, nyckelord och resursinnehåll (beroende på resurstyp). Den innehåller inte mappnamn.

De flesta sökresultat är exakta träffar. Ett undantag från den här&quot;exakta matchningsregeln&quot; är när [!UICONTROL Brand Connect] söker i filnamnsfältet. [!UICONTROL Brand Connect] returnerar partiella filnamnsmatchningar i stället för exakta filnamnsmatchningar.

## Avancerad sökning i [!UICONTROL Brand Connect]

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

## Riktlinjer för varumärken

Varumärkesriktlinjer är en uppsättning regler som förklarar hur organisationens varumärke fungerar. Riktlinjerna kallas även varumärkesstandarder, en stilguide, en varumärkesbok eller identitetshandböcker för varumärken och kan omfatta:

* En översikt över ert varumärkes historia, vision, personlighet och ton.
* Att inte använda företagets logotyp.
* Exempel på typsnitt som är godkända för tryck och webben.
* Uppdelningar av företagets primära och sekundära färger.
* Exempel på bildstil och foton som fungerar bra med varumärket.

När du loggat in [!UICONTROL Brand Connect]öppnar du riktlinjerna genom att klicka på Varumärkesriktlinjer i det övre navigeringsfältet.
