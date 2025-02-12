---
title: Genomgång av avancerad aggregering
description: Lär dig hur du anropar en webbtjänst för att returnera information om flera länder och identifiera populationer, grupperade efter underregion, allt i  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Genomgång av avancerad aggregering

Ring en webbtjänst för att returnera information om flera länder och identifiera den totala befolkningen i alla länder, grupperade efter underregion.

![En bild av Fusion-scenariot](assets/iteration-and-aggregation-3.png)

## Genomgång av avancerad aggregering

Workfront rekommenderar att du tittar på genomgången av videon innan du försöker återskapa övningen i din egen miljö.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops)

## URL för övning

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Förstärkning av aggregationsprincipen

Varje gång en modul matar ut flera paket kommer varje modul därefter att köra varje paket.

Du kan förhindra detta genom att lägga till en aggregator efter en modul som kan generera flera paket.

Du ser en skugga runt ett segment i ditt scenario från en **inledande iterator** till den **avslutande aggregatorn**. Detta gör det enklare att hitta dessa segment i ditt Workfront Fusion-scenario.

## Din tur

>[!NOTE]
>
>Praktiska övningar och utmaningar är frivilliga och behövs inte för att slutföra Fusion-utbildningen.

Denna övning bygger på vad du lärde dig under genomgången, men lösningen tillhandahålls inte.

Skapa ett nytt scenario för att summera alla timmars inloggade uppgifter i projekt i marknadsföringsportföljen. Skicka sedan ett e-postmeddelande som säger&quot;Ditt {Project Name}-projektteam har loggat {summerat timmar} av det totala antalet planerade timmar, vilket anger {percentage} av planen.&quot;

**Utmaning:** Se om du kan göra samma sak men bara för timmar som loggats i år.

## Vill du veta mer? Vi rekommenderar följande:

[Workfront Fusion-dokumentation](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
