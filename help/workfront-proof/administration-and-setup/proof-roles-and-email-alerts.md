---
title: Bevis på roller och e-postaviseringar
description: Lär dig hur du aktiverar korrekta korrekturroller och e-postaviseringar så att korrekturmottagare har tillgång till korrektur och synlighet för det arbete som utförs i  [!DNL &#x200B; Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Bevis på roller och e-postaviseringar

Korrekturroller och e-postvarningar hjälper till att driva korrekturarbetsflödet framåt och se till att mottagarna har rätt åtkomst till korrektur och har insyn i det arbete som utförs.

Låt oss titta på några grundläggande bevis:

* **Korrekturroll -** Definierar vad en användare kan göra med ett korrektur (t.ex. kommentarer, markeringar, godkännanden osv.).
* **E-postavisering -** E-postmeddelanden skickas till personer i korrekturarbetsflödet när det finns aktivitet på korrekturet.

![En bild av fönstret [!UICONTROL Nytt korrektur] med kolumnerna [!UICONTROL Korrekturroll] och [!UICONTROL E-postaviseringar] markerade.](assets/proof-roles-and-email-alerts.png)

Din systemadministratör kan ange standardkorrekturroller och e-postaviseringar för korrekturanvändare i din organisation. Den här informationen kan dessutom byggas in i korrekturarbetsflödesmallar (kallas även automatiska arbetsflödesmallar).

Det kan dock finnas tillfällen när du behöver ange den här informationen manuellt när du överför ett korrektur.

[!DNL Workfront] erbjuder följande allmänna rekommendationer när du tilldelar korrekturroller till korrekturmottagare:

* **Granskare och godkännare -** Dessa användare kan både kommentera korrektur och fatta ett beslut (som godkänt eller avvisat) om ett korrektur. Använd den här korrekturrollen för viktiga interna och externa intressenter i granskningsprocessen.
* **Granskare -** Vissa personer i korrekturarbetsflödet behöver bara göra kommentarer. Den här rollen passar dem perfekt. Granskarrollen kan även tilldelas [!DNL Workfront]-användare som primärt överför korrektur eller fungerar som en korrekturägare, men som annars inte är en del av korrekturprocessen.
* **Skrivskyddad -** Passar perfekt för mottagare som bara behöver se korrekturet. [!UICONTROL Skrivskyddad] ger vyåtkomst och tillåter inte kommentarer.

[!DNL Workfront] ger följande allmänna rekommendationer när du tilldelar e-postaviseringar till korrekturmottagare:

* **Slutligt beslut -** Det här skickar ett e-postmeddelande när den sista personen fattar ett beslut om beviset. Tilldela detta till personen som övervakar korrekturarbetsflödet. Detta kan vara en korrekturhanterare, korrekturägare, korrekturskapare, projektledare eller annan [!DNL Workfront]-användare. [!DNL Workfront] rekommenderar den här varningen när ett grundläggande arbetsflöde används, så att personen som övervakar korrekturet vet att alla beslut har fattats.
* **Beslut —** Detta skickar varningar när varje berörd part i språkarbetsflödet fattar ett beslut om korrekturet. Det här alternativet är bäst när du använder ett automatiserat arbetsflöde, med flera beslut. Tilldela den person som övervakar korrekturarbetsflödet. Detta kan vara en korrekturhanterare, korrekturägare, korrekturskapare, projektledare eller annan [!DNL Workfront]-användare.
* **Inaktiverad -** Använd detta för gästkorrektur för att begränsa antalet e-postmeddelanden som de får om korrekturet. Mottagarna meddelas fortfarande om nya korrektur, nya versioner och försenade korrektur, och [!DNL Workfront] användare får dessutom direktmeddelanden i en korrekturkommentar med @username och gästmottagare med @emailaddress.

## Din tur

1. Logga in på Workfront och skapa användare som ska använda korrektur som du inte har skapat tidigare. Ställ in korrekturbehörighetsprofilen i användarens inställningar utifrån den roll som personen ska spela i korrekturarbetsflöden.
1. För användare som redan har skapats kan du redigera inställningarna för att justera profilvalet för korrekturbehörigheter, om det behövs.
1. Gå till området för korrekturinställningar och gå till fliken Användare. Kontrollera de personliga inställningarna för dina användare - språk, tidszon, datumformat, korrekturroll som standard och e-poststandardvarning. Detta är viktigt om dessa användare skapades innan standardinställningarna för det globala systemet etablerades.

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
