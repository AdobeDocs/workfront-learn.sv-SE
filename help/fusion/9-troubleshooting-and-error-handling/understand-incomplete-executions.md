---
title: Förstå ofullständiga körningar
description: Lär dig vad ofullständiga körningar är och hur du hanterar ett fel som resulterar i en ofullständig körning i  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Förstå ofullständiga körningar

Ofullständiga körningar kan lagras i Workfront Fusion där de senare kan granskas och lösas. Lär dig utnyttja den här fantastiska funktionen.

I den här videon får du lära dig:

* Vad ofullständiga körningar är
* Så här hanterar du ett fel som resulterar i en ofullständig körning

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## Fel som resulterar i ofullständiga körningar

Det finns flera felkategorier som resulterar i att ofullständiga körningar lagras.

Olika feltyper som tas emot beror på vilka API:er du ansluter till. Felet kan vara ett valideringsfel som uppstår på grund av ofullständiga eller felaktiga data, huvudsakligen på grund av att ett objekt saknas som förväntas för att alla data ska kunna bearbetas genom en modul. Eller så kan felen uppstå om slutmålet inte är tillgängligt på grund av tillfälligt eller långvarigt anslutningsfel (t.ex. vid anslutning till e-post eller fjärr-FTP-server).

Om ett fel inträffar på den första modulen i scenariot avbryts körningen omedelbart och ingen ofullständig körning sparas.

Om ett fel inträffar i någon annan modul och det inte finns någon kopplad felhanterarväg:

* Om feltypen är ConnectionError, RateLimitError, OutOfSpaceError eller ModuleTimeoutError sparas en ofullständig körningspost MED automatiskt återförsök.
* Om feltypen är DataError, InvalidConfigurationError, InvalidAccessTokenError, UnexpectedError, MaxFileSizeExceededError eller MaxResultsExceededError lagras en ofullständig körningspost UTAN autoåterförsök.
* Om feltypen är något annat än ovanstående misslyckas körningen.

## Vill du veta mer? Vi rekommenderar följande:

[Workfront Fusion-dokumentation](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
