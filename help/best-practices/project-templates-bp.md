---
title: God praxis - projektmallar
description: Utforska rekommendationer från Adobe Workfront experter om hur du konfigurerar, hanterar och använder Workfront projektmallar.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: d39151288d8b749940c5183063392ee471769445
workflow-type: tm+mt
source-wordcount: '1743'
ht-degree: 0%

---

# God praxis - projektmallar

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa praxis är riktlinjer som utgör ett effektivt och effektivt sätt att agera, som enkelt används av dig och användarna på ditt företag och som kan återges framgångsrikt i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för projektmallar

* Använd mallar när du skapar projekt.

* Skapa en namnkonvention för projektmallar.

* Skapa en utvald grupp användare som kan skapa och uppdatera projektmallar.

* Använd Projektdelning på en projektmall för att automatiskt ge åtkomst till projekt som skapats med den mallen.

* Tilldela roller eller team för uppgifter, inte individer.

* Undvik att bli för detaljerad när du skapar uppgifter i en projektmall. Begränsa antalet uppgifter i en projektmall till de som behövs för att slutföra arbetet.

* Använd uppgiftsbeskrivningen för att hämta de små stegen i uppgiften, i stället för att dela upp dem i flera uppgifter.

* Se till att malluppgifterna innehåller varaktigheter, planerade timmar och föregående aktiviteter.

* Förkonfigurera projektinformation och bifoga anpassade formulär i mallen.

* Granska och uppdatera projektmallar regelbundet.

* Kontrollera mallarna så att de har all information de behöver innan du delar dem och andra börjar använda dem.

* När du justerar alternativet Schemalägg från för en mall granskar och uppdaterar du uppgiftsbegränsningarna.

* Kontrollera projektteamet i mallen och ta bort användare som inte är associerade med projektet.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Använd mallar när du skapar projekt.

**Det här är varför**

Med projektmallar slipper du gissa sig till projektledare (och andra som skapar projekt) vad gäller vilka uppgifter ett projekt ska innehålla, hur tidslinjen ska struktureras osv. Mallar är det mest effektiva sättet att snabba upp projektskapandet.

Det är viktigt att mallarna är enhetliga i projekt av liknande typ, så att människor, processer och datapunkter alltid är detaljerade på samma sätt. Även projekt med snabba övergångar (en eller två dagar) och minimala uppgifter kan dra nytta av att de skapas med projektmallar.

Denna enhetlighet i projekten ger exaktare data, vilket är viktigt när ni fattar beslut för ert team, på er avdelning och i hela organisationen.

</br>
</br>

**Bästa praxis**

Skapa en namnkonvention för projektmallar.

**Det här är varför**

Enhetliga namn gör mallarna enklare att hitta. Det hjälper även projektledare och andra att skapa projekt att välja rätt mall när det finns mallar med liknande namn i flera team eller avdelningar.

</br>
</br>

**Bästa praxis**

Skapa en utvald grupp användare som kan skapa och uppdatera projektmallar.

**Det här är varför**

Att ha välbyggda, enhetliga projektmallar är avgörande för god arbetshantering och korrekt rapportering. Begränsa antalet användare som kan redigera mallar för att undvika oavsiktliga eller ej godkända ändringar.

</br>
</br>

**Bästa praxis**

Använd Projektdelning på en projektmall för att automatiskt ge åtkomst till projekt som skapats med den mallen.

**Det här är varför**

Tillgång till särskilda projekt beviljas genom själva projektet. Om samma grupp av personer alltid behöver åtkomst till projekt som skapats med en viss mall lägger du till dem under alternativet Projektdelning i mallen. Det är inte bara så att du kan styra åtkomsten till projekt så snart de har skapats, det effektiviserar skalbarheten om behörigheterna behöver ändras i framtiden.

Instruktioner om hur du delar projekt som skapats med en mall finns i kapitlet&quot;Dela projekt som skapats med en mall&quot; i [Dela en projektmall](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/share-a-project-template.html?lang=sv-SE).

**Obs!**: Malldelning ger åtkomst till själva mallen. En användare måste ha minst behörigheten Visa för att kunna skapa projekt med mallen.

</br>
</br>

**Bästa praxis**

Tilldela roller eller team för uppgifter, inte individer.

**Det här är varför**

När en enskild användare ändrar positioner eller lämnar organisationen måste du uppdatera projektmallar som innehåller den personen manuellt. Detta tar tid för system- eller gruppadministratörer eller projektledare.

Om du använder jobbroller eller team i mallar kommer personaländringar inte att ha någon direkt effekt på dina projektmallar eftersom alla som har tilldelats den jobbrollen eller i det teamet kan tilldelas arbetet. Detta bidrar till att säkerställa att arbetet inte glider igenom sprickorna. Jobbrolltilldelningar gör det också enklare att tilldela arbete till enskilda användare eftersom Workfront kan visa en lista över personer som tilldelats den jobbrollen.

Dessutom används jobbroller av Workfront resursplaneringsverktyg för att hjälpa dig att beräkna nödvändiga resurser och planera för framtida arbete.

</br>
</br>

**Bästa praxis**

Undvik att bli för detaljerad när du skapar uppgifter i en projektmall. Begränsa antalet uppgifter i en projektmall till de som behövs för att slutföra arbetet.

**Det här är varför**

Överkomplicerade projektmallar ger en sämre upplevelse för användarna - projektledare, resurshanterare, teammedlemmar med mera. För många uppgifter gör projekttidslinjen svår att hantera, med överlappande deadlines och flera uppgifter tilldelade till samma roller eller personer.


</br>
</br>

**Bästa praxis**

Använd uppgiftsbeskrivningen för att hämta de små stegen i uppgiften, i stället för att dela upp dem i flera uppgifter.

**Det här är varför**

Om flera uppgifter på en rad tilldelas till samma jobbroll/person, är det en indikation på att dessa uppgifter kan kombineras. För många uppgifter som tilldelats en användare kan få dem att känna att det finns mer arbete att slutföra, vilket kan påverka Workfront användning.

</br>
</br>

**Bästa praxis**

Se till att malluppgifterna innehåller varaktigheter, planerade timmar och föregående aktiviteter.

**Det här är varför**

Dessa tre saker - varaktighet, planerad tid och föregångare - är byggstenarna i projektets tidslinje. Detta är nyckeln till att veta hur lång tid det kommer att ta och när det behöver göras. Workfront resurshanteringsverktyg använder varaktighet och planerade timmar, plus jobbrolltilldelningar, för att beräkna resurskapacitet, tillgänglighet och mycket annat.

Om du är osäker på hur du ska beräkna varaktighet eller planerade timmar för första gången kan du tillsammans med projektteamet definiera några initiala uppskattningar. När du har använt mallen kan du mötas med projektteamet igen för att avgöra var ändringar kan göras för att göra mallen mer exakt. Om användarna loggar tid i Workfront kan du jämföra ett projekts planerade timmar med faktiska timmar för att se var justeringar behövs.


</br>
</br>

**Bästa praxis**

Förkonfigurera projektinformation och bifoga anpassade formulär i mallen.

**Det här är varför**

Se till att information som är standard för alla projekt är ifylld i projektmallen. Detta snabbar inte bara upp projektframtagningen, utan säkerställer också att det finns nödvändig information och att den är konsekvent i alla projekt.

Bifoga anpassade projektformulär som matchar anpassade frågeformulär som hämtar in inskickad information när begäran konverteras till ett projekt med hjälp av mallen.

Instruktioner om hur du bifogar ett anpassat formulär till ett objekt, t.ex. en projektmall, finns i [Koppla ett anpassat formulär till ett objekt](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-using-a-custom-form.html?lang=sv-SE).

</br>
</br>

**Bästa praxis**

Granska och uppdatera projektmallar regelbundet.

**Det här är varför**

När processer och team förändras bör projektmallarna uppdateras. Upprätta ett regelbundet avbrott, t.ex. kvartalsvis, för att kontrollera och se vilka mallar som inte används aktivt. Du kan inaktivera dessa, så de finns fortfarande i Workfront men visas inte i mallurvalslistor.

Instruktioner om hur du inaktiverar en projektmall finns i [Inaktivera en projektmall](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/deactivate-a-project-template.html?lang=sv-SE).

</br>
</br>

**Bästa praxis**

Kontrollera mallarna så att de har all information de behöver innan du delar dem och andra börjar använda dem.


**Det här är varför**

Eftersom mallarna kommer att användas gång på gång för att skapa projekt måste du se till att allt är korrekt konfigurerat. Detta leder till enhetlighet i alla projekt och korrekta data för rapportering.

Förutom aktivitetsinställningar som varaktighet och planerade timmar kan du granska innan du delar mallar:

* Schemalägg från inställning
* Aktivitetsbegränsningar
* Projektägare, sponsor, grupp och företag
* Portfolio och program
* Milstolpebana och steg
* Godkännandeprocesser
* Se till att användare som tilldelats uppgifter i projekt har Contribute-åtkomst till projektet
* Resursgrupper
* Påminnelsemeddelanden
* Schema
* Valutainställning (om tillämpligt)
* Bifoga standarddokument
* Bifoga nödvändiga tullformulär
* Kontrollera att det inte finns fler tilldelade personer i projektteamet

</br>
</br>

**Bästa praxis**

När du justerar alternativet Schemaläge för en mall granskar och uppdaterar du uppgiftsbegränsningarna.

**Det här är varför**

Om du blandar olika uppgiftsbegränsningar i ett projekt kan det orsaka oväntade och förvirrande datumberäkningar. Om du t.ex. väljer Startdatum för alternativet Schemaläge tilldelas alla aktiviteter som skapas i det projektet som standard aktivitetsbegränsningen Så snart som möjligt. Om du senare byter till alternativet Schemaläge till Slutförandedatum har alla skapade uppgifter som standard en Aktivitetsbegränsning som är så sen som möjligt. Om du har en oavsiktlig blandning av uppgifter med var och en av dessa begränsningar kan det leda till att planerade datum på projekttidslinjen blir förvirrande.

Mer information om aktivitetskontraktioner och hur du använder dem finns i [Förstå och hantera varaktighetstyper och aktivitetsbegränsningar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=sv-SE).

</br>
</br>

**Bästa praxis**

Kontrollera projektteamet i mallen och ta bort användare som inte kommer att arbeta med projektet.

**Det här är varför**

När du skapar en mall från ett befintligt projekt, såvida du inte väljer alternativet Rensa tilldelningar när du skapar, tar Workfront över de personer som har tilldelats uppgifter/ärenden i projektet i avsnittet Personer. När du arbetar med mallen kanske du vill ta bort personer som tidigare tilldelats arbete eller ändra ett uppdrag som du själv har gjort i mallen.

Alla dessa användare kommer att listas som en del av projektteamet i avsnitten Personer och Schemaläggning i projektet. Resultatet blir att de sprids till alla projekt som skapas från den mallen. Detta kan skapa förvirring för användaren eftersom de som en del av projektteamet får meddelanden om aktivitet i projektet, ser projektet i listan Projekt som jag är på och får behörighet till projektet och dess uppgifter, utgåvor och dokument.

Instruktioner om hur du redigerar projektteamet i en projektmall finns i [Redigera projektteamet i en projektmall](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/edit-the-project-team-in-a-project-template.html?lang=sv-SE).
