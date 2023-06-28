---
title: Bästa praxis - Systemprestanda och underhåll
description: Utforska rekommendationer från Adobe Workfront experter om prestanda och underhåll för Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Bästa praxis - Systemprestanda och underhåll

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för systemprestanda och underhåll

* Granska versionsinformationen före releasedatum.

* Skapa olika typer av undantagsrapporter som markerar saknade eller felaktiga data och inställningar.

* Skapa en användarinaktiveringsprocess som omfattar en granskning av objekt som ägs eller tilldelas av dem, så att användare som inte längre är en del av företaget inte fortsätter att vara aktiva i systemet och skapar förvirring för andra användare.

* Behåll arbetsflödeskonfigurationerna så enkla som möjligt för att säkerställa att de är skalbara och kan underhållas utan att vara tillgängliga.

* Använd filter för rapporter och objektlistor för att minska antalet rader som visas samtidigt och fokusera teamet på viktig information.

* Rensa regelbundet webbläsarens cacheminne och cookies för att förbättra prestandan i Workfront.

* Börja rensa upp systemet i de stora områden inom Adobe Workfront som ofta är mest röriga: skräddarsydda blanketter, mallar, projekt och användare.

* Ta reda på vilket kluster din Workfront-instans är i så att du kan hålla utkik efter uppdateringar, vara medveten om underhållstiderna och så vidare.

* Håll projekten korta.

* Om det är möjligt bör rapporten&quot;light&quot; med mycket få och okomplicerade filter användas för att förbättra prestandan.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Granska versionsinformationen före releasedatum.



**Här är varför**

Versionsinformationen talar om vilka nya funktioner och verktyg som kommer till Workfront. Genom att granska anteckningarna och gå runt med de nya funktionerna i förhandsgranskningssandlådan får du möjlighet att lära dig mer om, öva med och lösa eventuella buggar med nya förbättringar innan de släpps till produktion.

</br>
</br>

**Bästa praxis**

Skapa olika typer av undantagsrapporter som markerar saknade eller felaktiga data och inställningar.



**Här är varför**

Rapporterna innehåller information om vilka användare som ska inaktiveras, vilka projekt som ska slutföras i procent av 100 % men som inte markerats som fullständiga, vilka mallar som aldrig har använts osv.



Lägg in dessa rapporter, och andra, på en kontrollpanel och ge andra system- och gruppadministratörer tillgång till den här kontrollpanelen för att få ett rent system i tid. Exempel: Workfront Cleanup Dashboard och Workfront Usage Dashboard innehåller rapportexempel som du kan skapa.



För att du lättare ska komma ihåg att kontrollera dessa rapporter, åtminstone kvartalsvis, ska du skapa ett projekt med kvartalsvisa uppgifter och tilldela dem till dig själv samt system- och gruppadministratörer. Se till att de här aktiviteterna har associerade planerade timmar så att tilldelningar av dessa arbetsobjekt kan fördela tiden korrekt.

</br>
</br>

**Bästa praxis**

Håll projekten korta.



**Här är varför**

Varje gång du sparar ett projekt, eller en uppgift i projektet, körs en tidslinjeberäkning som uppdaterar alla beroenden. Beroende på antalet uppgifter i projektet kan omberäkningen ta lång tid att köra.
