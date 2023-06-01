---
title: Bevis på roller och e-postaviseringar
description: Lär dig hur du aktiverar korrekta korrekturroller och e-postvarningar så att korrekturmottagare har tillgång till korrektur och kan se vad som görs i [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Bevis på roller och e-postaviseringar

Korrekturroller och e-postvarningar hjälper till att driva korrekturarbetsflödet framåt och se till att mottagarna har rätt åtkomst till korrektur och har insyn i det arbete som utförs.

Låt oss titta på några grundläggande bevis:

* **Korrekturroll —** Definierar vad en användare kan göra med ett korrektur (t.ex. kommentarer, markeringar, godkännanden osv.).
* **E-postavisering —** E-postmeddelanden skickas till personer i korrekturarbetsflödet när det finns en aktivitet på korrekturet.

![En bild av [!UICONTROL Nytt korrektur] fönster med [!UICONTROL Korrekturroll] och [!UICONTROL E-postaviseringar] kolumner markerade.](assets/proof-roles-and-email-alerts.png)

Din systemadministratör kan ange standardkorrekturroller och e-postaviseringar för korrekturanvändare i din organisation. Den här informationen kan dessutom byggas in i korrekturarbetsflödesmallar (kallas även automatiska arbetsflödesmallar).

Det kan dock finnas tillfällen när du behöver ange den här informationen manuellt när du överför ett korrektur.

[!DNL Workfront] ger följande allmänna rekommendationer när du tilldelar korrekturroller till korrekturmottagare:

* **Granskare och godkännare —** Dessa användare kan både kommentera korrektur och fatta ett beslut (som godkänt eller avvisat) om ett bevis. Använd den här korrekturrollen för viktiga interna och externa intressenter i granskningsprocessen.
* **Granskare —** Vissa personer i korrekturarbetsflödet behöver bara göra kommentarer. Den här rollen passar dem perfekt. Granskarrollen kan även tilldelas till [!DNL Workfront] användare som i första hand överför korrektur eller fungerar som en korrekturägare, men i övrigt inte är en del av korrekturprocessen.
* **Skrivskyddad —** Perfekt för mottagare som bara behöver se beviset. [!UICONTROL Skrivskyddad] ger åtkomst till vyn och tillåter inte kommentarer.

[!DNL Workfront] ger följande allmänna rekommendationer när du tilldelar e-postvarningar till korrekturmottagare:

* **Slutligt beslut -** Detta skickar ett e-postmeddelande när den sista personen fattar ett beslut om beviset. Tilldela detta till personen som övervakar korrekturarbetsflödet. Detta kan vara en korrekturansvarig, en korrekturläsare, en korrekturläsare, en projektledare eller någon annan [!DNL Workfront] användare. [!DNL Workfront] rekommenderar den här varningen när du använder ett grundläggande arbetsflöde, så att personen som övervakar beviset vet att alla beslut har fattats.
* **Beslut —** Detta skickar varningar eftersom varje berörd part i korrekturarbetsflödet fattar beslut om korrekturet. Det här alternativet är bäst när du använder ett automatiserat arbetsflöde, med flera beslut. Tilldela den person som övervakar korrekturarbetsflödet. Detta kan vara en korrekturansvarig, en korrekturläsare, en korrekturläsare, en projektledare eller någon annan [!DNL Workfront] användare.
* **Handikappade -** Använd detta för gästkorrekturläsare för att begränsa antalet e-postmeddelanden som de får om korrekturet. Mottagarna meddelas fortfarande om nya korrektur, nya versioner och försenade korrektur plus [!DNL Workfront] -användare får direktmeddelanden i en korrekturkommentar med @username och gästmottagare med @emailaddress.

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
