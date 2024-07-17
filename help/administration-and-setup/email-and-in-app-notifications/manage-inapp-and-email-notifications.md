---
title: Hantera händelsemeddelanden i appar och e-post
description: Lär dig hur användare kan styra vilka aviseringar i appar och e-postmeddelanden de får så att de får relevanta och användbara e-postmeddelanden om deras arbete.
short-description: Läs mer om hur användarna kan styra vilka meddelanden i appen och e-postmeddelanden de får.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10095.jpeg
jira: KT-10095
exl-id: 831646d2-ecf8-4fe6-8d4e-8c5fc233ed56
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 5%

---

# Hantera händelseaviseringar i appar och e-post

E-post är en del av det dagliga arbetslivet och, vissa dagar, är mängden e-post som du får överväldigande. Med [!DNL Workfront] kan systemadministratörer dock se till att alla får relevanta och användbara e-postmeddelanden om arbetet som de är involverade i.

Det finns flera typer av meddelanden som Workfront kan skicka till användare. Vissa av dessa meddelanden styrs på systemnivå och påverkar alla användare. Vissa meddelanden kan ställas in så att e-postmeddelanden genereras direkt i en daglig sammanfattning. Eller stäng av e-postmeddelanden så genereras endast meddelanden inifrån Workfront.

## Händelsemeddelanden

En händelse är till exempel en statusändring, en publicerad kommentar eller en tilldelad händelse och kan utlösa ett meddelande i appen i [!DNL Workfront].

![Meddelandelista](assets/admin-fund-user-notifications-01.png)

Du kan dock bestämma vilka händelser du vill få e-postmeddelanden för genom att markera eller avmarkera alternativen i inställningarna.

Klicka på ditt namn på [!UICONTROL huvudmenyn] om du vill göra ändringarna.

![Användarnamn i [!UICONTROL Huvudmeny]](assets/admin-fund-user-notifications-02.png)

Klicka på [!UICONTROL Redigera] på menyn [!UICONTROL Mer].

![Meny på användarprofilsidan](assets/admin-fund-user-notifications-03.png)

Klicka på [!UICONTROL Meddelanden] i popup-rutan [!UICONTROL Redigera person].

![[!UICONTROL Redigera person] fönster](assets/admin-fund-user-notifications-04.png)

Härifrån kan du bestämma vilka meddelanden du vill få direkt, dagligen eller inte alls. Alla ändringar du gör här är specifika för dig och påverkar inte andra användare i Workfront.

**[!UICONTROL Dagligen]**

Som standard är e-postmeddelanden konfigurerade att skickas direkt. Du kan dock ändra frekvensen för e-postmeddelanden från [!UICONTROL Instant] till [!UICONTROL Daily] och se till att du får den information du behöver, när du vill ha den.

![[!UICONTROL Meddelande] i [!UICONTROL Redigera person]-fönstret](assets/admin-fund-user-notifications-05.png)

Det dagliga alternativet skickar en sammanfattning av dagens händelser i ett e-postmeddelande. Användarna får ett e-postmeddelande för varje gruppering som de ser i avsnittet [!UICONTROL Meddelanden].

Avsnittet [!UICONTROL Information om projekt jag äger] genererar till exempel ett dagligt e-postmeddelande. Avsnittet [!UICONTROL Åtgärd krävs] genererar ett dagligt e-postmeddelande.

![[!UICONTROL Daglig sammandrag]-e-post för [!UICONTROL Information om projekt som jag äger]](assets/admin-fund-user-notifications-06.png)

![[!UICONTROL Daglig sammandrag] e-post för [!UICONTROL Åtgärd krävs]](assets/admin-fund-user-notifications-07.png)

Förutom att välja alternativet för dag anger du en tid för när dessa e-postmeddelanden ska skickas. Beroende på vad som fungerar bäst kan e-postmeddelanden skickas innan du kommer till jobbet på morgonen eller precis innan du går till jobbet.

![[!UICONTROL Email Daily Digest efter] i listrutan [!UICONTROL Redigera person] ](assets/admin-fund-user-notifications-08.png)

**Inte alls**

Det sista alternativet är att inaktivera e-postmeddelanden helt.

![Markerat meddelande inaktiverat i fönstret [!UICONTROL Redigera person]](assets/admin-fund-user-notifications-09.png)

Om du bestämmer dig för att göra detta, tänk på att även om du inte får e-postmeddelanden, så kommer arbetet fortfarande att tilldelas, kommenteras och uppdateras inom [!DNL Workfront]. Genom att stänga av alla meddelanden kan du sakna viktig information som du måste känna till.

Det finns några tillfällen när [!DNL Workfront] har sett användare inaktivera e-postmeddelanden. Om du till exempel gör mer av ditt arbete via mobilappen [!DNL Workfront] kan du inaktivera dina e-postmeddelanden och bara få meddelanden via appen.

Oavsett vilka [!UICONTROL händelsemeddelanden] du bestämmer dig för att ta emot är meddelanden viktiga för att arbetet ska lyckas för organisationens mål.


## Recommendations

Det finns ett par meddelanden som [!DNL Workfront] rekommenderar att du lämnar markerat, oavsett om det gäller ett snabbmeddelande eller en daglig sammanfattning.

För de flesta användare:

* [!UICONTROL En föregångare till en av mina uppgifter har slutförts]
* [!UICONTROL Någon inkluderar mig i en riktad uppdatering]
* [!UICONTROL Någon kommenterar mitt arbetsobjekt]
* [!UICONTROL Förfallodatumet ändras för en aktivitet som jag har tilldelats till]


Särskilt för projektledare:

* [!UICONTROL Ett projekt som jag är på blir aktivt]
* [!UICONTROL Ett projekt som jag äger ligger efter]
* [!UICONTROL Ett problem har lagts till i ett projekt som jag äger]
* [!UICONTROL Milstolpeaktiviteten har slutförts för ett projekt som jag äger]


<!---
learn more URLs
Email notifications
guide: manage your notifications
--->
