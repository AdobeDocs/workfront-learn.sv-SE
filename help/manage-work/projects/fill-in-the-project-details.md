---
title: Fyll i projektinformationen
description: Lär dig vilka 12 projektinformationsfält som ska visas [!DNL  Workfront] rekommenderar att du fyller i när du skapar ett projekt.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
kt: 10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: 6b651fa3e8da77627d4fa1379f1221ebd5793b34
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 0%

---

# Fyll i projektinformationen

Du behöver inte fylla i alla fält och kryssrutor i projektinformationen för varje projekt som du skapar i [!DNL  Workfront]. Använd mallar för att fylla i informationen i förväg och rikta sedan uppmärksamheten mot de 12 viktigaste projektinformationsfälten som listas nedan.

1. **Namn**

   Ett beskrivande projektnamn hjälper alla att identifiera syftet med projektet. Kom ihåg att följa organisationens regler för projektnamn, som kan kräva att viss information inkluderas i projektnamnet (t.ex. ett referensnummer, avdelningsnamn eller kategoriindikator).


1. **Beskrivning**

   När flera personer arbetar med ett projekt måste du - som projektledare - se till att alla är uppdaterade om projektets syfte och förväntningar.

   Gör detta med en projektbeskrivning som ger grundläggande information, svar på frågor och låter projektteamet gå vidare med sitt arbete. Exempel:&quot;En kampanj som syftar till att öka intäkterna från att generera arbete med 50 %&quot; eller&quot;Ny systemuppgradering för att förbättra effektiviteten i hela avdelningen&quot;.

   Vissa Workfront-kunder har ett exempel på hur en projektbeskrivning ska se ut i sina projektmallar.

1. **Status**

   Status används i Workfront för att ange var, eller i vilket skede, i arbetsflödet ett projekt befinner sig. Status används i många Workfront-rapporter för att spåra hur arbetet fortskrider.

   Workfront rekommenderar att du ställer in statusen till Planning medan du slutför projektplanen. Det viktigaste med planeringsstatusen är att Workfront-meddelanden inte går ut till aktivitetstilldelningar om projektet när det är i den här statusen.

   När projektet är klart att publiceras ändrar du statusen till Aktuell. Detta gör att Workfront kan skicka meddelanden till personer om nya uppgifter som de har tilldelats, men det går inte att skicka meddelanden till användare för de uppgifter som de har tilldelats när projektet hade statusen Planering.

   >[!TIP]
   >
   >  När du gör ändringar i projektet, t.ex. ändrar förfallodatum, kan du återställa statusen till Planering eller inaktivera funktionen Spara automatiskt för att förhindra att meddelanden skickas tills ändringarna är klara.

   Planeringsstatusen kan anges som global Workfront-standard för nya projekt av systemadministratören.

1. **Schemaläge**

   Workfront-projekt kan schemaläggas från ett startdatum eller ett avslutsdatum. Det viktiga valet avgör hur de planerade datumen för varje uppgift beräknas.

   Alternativet Startdatum är startdatumet för projektet, som du anger, och varje uppgifts varaktighet och föregående aktiviteter för att beräkna när projektet ska slutföras. Workfront rekommenderar att du använder det här alternativet eftersom det är det vanligaste och gör det enklare att planera projektdatum.

   Du kan dock använda ett slutdatum. Workfront tittar på slutdatumet (anges av dig) och det arbete som ska utföras (baserat på varaktighet och föregående aktiviteter) och arbetar sedan bakåt för att beräkna projektets startdatum. Workfront rekommenderar att du väntar på att använda slutdatumet när en viss kunskapsnivå i Workfront har etablerats.

   Oavsett vilket alternativ du väljer ska du inte glömma att välja ett datum i popup-kalendern.

   Alternativet Schemaläge kan ställas in i mallen.

1. **Grupp**

   En grupp är en organisationsenhet i Workfront som ofta är knuten till en avdelning. Det här fältet kan anges i projektmallen. Om så inte är fallet ställs fältet automatiskt in på hemgruppen för den person som skapar projektet. Du kan ändra gruppen efter behov.

   I allmänhet kommer de flesta som arbetar med projektet från den här gruppen. Men detta begränsar inte personer från andra grupper som tilldelas arbete i projektet.

   Gruppen i projektet avgör också vilka inställningar för projekt, uppgift och utgåva som projektet ska använda. Dessa inställningar, till exempel en anpassad status för en viss grupp, anges av systemadministratören eller en gruppadministratör.

   Gruppinställningen är ett bekvämt sätt att, genom rapportering, visa alla projekt som en avdelning arbetar med.

1. **Projektägare**

   Projektägaren är Workfront villkor för projektledare. Detta är den person som ansvarar för planeringen och/eller ledningen av projektet.

   För att projektägaren ska ha fullständig behörighet att hantera projektet måste han/hon ha en planlicens.

   Normalt lämnas det här fältet tomt i mallen och fylls i automatiskt med namnet på den person som skapar projektet. Om ett namn anges i mallen är det standardägaren av projektet.

1. **Projektsponsorer**

   Projektsponsorn krävs inte, men när den används är det i allmänhet den som begärde projektet. Detta är ofta en intern aktör, till exempel en chef eller en chef, med övergripande ansvar för projektet.

   Sponsorn får automatiskt visningsbehörighet för projektet och måste vara en Workfront-licensierad användare.

   Projektsponsorn kan anges i mallen.

1. **Resurshanteraren**

   De Workfront-användare som visas i det här fältet kan använda verktygen för resursplanering och resurshantering i Workfront för de specifika projekt de listas i. Upp till 30 namn kan listas i fältet Resurshanterare och varje namn måste ha en planlicens.

   Fältet Resurshanterare kan anges i mallen.

1. **Anpassad Forms**

   Workfront innehåller inbyggda fält för exempelvis projektnamn och startdatum. Men det finns ytterligare information som du behöver som projektledare, eller som projektteamet behöver. Dina unika data är lika viktiga och kan enkelt lagras i dessa formulär. Information om publiceringsdatum, utskriftsmaterialstorlekar, leveranskanaler osv.

   Anpassade formulär kan hämta in den här informationen och kan inkluderas i listor och rapporter i Workfront, vilket gör informationen enkel att visa och redigera.

   Anpassade formulär kan bifogas till mallarna i förväg.

1. **Schema**

   Arbetet sker dygnet runt, eftersom många företag har anställda över hela världen.

   Med Workfront kan du använda ett gemensamt schema för projekt. Dessa skapas av systemadministratören. Schemana återspeglar arbetsdagarna och arbetstiderna för era team, plus dagar då medarbetarna inte arbetar (t.ex. helger).

   Som planerare måste du se till att du använder rätt schema för rätt projekt. Schemainställningarna påverkar tidslinjeberäkningar, med hänsyn tagen till tid och tidszoner.

   Det schema som tilldelats projektet ska vara det som gäller för merparten av de tilldelade uppgifterna. Om inget schema har angetts för projektet används det schema som är markerat som standard.

   Schemat kan anges i mallen.

1. **Resurspooler**

   Resurspooler är samlingar med Workfront-användare som samtidigt behövs för att slutföra projekt i organisationen. En resurspool kan tilldelas till flera projekt, vilket betyder att du har projekt som konkurrerar om resurser.

   Att ha resurspooler tilldelade till ett projekt är en förutsättning för att du ska kunna använda resursplaneringsverktyget och andra resurshanteringsverktyg i Workfront.

   En standardresurspool kan anges i mallen.

1. **Åtkomst till projektet för tittare och medarbetare**

   När någon får åtkomst till ett projekt via Dela finns det tre behörighetsnivåer som kan tilldelas: Visa, Contribute och Hantera. Varje behörighetsnivå tillåter användaren att se och göra vissa saker med projektet.

   Det finns till exempel personer som kan ha tillgång till projektet men som inte ska se den ekonomiska informationen. Du kan alltså inaktivera alternativet Visa finansiering för dem.

   Åtkomstinställningarna kan anges i mallen.
