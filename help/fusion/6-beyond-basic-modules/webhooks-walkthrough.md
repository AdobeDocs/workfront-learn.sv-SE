---
title: Genomgång av webbhooks
description: Lär dig hur du använder en webkrok för att skapa en app för att avgöra om en kund är gammal nog att köpa alkohol, allt i  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Genomgång av webbhooks

Det här scenariot skapar en bekväm butiksapp så att de enkelt kan avgöra om en kund är gammal nog att köpa alkohol eller inte. Kassören behöver bara bokföra kundens namn och födelsedatum OCH en verifierad klienttoken till en angiven URL. När detta anges utlöses vårt scenario för att beräkna det lämpliga svaret och returnera det till den som gjorde begäran.

![En bild som använder växlingsmodulen](assets/beyond-basic-modules-5.png)

## Genomgång av webbhooks

Workfront rekommenderar att du tittar på genomgången av videon innan du försöker återskapa övningen i din egen miljö.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on&enablevpops=1)


## Postman

Om du vill följa med i genomgången måste du ladda ned den kostnadsfria Postman-appen. Följ stegen nedan för att navigera till rätt del av Postman för övningen.

1. Skapa en arbetsyta och öppna den.
1. Klicka på fliken Nytt och skapa en ny samling med namnet Drinking Age.
1. Klicka på fliken Nytt igen och skapa en ny GET-förfrågan med namnet GET födelsedatum.
1. Ändra begäran från GET till POST.
1. Gå till underfliken Brödtext under fältet POST URL.
1. Välj formulärdata under fliken Behörighet.
1. Skapa tre nycklar för Name, Birthdate och clientToken.

![En bild som använder växlingsmodulen](assets/beyond-basic-modules-6.png)

## Din tur

>[!NOTE]
>
>Praktiska övningar och utmaningar är frivilliga och behövs inte för att slutföra Fusion-utbildningen.

Denna övning bygger på vad du lärde dig under genomgången, men lösningen tillhandahålls inte.

Skapa en Workfront-webkrok som väntar på nya uppdateringar och loggar sedan datumet, namnet på den person som gjorde uppdateringen och det som står i uppdateringen. Mejla den här informationen själv.

**Tips**: Använd utlösarmodulen Workfront Watch Events för att skapa din webkrok. Uppdateringar i Workfront kallas också anteckningar.

**Utmaning**: Kan du hitta och lägga till URL:en som uppdateringen gjordes för enkel åtkomst?


## Vill du veta mer? Vi rekommenderar följande:

[Workfront Fusion-dokumentation](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
