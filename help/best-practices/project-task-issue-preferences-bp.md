---
title: Bästa praxis - Inställningar för projekt, uppgift och utgåva
description: Utforska rekommendationer om god praxis från Adobe Workfront experter om hur du konfigurerar, hanterar och använder Workfront projekt, uppgifter och ärenden.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Bästa praxis - Inställningar för projekt, uppgift och utgåva

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa praxis är riktlinjer som utgör ett effektivt och effektivt sätt att agera, som enkelt används av dig och användarna på ditt företag och som kan återges framgångsrikt i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för projekt, aktiviteter och utgåvor av inställningar

* Ange standardvaraktighetstypen för aktiviteten till Enkel.

* Ange planerings- eller Ideainställningarna för ett nytt projekts status, inte Aktuell.

* Aktivera Skapa baslinjer automatiskt i de globala projektinställningarna.

* Markera alla alternativ i avsnittet Affärsfall i systemprojektinställningarna.

* Markera alternativet Uppdatera status för Lösning av problem automatiskt i Utgåvningsinställningar när statusen för Lösning av objekt ändras.

</br>
</br>


## Varför är detta de bästa sätten?

**Bästa praxis**

Ange standardvaraktighetstypen för aktiviteten till Enkel.

**Det här är varför**

Varaktighetstyper definierar relationen mellan aktivitetens varaktighet, planerade timmar och antalet personer som tilldelats till aktiviteten.

Med Simple som standard för det globala systemet har alla manuellt skapade uppgifter den här varaktighetstypen. Planerade timmar fördelas jämnt mellan de tilldelade uppgifterna över varaktighetens längd. Typen av enkel varaktighet kan förenkla projektplaneringen, eftersom den gör det möjligt att ändra aktivitetens tilldelningar och planerade timmar utan att det påverkar aktivitetens varaktighet, planerade startdatum eller planerade slutdatum.

</br>
</br>

**Bästa praxis**

Ange planerings- eller Ideainställningarna för ett nytt projekts status, inte Aktuell.

**Det här är varför**

Statusen Aktuell anger att ett projekt är aktivt och att arbete aktivt utförs. Det är sällsynt att ett projekt behöver ha denna status när det skapas. Även om du använder en projektmall är det en del &quot;planering&quot; som handlar om att göra aktivitetstilldelningar, justera projektets planerade slutförandedatum osv. Planeringsstatusen inaktiverar även meddelanden till aktivitetstilldelningar och projektgruppsmedlemmar. Att ta emot meddelanden innan projektet är live kan vara förvirrande för alla inblandade.

</br>
</br>

**Bästa praxis**

Aktivera Skapa baslinjer automatiskt i de globala projektinställningarna.

**Det här är varför**

Varje gång du ändrar en projektstatus till Aktuell registreras en projektbaslinje automatiskt i Workfront. Denna&quot;ögonblicksbild&quot; av projektet ger historik över hur projektets plan ändrades över tid. Du kan t.ex. jämföra den ursprungliga projektplanen med den aktuella planen när du visar ledarskap hur förskjutningsprioriteringarna eller omfattningen påverkade projektets deadlines.

</br>
</br>

**Bästa praxis**

Markera alla alternativ i avsnittet Affärsfall i systemprojektinställningarna.

**Det här är varför**

Möjliggör för alla fem alternativen så att projektledare, planerare och andra kan ta med vilka avsnitt som helst i affärsärendet i ett projekt. Om alternativen inte är aktiverade visas de inte i fönstret med affärsärenden. Användarna kan lämna alla fält tomma om de inte behövs för det aktuella projektet, men de kan inte aktivera ett fält på projektnivå. Dessa alternativ kan bara aktiveras globalt i installationsprogrammet.

</br>
</br>

**Bästa praxis**

Markera alternativet Uppdatera status för Lösning av problem automatiskt i Utgåvningsinställningar när statusen för Lösning av objekt ändras.

**Det här är varför**

När ett problem konverteras till ett projekt används den här inställningen för att länka status för de två objekten. Om du uppdaterar statusen för projektet (det objekt som löser problemet) uppdateras status automatiskt. Det innebär att den som beställer kan se hur processen fortskrider på begäran, även om de inte har behörighet att se hela projektet i Workfront.
