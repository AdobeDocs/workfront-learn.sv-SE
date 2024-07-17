---
title: Förstå felhanteringsdirektiv
description: Läs mer om felhanteringsdirektiven som tillåter att körningen fortsätter och de som stoppar körningen i  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,noCatalog
doc-type: video
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Förstå felhanteringsdirektiv

I den här videon får du lära dig:

* De tre felhanterardirektiven som tillåter körning
* De två felhanterardirektiven som stoppar körningen

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## Direktiv - scenariot fortsätter

### Återuppta

* Ett ersättningsutdata anges och skickas till modulen som påträffar ett fel.
* De efterföljande modulerna bearbetas.
* Scenariots körningsstatus är markerad som &quot;success&quot;.

![En bild av ett Återuppta-direktiv](assets/troubleshooting-and-error-handling-2.png)

### Brytning

* Scenario-körningens tillstånd lagras i kön med ofullständiga körningar där felet kan lösas manuellt. Det finns dock vissa undantag som nämns här.
* De efterföljande modulerna bearbetas inte.
* Om det finns obearbetade paket fortsätter scenariokörningen normalt.
* Scenariots körningsstatus är markerad som &quot;varning&quot;.

![En bild av ett Bryt-direktiv](assets/troubleshooting-and-error-handling-3.png)

### Ignorera

* Felet ignoreras och efterföljande moduler bearbetas inte.
* Om det finns obearbetade paket fortsätter scenariokörningen normalt.
* Scenariots körningsstatus är markerad som &quot;success&quot;.

![En bild av direktivet Ignorera](assets/troubleshooting-and-error-handling-4.png)

## Direktiv - Scenariostopp

### Återställning

* Scenariokörningen stoppas omedelbart och en återställningsfas startas på alla moduler i ett försök att återställa alla till deras ursprungliga tillstånd.
* De efterföljande modulerna bearbetas inte.
* Om du utelämnar ett fåtal feltyper inaktiveras scenariot efter det&quot;antal på varandra följande fel&quot; som anges i scenarieinställningarna.
* Scenariots körningsstatus är markerad som &quot;error&quot;.

>[!NOTE]
>
>Detta är standardbeteendet om ingen felhanterarväg är kopplad till modulen och inställningen Tillåt lagring av ofullständiga körningar under scenarieinställningarna inte är markerad.

![En bild av ett återställningsdirektiv](assets/troubleshooting-and-error-handling-5.png)

### Verkställ

* Felet ignoreras och efterföljande moduler bearbetas inte.
* Om det finns obearbetade paket fortsätter scenariokörningen normalt.
* Scenariots körningsstatus är markerad som &quot;success&quot;.

![En bild av ett implementeringsdirektiv](assets/troubleshooting-and-error-handling-6.png)
