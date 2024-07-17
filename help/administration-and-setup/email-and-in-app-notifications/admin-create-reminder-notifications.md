---
title: Ställ in påminnelsemeddelanden
description: Lär dig hur du ställer in objektspecifika påminnelsemeddelanden för att tala om för användarna när arbetet ska utföras snart eller när det är försenat.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

# Ställ in påminnelsemeddelanden

Påminnelsemeddelanden skapas av systemadministratörer i området [!UICONTROL Inställningar]. Sedan kan de bifogas och användas av projekt-, uppgifts- och utgivningsägare som påminnelser om när arbetet förfaller inom kort eller förfaller.

Påminnelser är objektspecifika och måste bifogas manuellt till motsvarande arbetsobjekt så att meddelandet kan skickas.

**Skapa ett påminnelsemeddelande**

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Klicka på avsnittet **[!UICONTROL E-post]**.
1. Klicka på avsnittet **[!UICONTROL Meddelanden]**.
1. Klicka på fliken **[!UICONTROL Ny påminnelse]**.
1. Klicka på knappen **[!UICONTROL +Nytt påminnelsemeddelande]**.
1. Välj önskat objekt för listrutan.
1. Fyll i den obligatoriska informationen.
1. Klicka på **[!UICONTROL Spara]**.

![[!UICONTROL Nytt påminnelsemeddelande] fönster](assets/admin-fund-reminder-notification-1.png)

När du ställer in påminnelsen finns det några saker att tänka på:

* **[!UICONTROL Påminnelsemeddelandenamn] —** Det här namnet visas för projektledare när de bifogar en påminnelse till ett objekt. Kontrollera att namnet är koncist men beskrivande.
* **[!UICONTROL Kvalificeringsperiod] —** Antalet timmar, dagar, veckor eller månader före/efter det datum som valts i timingavsnittet.
* **[!UICONTROL Timing] —** Välj om påminnelsen ska skickas före eller efter objektets planerade, planerade eller faktiska start-/slutförandedatum. Alternativen för tidrapporter är relaterade till startdatum, slutdatum eller senaste uppdateringsdatum.
* **[!UICONTROL Villkor] —** Ange villkoren för att kvalificera påminnelsen som ska skickas. Alternativen varierar beroende på den objektspecifika påminnelsen.
* **[!UICONTROL Mottagare] —** Välj vem påminnelsen ska skickas till. Vilka alternativ som är tillgängliga för berörda parter varierar beroende på vilken objekttyp som har valts för påminnelsen.

När påminnelseinställningarna har skapats och sparats är påminnelsemeddelandet tillgängligt för objektägare att använda inom [!DNL Workfront].

## E-postanpassning

Påminnelsemeddelanden använder ett standardformat för e-post och ett standardmeddelande. Om du vill anpassa e-postmeddelandet kan du skapa en mall.

<!---
paragraph above needs a hyperlink to an article
--->

![Nytt fönster för e-postmall](assets/admin-fund-email-customization.png)

<!---
learn more URLs
--->
