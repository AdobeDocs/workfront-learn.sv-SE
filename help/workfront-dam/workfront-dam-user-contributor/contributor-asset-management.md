---
title: Hantera resurser i [!UICONTROL Workfront DAM]
description: Lär dig hantera resurser i [!UICONTROL Workfront DAM] för att förbättra arbetsflödet.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Medarbetare: kapitalförvaltning

I den här videon får du lära dig att:

* Använda menyn Redigera för en resurs
* Ange ett förfallodatum
* Visa meddelanden
* Ange inställningar för enskilda meddelanden
* Överföra en resursversion
* Skapa en ny mapp
* Använda en metadatamall i en mapp
* Skapa mappbehörigheter

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## Så här fungerar resursversioner

En del av arbetsflödet kan vara att hantera flera versioner - eller rundor, korrektur, iterationer, vad du än kallar dem - av en resurs. Du kan hantera alla versioner via [!UICONTROL Workfront DAM].

Systemet tillåter automatisk versionskontroll när en fil med samma namn som en befintlig fil överförs till samma mapp. Kontrollera med systemadministratören om den här funktionen har aktiverats.

Om automatisk versionskontroll är aktiverat kommer en resurs endast att versionskontrolleras om den har lästs in i den mapp som innehåller den ursprungliga resursen. Båda resurserna måste ha samma filnamn. Om resursen läses in i en annan mapp läggs resursen in som en ny fil.
Om versionskontroll inte är aktiverat överförs en fil med samma namn som en befintlig fil som en ny fil, oavsett vilken mapp den placeras i. Detta kan leda till att två resurser med samma namn finns i samma mapp.

Du kan också överföra versioner av en viss resurs manuellt. Klicka på redigeringsikonen på resursen och välj sedan **[!UICONTROL Överför ny version]**.

Om du publicerar en resurs med versioner till Brand Connect ser användaren Brand Connect bara den senaste versionen av resursen.

## Mapp- och resursstatus och förfallodatum

Status är ett annat sätt att hantera åtkomst till mappar och resurser i [!UICONTROL Workfront DAM]. Status kan användas för att dölja vissa resurser eller mappar från [!UICONTROL Brand Connect] användare eller för att förfalla en resurs eller mapp så att ingen annan än systemadministratören kan komma åt den.

* **[!UICONTROL Aktiv]**—Används för resurser och mappar. Resurser och mappar med [!UICONTROL Aktiv] status visas för alla användare med behörigheter och kan publiceras till [!UICONTROL Brand Connect]. [!UICONTROL Aktiv] anges med en grön punkt på en resurs eller mapp.
* **[!UICONTROL Inaktiv]**—Används för resurser och mappar. Resurser och mappar med [!UICONTROL Inaktiv] status visas för [!UICONTROL Workfront DAM] -användare, men de syns inte i [!UICONTROL Brand Connect]. [!UICONTROL Inaktiv] anges med en röd punkt på en resurs eller mapp.
* **[!UICONTROL Outgången]**—Används endast för resurser. Det här är standardstatusen för alla resurser. Outgångna resurser som också [!UICONTROL Aktiv] är synliga i [!UICONTROL Brand Connect].
* **[!UICONTROL Utgånget]**—Används endast för resurser. Resurser med [!UICONTROL Utgånget] status kan inte hämtas av någon användare förutom systemadministratören. Utgångna resurser är synliga/inte synliga i [!UICONTROL Brand Connect], beroende på systemkonfigurationer.
