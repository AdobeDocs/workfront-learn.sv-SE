---
title: Förstå felhanteringsdirektiv
description: Läs mer om felhanteringsdirektiven som tillåter att körningen fortsätter och de som stoppar körningen i [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Förstå felhanteringsdirektiv

I den här videon får du lära dig:

* De tre felhanterardirektiven som tillåter att körningen fortsätter
* De två felhanterardirektiven som stoppar körningen

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

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

![En bild av ett Break-direktiv](assets/troubleshooting-and-error-handling-3.png)

### Ignorera

* Felet ignoreras och efterföljande moduler bearbetas inte.
* Om det finns obearbetade paket fortsätter scenariokörningen normalt.
* Scenariots körningsstatus är markerad som &quot;success&quot;.

![En bild av ett Ignorera-direktiv](assets/troubleshooting-and-error-handling-4.png)

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
