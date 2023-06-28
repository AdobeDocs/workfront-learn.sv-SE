---
title: God praxis - API Explorer
description: Utforska rekommendationer om god praxis från Adobe Workfront experter om hur du konfigurerar, hanterar och använder Workfront API Explorer.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# God praxis - API Explorer

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för API Explorer

* Upprätta en namnkonvention för anpassade fält som används med integreringar från tredjepartssystem.

* Spåra alla anpassade fält som används i integreringar med ett Workfront-projekt.

* Lägg till objektets ID-fält i rapporter som används av systemadministratören.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Upprätta en namnkonvention för anpassade fält som används med integreringar från tredjepartssystem.

**Här är varför**

Se till att alla som skapar anpassade formulär känner till namnkonventionen, så att de inte oavsiktligt använder ett fält som är reserverat för en integrering. Beroende på era integreringar och arbetsflöden kan användning av samma fält på flera sätt leda till att data ändras eller skrivs över, vilket kan leda till felaktiga data i rapporter.

</br>
</br>


**Bästa praxis**

Spåra alla anpassade fält som används i integreringar med ett Workfront-projekt.

**Här är varför**

Ett projekt är det perfekta stället att logga egna fältnamn, vilken integrering de används med osv. Det hjälper dig att undvika att skapa redundanta anpassade fält eller att använda samma anpassade fält med flera integreringar.

</br>
</br>


**Bästa praxis**

Lägg till objektets ID-fält i rapporter som används av systemadministratören.

**Här är varför**

Systemadministratörer behöver ofta referera till objekt i Workfront med sina ID-nummer när de använder API:er eller andra integreringar. Inkludera ID-fältet i vyer för de objekt du arbetar med (projekt, uppgifter, ärenden, mallar, anpassade formulär osv.) för att göra det enkelt att komma åt och kopiera.
