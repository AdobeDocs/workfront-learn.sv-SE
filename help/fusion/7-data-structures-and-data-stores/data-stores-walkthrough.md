---
title: Genomgång av datalager
description: Lär dig hur du använder i ett datalager för att synkronisera företagsnamn mellan en lista över företag och Workfront med  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Genomgång av datalager

I den här övningen använder vi ett datalager för att synkronisera företagsnamn mellan en lista över företag och Workfront.

Detta ingår i en enkelriktad synkronisering av företag i Workfront och andra system. Just nu synkroniseras den bara mellan en CSV-fil och Workfront. Men det kommer också att underhålla en tabell i ett datalager som håller reda på Workfront-id:t (WFID) och företags-ID:t i CSV-filen (CID) för varje företag. Detta gör att vi kan göra detta till en dubbelriktad synkronisering någon gång i framtiden.

![En bild av ett Fusion-scenario](assets/data-structures-and-data-stores-2.png)

## Genomgång av datalager

Workfront rekommenderar att du tittar på genomgången av videon innan du försöker återskapa övningen i din egen miljö.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on&enablevpops=1)



## Slutkommentar

Nu när du har lärt dig mer om datastrukturer och datalager kan du fråga dig själv: När ska du använda dem?

Datastrukturer används oftast för serialisering eller tolkning av dataformat som JSON, XML, CSV med flera. Med datastrukturer kan ni styra datastrukturen och till och med validera data. Den vanligaste anledningen till att du använder en datastruktur är att skapa giltiga data som ska skickas till ett API som förväntar sig JSON eller XML. I dessa fall ska du använda JSON- eller XML-appen tillsammans med din datastruktur för att säkerställa att data har rätt format.

Datalager bör bara användas för att lagra beständiga data som behöver vara tillgängliga för mer än en scenariokörning. Du kan t.ex. lagra metadata om den sista posten som bearbetats för avancerad användning, vilket kräver exakt kontroll över bearbetningen.

Datalager är inte utformade för att användas som datalager eller loggning. Datalager är inte tillgängliga utanför Workfront Fusion och de flesta interaktioner med datalager sker via ett Workfront Fusion-scenario. Det är därför inte möjligt att ansluta ett datalager till ett analys- eller rapporteringsverktyg som skulle kunna förväntas för datalager- och loggningsanvändningsfall. Workfront Fusions roll i användningsområden som dessa skulle vara att fylla i ett system som passar för att organisera och lagra data (t.ex. SQL, MariaDB).

## Vill du veta mer? Vi rekommenderar följande:

[Workfront Fusion-dokumentation](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
