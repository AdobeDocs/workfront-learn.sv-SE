---
title: Konfigurera händelseaviseringar
description: Lär dig hur du styr vilka e-post- och appmeddelanden som användare får genom att hantera händelsemeddelanden.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Ställ in händelsemeddelanden

>[!NOTE]
>
>På grund av en fasad utrullning är funktionen som tillåter system- och gruppadministratörer att hantera händelsemeddelanden tillfälligt inte tillgänglig för vissa [!DNL Workfront]-kunder. Följ den här artikeln för att få uppdateringar om releasen: Lås upp konfigurationen av händelsemeddelanden för grupper.

Systemadministratörer avgör vilka meddelanden användare ska få via [!DNL Workfront].

![[!UICONTROL E-postmeddelanden] i [!UICONTROL inställningsområdet]](assets/admin-fund-notifications-1.png)

Listan [!UICONTROL Händelsemeddelanden] är grupperad efter typ. För varje händelsemeddelande visas fem informationsdelar:

* **[!UICONTROL Aktiv] —** Med kolumnen [!UICONTROL Aktiv] kan du aktivera eller inaktivera ett meddelande på systemnivå.
* **[!UICONTROL Namn] —** Detta är namnet på meddelandet i [!DNL Workfront].
* **[!UICONTROL Beskrivning] —** Beskrivningen innehåller en kort förklaring av vilken åtgärd som har vidtagits för att utlösa ett meddelande eller som behöver vidtas som svar på att ett meddelande tas emot.
* **[!UICONTROL E-postämne] —** Vad visas för användaren på ämnesraden när e-postmeddelandet skickas till användarna.
* **[!UICONTROL Gruppåtkomst] —** Lås upp meddelanden så att de kan hanteras av gruppadministratörer.

## Aktivera meddelanden

Om du vill hantera meddelanden på global systemnivå ska du kontrollera att sökfältet säger [!UICONTROL Systemhändelsemeddelanden].

Aktivera ett specifikt meddelande för att göra det tillgängligt för alla användare genom att klicka på växlingsknappen så att det blå visas. Om det blå är dolt är meddelandet inaktiverat.

![[!UICONTROL Aktiv] kolumn på [!UICONTROL E-postmeddelanden] sida ](assets/admin-fund-notifications-2.png)

När ett händelsemeddelande är aktiverat skickas meddelanden direkt när händelsen inträffar.

## Tillåt gruppadministratörskontroll

Gruppadministratörer kan få tillstånd av systemadministratörer att anpassa meddelandelistan ytterligare baserat på hur deras grupper och undergrupper fungerar och vilka arbetsflöden de har.

![[!UICONTROL Gruppåtkomst], kolumn på [!UICONTROL E-postmeddelanden], sida ](assets/ganotifications_01.png)

För att gruppadministratörer ska kunna hantera meddelanden för sina grupper och undergrupper måste meddelanden på systemnivå låsas upp.

* Gå till fliken Händelsemeddelanden på sidan E-postmeddelanden.

* Kontrollera att sökfältet innehåller systemhändelsemeddelanden.

* Lås upp ett meddelande för alla gruppadministratörer genom att klicka på växlingsknappen i kolumnen Gruppåtkomst så att det blå visas.

* Lås upp flera meddelanden samtidigt genom att markera kryssrutan till vänster om varje meddelande och klicka på upplåsningsikonen i verktygsfältet ovanför listan.

![[!UICONTROL Gruppåtkomst], kolumn på [!UICONTROL E-postmeddelanden], sida ](assets/ganotifications_02.png)

Lås ett olåst meddelande genom att klicka på växlingsknappen så att den grå visas. Lås flera meddelanden samtidigt genom att markera kryssrutorna och klicka på upplåsningsikonen i verktygsfältet.

![[!UICONTROL Gruppåtkomst], kolumn på [!UICONTROL E-postmeddelanden], sida ](assets/ganotifications_03.png)

Olåsta meddelanden visas för gruppadministratörer på den översta nivån för att avgöra om meddelandet behövs för deras grupper och undergrupper. Undergrupper ärver meddelandekonfigurationerna från den översta överordnade gruppen. ﻿


## Hantera gruppmeddelanden

När systemadministratören har olåst meddelandealternativ kan gruppadministratörerna hantera en grupps meddelanden från den enskilda gruppsidan genom att klicka på Händelsemeddelanden på den vänstra panelmenyn. Sedan kan du aktivera eller inaktivera meddelandealternativ.

![[!UICONTROL Gruppåtkomst], kolumn på [!UICONTROL E-postmeddelanden], sida ](assets/managegroupnotifications_01.png)

Vid behov kan systemadministratörer hantera en grupps meddelanden från meddelandesidan genom att ange gruppnamnet i sökfältet högst upp i fönstret.

![[!UICONTROL Gruppåtkomst], kolumn på [!UICONTROL E-postmeddelanden], sida ](assets/managegroupnotifications_02.png)

## Proffstips

Det finns vissa meddelanden som [!DNL Workfront] rekommenderar att du gör tillgängliga för dina användare.

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
--->
