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
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# Skapa en automatiserad arbetsflödesmall

I den här videon får du lära dig att:

* Skapa en automatiserad arbetsflödesmall för [!DNL  Workfront] korrektur
* Tilldela korrekturmottagare
* Ange en deadline för granskning och godkännandeprocess
* Dela den automatiserade arbetsflödesmallen med andra

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on)

## Aktivera ytterligare steg

Det finns två sätt att avgöra när ett korrekturarbetsflöde ska starta: [!UICONTROL Datum och tid] och[!UICONTROL När deadline för föregående fas passeras]&quot;.

Det andra alternativet fungerar bara i scenarier där du har en stor grupp granskare och du inte vill vänta på alla. Det är ett slags&quot;jag ger dig en viss tid att slutföra granskningen och sedan förlora din chans&quot;-alternativ. Men även detta kan göra granskningsprocessen långsammare.

Om du använder &quot;[!UICONTROL när den föregående scenens deadline har passerat]&quot; är det viktigt att komma ihåg att du när som helst kan aktivera en scen manuellt om du inte vill vänta på en deadline att passera.

## Bästa praxis

| Bästa praxis | Här är varför |
|---|---|
| Ställ in korrekturförfattarens korrekturroll till Granskare. | Med korrekturrollen som granskare kan du försäkra dig om att den som skapar korrekturet kan göra kommentarer och komma åt kommentarer som andra lämnar. Oftast behöver den som skapar beviset inte fatta beslut om ett bevis som de har överfört. Alla korrekturroller för godkännare, granskare och godkännare, författare eller moderator kräver ett beslut. Om korrekturförfattaren tilldelas en av dessa korrekturroller men aldrig fattar något beslut, kan detta påverka korrekturernas deadlines negativt. |
| Undvik att använda korrekturrollen för godkännare. | Godkännarens korrekturroll tillåter inte användaren att kommentera det här korrekturet. Detta kan leda till att en användare avvisar korrekturet, utan någon förklaring, eftersom han/hon inte kunde göra några kommentarer. Använd korrekturrollen Granskare och godkännare i stället så att användaren kan ge feedback. |
| Undvik e-postaviseringsalternativet Alla aktivitetskorrektur. | Med det här alternativet skickas ett e-postmeddelande med korrektur varje gång något händer med ett korrektur - en kommentar görs, ett svar skickas, ett beslut fattas osv. Mottagaren ser i stort sett korrekturaktiviteten när den utförs.<br><br>För korrekturläsare och skapare fungerar e-postvarningen för beslut bäst för korrekturarbetsflöden i flera steg och det slutliga beslutet fungerar bäst för arbetsflöden i ett enda steg. I allmänhet kan alla andra anges till Inaktiverat, såvida de inte vill bli informerade om andra personer som gör kommentarer eller fattar beslut (i vilket fall ett av alternativen för att sammanfatta e-post kanske fungerar bäst). |
