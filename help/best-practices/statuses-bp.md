---
title: God praxis - status
description: Utforska rekommendationer från Adobe Workfront experter om hur man ställer in, hanterar och använder Workfront-status.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# God praxis - status

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för status

* När du byter namn på Workfront standardstatus bör du behålla det ursprungliga syftet med statusen.

* Om du skapar en anpassad projektstatus för Avbrutet, jämför du statusen med Dölj.

* Minimera globala anpassade statusvärden.

* Använd inte projektstatus i stället för uppgifter för att ange ett projekts förlopp.


</br>
</br>



## Varför är detta de bästa sätten?

**Bästa praxis**

När du byter namn på Workfront standardstatus bör du behålla det ursprungliga syftet med statusen.



**Här är varför**

Vissa åtgärder i Workfront aktiveras av systemets standardstatus. Om du ändrar avsikten för en status kan det påverka hur Workfront fungerar i vissa situationer, påverka rapporter osv.



Standardaktivitetsstatusen till Fullständig anger till exempel att Workfront ska ändra procentandelen färdigt för en uppgift till 100 %. Statusen Slutför talar också om för Workfront att arbete med beroende uppgifter kan börja. Om du har ändrat statusnamnet till Väntar, för att ange att ett arbete med en uppgift har pausats, kommer Workfront att tro att uppgiften är klar och starta nästa steg i projektet.

</br>
</br>



**Bästa praxis**

Om du skapar en anpassad projektstatus för Avbrutet, jämför du statusen med Dölj.



**Här är varför**

Om du jämför Avbrutet med Fullständigt kan du inte använda statusen för att avbryta ett projekt om inte alla aktiviteter är markerade som slutförda och alla utgåvor stängs. Om du jämför Avbrutet med Annullerat kan du avbryta projektet utan att ändra något i historikposten.


</br>
</br>

**Bästa praxis**

Minimera globala anpassade statusvärden.



**Här är varför**

Mindre är mer. Förutom att skapa onödigt underhåll skapar för många anpassade statusar förvirring, särskilt när du arbetar med korsfunktionella projekt. Gör i stället en anpassad statusgrupp specifik. På så sätt blir Workfront-miljön renare och bättre lämpad för expansion i andra grupper i framtiden. Samarbeta med era styrnings-/tillsynskommittéer och intressenter för att identifiera vilka statusar era grupper behöver använda.


</br>
</br>

**Bästa praxis**

Använd inte projektstatus i stället för uppgifter för att ange ett projekts förlopp.



**Här är varför**

Håll projektstatus enkel för att indikera högnivåfaser av progression, som Planning, Aktuell, Fullständig osv. Låt uppgifterna, uppgiftsstatusvärdena och procentandelen slutförda uppgifter visa hur arbetet fortskrider generellt i projektet. Dessa indikatorer för aktivitetsnivå räknas in i projektets Procent färdigt, projektvillkoren och projektets förloppsstatus, som alla är bättre och exaktare indikatorer på projektstatus än projektstatus. Dessutom ger den här informationen på aktivitetsnivå bättre projektrapportering.
