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
last-substantial-update: 2025-06-26T00:00:00Z
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 4f82fb7be6bed149036f0218038f927ef57e67f4
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Skapa filter med användarbaserade jokertecken

I den här videon får du lära dig att:

* Förstå varför du använder jokertecken
* Skapa ett filter med ett användarbaserat jokertecken

>[!VIDEO](https://video.tv.adobe.com/v/3464482/?quality=12&learn=on&captions=swe)

>[!TIP]
>
>Använd fältkällan och namnet för Tilldelningsanvändare >> ID när du skapar filter som tittar på information om uppgifter eller ärenden.  Det här alternativet söker efter alla användare som har tilldelats uppgiften eller utgåvan, inte bara&quot;ägaren&quot; eller den primära tilldelade personen.

>[!TIP]
>
>Använd $$USER.ID (i stället för ditt namn) även när du skapar filter för dig själv. På så sätt, om någon ser ett filter som du kör och säger&quot;dela det med mig&quot;, är filtret redan konfigurerat så att varje person som använder det ser sin egen information.

>[!TIP]
>
>Du måste alltid använda filtret Likvärdig när du använder användarbaserade jokertecken.


## Skapa filter med användarbaserade jokertecken

### Aktivitet 1

Du har lite extra tid den här veckan, så du vill se om det finns någon i ditt team som kan behöva lite hjälp med sina uppdrag. Skapa ett uppgiftsfilter för att hitta uppgifter som har tilldelats ditt hemteam och som ska utföras den här veckan och som inte har slutförts än.

### Svar 1

Du är toppen att hjälpa dina lagkamrater! När filtret är inställt som bilden nedan hittar du uppgifter:

* Den har inte slutförts (vilket innebär att de inte har en [!UICONTROL fullständig]-status eller status som motsvarar [!UICONTROL fullständig]);
* De finns i projekt med statusen [!UICONTROL Aktuell] (du vill trots allt inte hitta aktiviteter för projekt som inte har startats än);
* som är tilldelade någon i ditt hemteam, enligt Workfront gruppinställningar,
* Och som har ett avslutsdatum någon gång den här veckan (den här regeln använde det fördefinierade datumfiltret för att definiera &quot;den här veckan&quot;).

![En bild av skärmen för att skapa ett aktivitetsfilter med ett användarbaserat jokertecken](assets/user-wildcard-exercise-answer.png)

Du kan behöva lägga till ytterligare filter om du behöver begränsa listan lite till. Du kan till exempel lägga till en filterregel som tittar på ett visst program eller en viss portfölj som teamet arbetar med.
