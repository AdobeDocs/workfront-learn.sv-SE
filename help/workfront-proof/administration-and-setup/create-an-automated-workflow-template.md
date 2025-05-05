---
title: Skapa en automatiserad arbetsflödesmall
description: Lär dig hur du skapar en automatiserad arbetsflödesmall genom att tilldela korrekturmottagare och ange korrekturtider. Dela sedan mallen med andra användare.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Skapa en automatiserad arbetsflödesmall

I den här videon får du lära dig att:

* Skapa en automatisk arbetsflödesmall för korrektur av [!DNL &#x200B; Workfront]
* Tilldela korrekturmottagare
* Ange en deadline för granskning och godkännandeprocess
* Dela den automatiserade arbetsflödesmallen med andra

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops)

## Aktivera ytterligare steg

Två alternativ för att avgöra när en korrekturarbetsflödesfas ska startas används sällan, om det någonsin ska ske: alternativet [!UICONTROL Datum och tid] och alternativet [!UICONTROL När den föregående scenens deadline passerar].

Det andra alternativet fungerar bara i scenarier där du har en stor grupp granskare och du inte vill vänta på alla. Det är ett slags&quot;jag ger dig en viss tid att slutföra granskningen och sedan förlora din chans&quot;-alternativ. Men även detta kan göra granskningsprocessen långsammare.

Om du använder [!UICONTROL när den föregående scenens deadline passerar] är det viktigt att komma ihåg att du när som helst kan aktivera en scen manuellt om du inte vill vänta på en deadline att passera.

## Bästa praxis

| Bästa praxis | Här är varför |
|---|---|
| Ställ in korrekturförfattarens korrekturroll till Granskare. | Med korrekturrollen som granskare kan du försäkra dig om att den som skapar korrekturet kan göra kommentarer och komma åt kommentarer som andra lämnar. Oftast behöver den som skapar beviset inte fatta beslut om ett bevis som de har överfört. Alla korrekturroller för godkännare, granskare och godkännare, författare eller moderator kräver ett beslut. Om korrekturförfattaren tilldelas en av dessa korrekturroller men aldrig fattar något beslut, kan detta påverka korrekturernas deadlines negativt. |
| Undvik att använda korrekturrollen för godkännare. | Godkännarens korrekturroll tillåter inte användaren att kommentera det här korrekturet. Detta kan leda till att en användare avvisar korrekturet, utan någon förklaring, eftersom han/hon inte kunde göra några kommentarer. Använd korrekturrollen Granskare och godkännare i stället så att användaren kan ge feedback. |
| Undvik e-postaviseringsalternativet Alla aktivitetskorrektur. | Med det här alternativet skickas ett e-postmeddelande med korrektur varje gång något händer med ett korrektur - en kommentar görs, ett svar skickas, ett beslut fattas osv. Mottagaren ser i stort sett korrekturaktiviteten när den utförs.<br><br>För korrekturägare och skapare fungerar e-postvarningen för beslut bäst för korrekturarbetsflöden i flera steg och det slutliga beslutet fungerar bäst för arbetsflöden i en enda fas. I allmänhet kan alla andra anges till Inaktiverat, såvida de inte vill bli informerade om andra personer som gör kommentarer eller fattar beslut (i vilket fall ett av alternativen för att sammanfatta e-post kanske fungerar bäst). |
