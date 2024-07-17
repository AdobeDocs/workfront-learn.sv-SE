---
title: God praxis - scheman
description: Utforska rekommendationer från Adobe Workfront experter om hur man ställer in, hanterar och använder Workfront scheman.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10925
exl-id: 508d6f90-f9f4-4f12-9bf1-5e89246f3e3a
source-git-commit: 214457a95a310920f5f7c623021b5d9d40ec61e8
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# God praxis - scheman

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa praxis är riktlinjer som utgör ett effektivt och effektivt sätt att agera, som enkelt används av dig och användarna på ditt företag och som kan återges framgångsrikt i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för scheman

* Begränsa antalet scheman du skapar i Adobe Workfront.

* Det totala antalet arbetstimmar i schemat för varje arbetsdag ska vara lika med antalet timmar per dag som anges i de globala projektinställningarna.

* Lägg till en påminnelse till Adobe Workfront-systemadministratörens kalender om att uppdatera scheman vid en viss tidpunkt varje år.


Instruktioner om hur du skapar och hanterar scheman finns i självstudiekursen [Skapa och hantera scheman](/help/administration-and-setup/configure-system-defaults/create-and-manage-schedules.md).

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Begränsa antalet scheman du skapar i Adobe Workfront.



**Det här är varför**

Skapa inte dussintals scheman för olika grupper, team eller individer. Färre scheman innebär mindre underhåll av system- eller gruppadministratörer.



Separata scheman kan behövas när:

* Anställda befinner sig i olika tidszoner (i USA och östra USA) eller i olika regioner (EMEA jämfört med APAC).

* Du har deltidsarbetare som arbetar mindre än 40 timmar per vecka.

* Arbetare arbetar inte 8 timmar om dagen, måndag-fredag, som heltidsarbetare eller de som arbetar 4-timmars dagar.

</br>
</br>

**Bästa praxis**

Det totala antalet arbetstimmar i schemat för varje arbetsdag ska vara lika med antalet timmar per dag som anges i de globala projektinställningarna.



**Det här är varför**

Om de totala arbetstiderna inte stämmer överens kan det leda till felaktigt beräknade datum- och tidsberäkningar på projekttidslinjen och i rapporter.

Om systeminställningen till exempel är åtta timmar per dag och schemat som tilldelats ett projekt bara har sju arbetstimmar per dag, kommer du att märka att en aktivitet med en dagslängd tar mer än en dag att slutföra, eftersom den försöker passa in på åtta timmar.

**Obs!**: Systemets globala projektinställningar görs i Inställningar > Projektinställningar > Tidslinjeberäkningar > Vanliga timmar per arbetsdag.

</br>
</br>


**Bästa praxis**

Lägg till en påminnelse till Adobe Workfront-systemadministratörens kalender om att uppdatera scheman vid en viss tidpunkt varje år.

**Det här är varför**

Uppdatera scheman i din Workfront-instans med nationella helgdagar, helger och andra dagar som användare inte arbetar. Gör detta vid en fast tidpunkt varje år, antingen i slutet av året eller när helgerna frigörs av personalavdelningen, så att projekttidslinjer, resursplanering osv. återspeglar den korrekta tillgängligheten.
