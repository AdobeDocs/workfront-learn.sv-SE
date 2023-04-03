---
title: Skapa filter med användarbaserade jokertecken
description: Lär dig hur du använder användarbaserade jokertecken och hur du skapar ett filter baserat på den inloggade användaren.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Skapa filter med användarbaserade jokertecken

I den här videon får du lära dig att:

* Förstå varför du använder jokertecken
* Skapa ett filter med ett användarbaserat jokertecken

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>Använd fältkällan och namnet för Tilldelningsanvändare >> ID när du skapar filter som tittar på information om uppgifter eller ärenden.  Det här alternativet söker efter alla användare som har tilldelats uppgiften eller utgåvan, inte bara&quot;ägaren&quot; eller den primära tilldelade personen.

>[!TIP]
>
>Använd $$USER.ID (i stället för ditt namn) även när du skapar filter för dig själv. På så sätt, om någon ser ett filter som du kör och säger&quot;dela det med mig&quot;, är filtret redan konfigurerat så att varje person som använder det ser sin egen information.

>[!TIP]
>
>Du måste alltid använda filtret Likvärdig när du använder användarbaserade jokertecken.

## Aktivitet

Du har lite extra tid den här veckan, så du vill se om det finns någon i ditt team som kan behöva lite hjälp med sina uppdrag. Skapa ett uppgiftsfilter för att hitta uppgifter som förfaller den här veckan och som inte har slutförts.

## Svar

Du är toppen med att hjälpa dina teamkamrater! När filtret är inställt som bilden nedan hittar du uppgifter:

* Detta har inte slutförts (vilket innebär att de inte har en [!UICONTROL Slutförd] status eller status som motsvarar [!UICONTROL Slutförd]).
* I projekt med en [!UICONTROL Aktuell] status (du vill trots allt inte hitta uppgifter för projekt som ännu inte startats);
* som är tilldelade någon i ditt hemteam, enligt Workfront gruppinställningar,
* Och som har ett avslutsdatum någon gång den här veckan (den här regeln använde det fördefinierade datumfiltret för att definiera &quot;den här veckan&quot;).

![En bild av skärmen för att skapa ett aktivitetsfilter med ett användarbaserat jokertecken](assets/user-wildcard-exercise-answer.png)

Du kan behöva lägga till ytterligare filter om du behöver begränsa listan lite till. Du kan till exempel lägga till en filterregel som tittar på ett visst program eller en viss portfölj som teamet arbetar med.
