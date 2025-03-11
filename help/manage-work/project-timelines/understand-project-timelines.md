---
title: Förstå projekttidslinjer
description: Lär dig hur du tilldelar uppgifter, använder Gantt-scheman och funktioner för kritiska sökvägar, övervakar projekt via vyer, schemalägger aktiviteter effektivt och tillämpar begränsningar för optimal projektplanering.
activity: use
feature: Work Management
thumbnail: 335213.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2024-11-01T00:00:00Z
recommendations: noDisplay,catalog
jira: KT-8953
exl-id: ba993197-9f84-4fc0-86cc-cf849c889f56
doc-type: video
source-git-commit: b31a0e6255d7e298ac95b14c308ca3fa5fb8e1d3
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Förstå projekttidslinjer

Det här lär du dig:

* Få en översikt över projektplanering och projektledning med Workfront. Lär dig hur överordnade uppgifter grupperar flera underuppgifter, som tilldelas till jobbroller och senare till användare med nödvändiga kunskaper. Föregångare anger sekventiella relationer mellan uppgifter, medan aktiviteter utan föregående aktiviteter kan utföras parallellt. Gantt-schemat erbjuder en visuell tidslinje och funktionen Kritisk bana lyfter fram uppgifter som kan fördröja projektet om de glider.
* Olika vyer i Workfront, t.ex. standardvyn för planering och statusvyn för övervakning av förloppet, som innehåller flaggor för förlopp, kommentarer, dokument, ärenden, godkännanden, kritisk sökväg och milstolpar. Senaste aktivitet kan spåras för att visa uppdateringar och anteckningar.
* Schemaläggningen kan göras från ett startdatum eller ett avslutsdatum, där Workfront beräknar motsvarande datum baserat på aktivitetens varaktighet och föregående aktiviteter. I videon rekommenderas schemaläggning från ett startdatum för viktiga slutförandedatum för att tillåta en viss frånkoppling. Uppgiftsbegränsningar som&quot;så snart som möjligt&quot; och&quot;så sent som möjligt&quot; omfattas också, vilket visar hur de påverkar schemaläggningen av uppgifter. Anpassade vyer kan skapas för att visa begränsningar för aktiviteter.

>[!VIDEO](https://video.tv.adobe.com/v/335213/?quality=12&learn=on&enablevpops)

>[!IMPORTANT]
>
>En mer fullständig förklaring av varaktighetstyper och aktivitetsbegränsningar finns i [Förstå och hantera varaktighetstyper och aktivitetsbegränsningar](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md).

## Viktiga uppgifter

* **Aktivitetshantering och tilldelning:** Överordnade uppgifter grupperar flera underaktiviteter, som tilldelas till jobbroller och senare till användare med nödvändiga kunskaper. &#x200B; Föregångare anger sekventiella relationer, medan åtgärder utan föregångare kan utföras parallellt. &#x200B;
* **Gantt-schema och kritisk sökväg:** Gantt-schemat ger en visuell tidslinje för projektet och funktionen Kritisk sökväg markerar aktiviteter som kan fördröja projektet om de glider. &#x200B;
* **Vyer och övervakning:** Olika vyer i Workfront, t.ex. standardvyn för planering och statusvyn för övervakning, innehåller flaggor för förlopp, kommentarer, dokument, utgåvor, godkännanden, kritisk sökväg och milstolpar. Senaste aktivitet kan också spåras. &#x200B;
* **Schemaläggningsalternativ:** Projekt kan schemaläggas från ett startdatum eller ett slutförandedatum, där Workfront beräknar motsvarande datum baserat på aktivitetens varaktighet och föregående aktiviteter. &#x200B; Vi rekommenderar att du schemalägger från ett startdatum för viktiga slutförandedatum så att du kan använda lite slack. &#x200B;
* **Aktivitetsbegränsningar:** Aktivitetsbegränsningar som &quot;så snart som möjligt&quot; och &quot;så sent som möjligt&quot; påverkar schemaläggningen av aktiviteter. &#x200B; Om du ändrar schemaläget efter att projektet har skapats kan aktivitetsbegränsningar och planerade datum påverkas. &#x200B; Anpassade vyer kan skapas för att visa begränsningar för aktiviteter. &#x200B;


## Om du vill ändra eller inte ändra datum på &#x200B; projekttidslinjer..

| PROS (ändra datum) | KONS (Ändra datum) | PROS (ändrar inte datum) | KONS (Ändrar inte datum) |
|---------------------------|---------------------------|---------------------------|---------------------------|
| <ul><li>Minska stressen/ge användarna uppdaterade förväntningar - &quot;_Creative Cloud vet inte vad som är verkligt_&quot;</li><li>Korrekt resursallokering, särskilt i arbetsbelastningsutjämnaren</li><li>Använd journalpostrapporter (eller projektvaraktighet) för att anropa datumändringar</li><li>Användning av villkor som ska visas om projektet ligger utanför omfånget</li><li>Kan lägga till ett eget formulär (eller använda problem) för att spåra ändringar - varför det skickades, av vem, hur länge</li></ul> | <ul></li><li>Felaktiga data som rapporter återspeglar inte det verkliga läget</li><li>Felaktig uppfattning om förloppet - illusion av att allt är på rätt spår &#x200B;</li><li>Utveckla en kultur av att alltid skjuta bakåt tidslinjer i stället för att ta itu med &#x200B; grundorsaker</li><li>Förlorat förtroende hos intressenter/team för att klara deadlines </li></ul> | <ul></li><li>Korrekt återgivning av projekttidslinjen - data kan användas för analys och för att ge en tydlig bild av vad som hände</li><li>Alternativ för att ändra varaktighet eller lägga till fördröjning till föregående i stället</li><li>Identifiera enkelt processförbättringar för framtida projektplanering/&#x200B;</li><li>Möjlighet att utnyttja baslinjer för att hämta in den ursprungliga projektplanen och använda den som jämförelse</li><li>Om ni inte har folk som kan göra det, och göra det för allt, gör det inte &#x200B;</li></ul> | <ul></li><li>Användarförvirring och/eller frustration - överflödet av&quot;sena&quot; uppgifter trots att de just fått meddelanden</li><li>Resurserna allokerades effektivt för att mappa till den ursprungliga planen, men nu är de överbelastade med försenat arbete</li><li>Projektets tidslinje kan inte användas för att tydligt kommunicera uppdateringar till intressenter</li></ul> |


## Rekommenderade självstudiekurser i detta ämne

* [Spåra förlopp från projekttidslinjen](/help/manage-work/project-timelines/track-work-progress-from-the-project-timeline.md)
* [Förstå datumtyper och förloppsstatus](/help/manage-work/project-timelines/understand-task-dates-and-progress-status.md)
* [Förstå och hantera varaktighetstyper och uppgiftsbegränsningar](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)

