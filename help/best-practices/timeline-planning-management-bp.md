---
title: God praxis - planering och hantering av tidslinjer
description: Utforska rekommendationer från Adobe Workfront experter om hur man ställer in, hanterar och använder projekttidslinjer i Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# God praxis - planering och hantering av tidslinjer

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa praxis är riktlinjer som utgör ett effektivt och effektivt sätt att agera, som enkelt används av dig och användarna på ditt företag och som kan återges framgångsrikt i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för planering och hantering av tidslinjer

* Alla slutförda projekt ska ha en status som visar att de är slutförda.

* När du kopierar ett projekt anger du statusen för det nya projektet till Planering.

* Låt användarna registrera den faktiska tiden för uppgifter så att ni kan jämföra faktiska timmar med planerade timmar.

* Använd aktivitetens varaktighet och föregångare när det är möjligt för att skapa och uppdatera en projekttidslinje, i stället för att välja specifika start- och slutdatum.

* Be användarna att uppdatera uppgiftsstatus, procent slutfört och faktiskt antal timmar varje dag (eller enligt ett bestämt schema varje vecka).

* Ställ in projektstatus på Planering när du uppdaterar projektplanen för att förhindra att meddelanden skickas automatiskt när ändringar görs.

* Ta bort användare från projektteamet som inte har tilldelats arbete i projektet.

* Placera Project Metrics överst i den vänstra panelmenyn så att användare som huvudsakligen använder Workfront kan visa data.


</br>
</br>


## Varför är detta de bästa sätten?

**Bästa praxis**

Alla slutförda projekt ska ha en status som visar att de är slutförda.


**Det här är varför**

Om du ser till att alla projekt som är slutförda har statusen Fullständigt (eller motsvarande) håller Workfront-instansen ren och aktuell. Genom att hålla projektstatusarna uppdaterade och stänga dem kan användarna enkelt se vilket arbete som redan har utförts så att de kan fokusera på de aktiva prioriteringarna. Det säkerställer också att rapportdata om projekt, uppgifter, resurser osv. är korrekta.


</br>
</br>

**Bästa praxis**

När du kopierar ett projekt anger du statusen för det nya projektet till Planering.

**Det här är varför**

Planeringsstatusen (eller motsvarande) förhindrar att Workfront-meddelanden om tilldelningar, ändringar av tidslinjen osv. skickas innan projektet är klart. När du kopierar ett projekt visas en dialogruta med projektalternativ. Ändra status här och justera andra alternativ så att data inte kopieras från det ursprungliga projektet till den kopierade versionen.

</br>
</br>

**Bästa praxis**

Låt användarna registrera den faktiska tiden för uppgifter så att ni kan jämföra faktiska timmar med planerade timmar.


**Det här är varför**

Att veta hur lång tid det tar att arbeta med en uppgift innebär att du kan uppdatera projektmallar för större precision i planeringen av framtida projekt. Det innebär också att resursuppskattningar, som använder Workfront resurshanteringsverktyg, blir mer korrekta.

</br>
</br>

**Bästa praxis**

Använd aktivitetens varaktighet och föregångare när det är möjligt för att skapa och uppdatera en projekttidslinje, i stället för att välja specifika start- och slutdatum.

**Det här är varför**

Genom att använda varaktighet och föregångare i kombination med flexibla uppgiftsbegränsningar (så snart som möjligt och så sent som möjligt) kan du automatiskt ändra tidslinjedatum som&quot;överlappar&quot; genom projektplanen. När en uppgifts varaktighet ökar med en dag ändras till exempel aktivitetens planerade slutförandedatum, vilket i sin tur ändrar slutförandedatumet för följande uppgifter.

Om du väljer specifika start- och slutdatum för uppgifter ändras aktivitetsbegränsningen till ett som&quot;låser&quot; datumet (Måste börja på, Måste sluta på, Fasta datum), vilket innebär att du måste göra vissa tidslinjedatumuppdateringar manuellt.

</br>
</br>


**Bästa praxis**

Be användarna att uppdatera uppgiftsstatus, procent slutfört och faktiskt antal timmar varje dag (eller enligt ett bestämt schema varje vecka).

**Det här är varför**

Rapporterna i Workfront är bara lika exakta som uppgifterna i Workfront. När information som indikerar arbetsförloppet - som status och procent färdigt - inte uppdateras regelbundet kommer rapporter som visar arbetsförloppet inte att vara korrekta. Att uppdatera dagligen ger största möjliga noggrannhet när det gäller rapporteringsdata i realtid.


Uppgiftsstatus används också för att meddela användare när tidigare arbete har slutförts och deras nya uppgifter kan börja. När uppgiftsstatusen inte ändras för att återspegla arbetsobjektets verkliga förlopp kan Workfront inte skicka ut lämpliga meddelanden.

</br>
</br>

**Bästa praxis**

Ställ in projektstatus på Planering när du uppdaterar projektplanen för att förhindra att meddelanden skickas automatiskt när ändringar görs.

**Det här är varför**

Ändringar i projektplanen kan generera flera meddelanden när uppgiftstilldelningar, planerade start- och slutförandedatum och andra inställningar ändras. Detta kan vara störande för användarna och skapa förvirring om korrekta tilldelningar, deadlines osv.

Planeringsstatusen anger för Workfront att inga meddelanden om projektet ska skickas till medlemmar i projektteamet (användare tilldelade uppgifter/ärenden eller andra med tillgång till projektet) eftersom projektplanen fortfarande håller på att utvecklas eller projektet inte är färdigt att publiceras än. När ändringarna är klara ändrar du projektstatus till Aktuell och meddelanden skickas. Om du följer den här processen minimeras antalet meddelanden som användarna får.

</br>
</br>

**Bästa praxis**

Ta bort användare från projektteamet som inte har tilldelats arbete i projektet.


**Det här är varför**

När du tilldelar någon en aktivitet eller ett problem i ett projekt läggs användaren till i projektgruppslistan i avsnitten Schemaläggning och Personer i projektet. De finns dock kvar i projektgruppslistan även om du har tagit bort dem från uppdraget. Detta kan skapa förvirring för användaren eftersom de som en del av projektteamet får meddelanden om aktiviteter i projektet och ser projektet i listan Projekt som jag är på.


Dessutom får projektmedlemmarna behörighet till projektet och dess uppgifter, utgåvor och dokument. Detta kan leda till att användare får tillgång till objekt i Workfront som de inte behöver eller inte borde ha.

</br>
</br>

**Bästa praxis**

Placera Project Metrics överst i den vänstra panelmenyn så att användare som huvudsakligen använder Workfront kan visa data.

**Det här är varför**

De flesta chefer, chefer och andra användare som inte hanterar projekt eller utför uppgifter skulle uppskatta att se den här nivån av projektstatistik när de först öppnar ett projekt. Använd en layoutmall för att flytta Project Metrics till toppen av den vänstra panelmenyn på en projektsida, så att den blir mer synlig och lättare att komma åt för användarna.
