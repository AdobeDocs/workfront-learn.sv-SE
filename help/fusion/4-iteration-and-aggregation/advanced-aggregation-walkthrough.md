---
title: Genomgång av avancerad aggregering
description: Lär dig hur du anropar en webbtjänst för att returnera information om flera länder och identifiera populationer, grupperade efter underregion, allt i [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Genomgång av avancerad aggregering

## Översikt

Ring en webbtjänst för att returnera information om flera länder och identifiera den totala befolkningen i alla länder, grupperade efter underregion.

![En bild av Fusion-scenariot](assets/iteration-and-aggregation-3.png)

## Genomgång av avancerad aggregering

Workfront rekommenderar att du tittar på genomgången av videon innan du försöker återskapa övningen i din egen miljö.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## URL för övning

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Om du vill ha stegvisa instruktioner för hur du slutför genomgången går du till [Genomgång av avancerad aggregering](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) träna.

## Förstärkning av aggregationsprincipen

Varje gång en modul matar ut flera paket kommer varje modul därefter att köra varje paket.

Du kan förhindra detta genom att lägga till en aggregator efter en modul som kan generera flera paket.

Du ser en skugga runt ett segment i ditt scenario från en **begynnelseiterator** till **slutaggregator**. Detta gör det enklare att hitta dessa segment i ditt Workfront Fusion-scenario.

## Din tur

>[!NOTE]
>
>Praktiska övningar är frivilliga och är inte nödvändiga för att slutföra Fusion-utbildningen.

Denna övning bygger på vad du lärde dig under genomgången, men lösningen tillhandahålls inte.

Skapa ett nytt scenario för att summera alla timmars inloggade uppgifter i projekt i marknadsföringsportföljen. Skicka sedan ett e-postmeddelande som säger&quot;Ditt {Project Name}-projektteam har loggat {summerat timmar} av det totala antalet planerade timmar, vilket innebär att du har angett till {percentage} av planen.&quot;

**Utmaning:** Se om du kan göra samma sak, men bara i timmar som loggats i år.

## Vill du veta mer? Vi rekommenderar följande:

[Workfront Fusion - dokumentation](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
