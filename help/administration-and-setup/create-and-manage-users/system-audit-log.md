---
title: Förstå systemgranskningsloggen
description: Lär dig hur du använder systemgranskningsloggen för att granska när ändringar gjorts och när objekt ska tas bort.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Förstå systemgranskningsloggen

Systemets granskningslogg är det bästa sättet för systemadministratören att hålla ett öga på vad som händer i [!DNL Workfront]. Tänk på loggen som din källa till sanning för vem som gjorde vad och när.

Gå till granskningsloggen [!UICONTROL Inställningar] i [!UICONTROL Inställningar] område. Som standard visas data från de senaste sju dagarna. Ändra filtervillkoren för att visa data från olika datumintervall.

När en användare utför vissa åtgärder, [!UICONTROL Workfront] sparar dem i [!UICONTROL Granskningsloggar] i [!UICONTROL Inställningar] område.

![[!UICONTROL Loggtyp] nedrullningsbar meny på [!UICONTROL Granskningsloggar] sida in [!UICONTROL Inställningar]](assets/admin-fund-audit-log-1.png)

Varje inspelad eller loggad åtgärd visar:

* Datum och tid för ändringen
* Loggtypen
* Namnet på den användare som slutförde åtgärden
* Objektet
* All information som är associerad med åtgärden
* IP-adressen

![[!UICONTROL Granskningslogg] list](assets/admin-fund-audit-log-2.JPG)

## Exportera granskningsloggen

Genom att exportera granskningsloggdata kan systemadministratörer dela informationen med interna/externa revisorer eller säkerhetsspecialister. Vissa organisationer kräver att vissa loggar sparas för att uppfylla kraven i gällande säkerhetsbestämmelser. Andra behöver den information som importeras till ett säkerhetssystem för analys.

Granskningsloggar kan exporteras i en CSV-fil (kommaavgränsat värde) som kan öppnas i ett kalkylbladsprogram eller en vanlig textredigerare. Exporten är begränsad till 50 000 rader i taget, så använd filtren för att begränsa listan om summan överstiger 50 000.

![[!UICONTROL Exportera] knapp på [!UICONTROL Granskningsloggar] page](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
