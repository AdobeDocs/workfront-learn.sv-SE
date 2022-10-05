---
title: God praxis - licenser och åtkomstnivåer
description: Utforska rekommendationer från Adobe Workfront experter om hur man ställer in, hanterar och använder Workfront licenser och åtkomstnivåer.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# God praxis - licenser och åtkomstnivåer

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för licenser och åtkomstnivåer

* Börja med mindre åtkomst för användare när de ställer in åtkomstnivåer.

* När du tilldelar gransknings- och begärandelicenser är standardvärdet Granska eftersom det ger användaren fler behörigheter i Adobe Workfront.

* Avmarkera kryssrutan &quot;Dela hela systemet&quot; för varje objekt på alla dina åtkomstnivåer, såvida du inte särskilt vill att användarna ska kunna göra det.

* Överväg att aktivera inställningen&quot;Tillåt aldrig användare att ta bort kommentarer&quot; under Ange ytterligare begränsningar på en åtkomstnivå.

* Begränsa antalet systemadministratörer till förmån för gruppadministratörer.

* Kopiera en befintlig åtkomstnivå och gör ändringar i stället för att skapa en ny åtkomstnivå från grunden.

* Dokumentera vad varje åtkomstnivå kan göra i rutan Beskrivning.

* Begränsa dig till de åtkomstnivåer som krävs för att du ska kunna uppnå dina arbetsmål, helst fyra eller fem som fångar behoven hos de flesta användare i systemet.

* Tilldela minst två användare den globala systemadministratörens åtkomstnivå.

* Begränsa vad användare kan göra med Workfront-objekt genom delning, i stället för att ta bort en funktion på åtkomstnivå.

</br>
</br>


## Varför är detta de bästa sätten?

**Bästa praxis**

Börja med mindre åtkomst för användare när de ställer in åtkomstnivåer.



**Här är varför**

Ge användarna så snabb åtkomst de behöver för att göra sitt arbete. Om de inte kan utföra sina uppgifter på grund av otillräckliga åtkomsträttigheter begär de vanligtvis ytterligare åtkomst. Om användarna får för mycket åtkomst direkt kan det leda till säkerhetsproblem. Dessutom är det alltid bättre att ge användarna mer åtkomst än att ta bort åtkomsten.

</br>
</br>



**Bästa praxis**

När du tilldelar gransknings- och begärandelicenser är standardvärdet Granska eftersom det ger användaren fler behörigheter i Adobe Workfront.



**Här är varför**

Även om både Granska- och Begär-licenser kan tilldelas ett obegränsat antal användare i Workfront, är antalet begärda licenser begränsat till i princip bara att göra och uppdatera begäranden. En granskningslicens har större åtkomst till projekt och uppgifter än en Request-licens, liksom möjlighet att visa portföljer och program, redigera dokument och komma åt resurshanteringsverktyg.

</br>
</br>

**Bästa praxis**

Avmarkera kryssrutan &quot;Dela hela systemet&quot; för varje objekt på alla dina åtkomstnivåer, såvida det inte finns en specifik anledning till att användarna måste kunna dela hela systemet.



**Här är varför**

Att dela objekt i hela systemet används ofta som en kryckning så att vissa användare kan se objekt i Workfront. Detta inträffar när Workfront-gruppstrukturen saknas eller när delningsbehörigheterna inte är helt klarlagda. När objekt delas över hela systemet innebär det att alla kan se det objekt som delas. Beroende på vilken typ av information som lagras i systemet kan detta leda till sekretessproblem.



Du kanske till exempel arbetar med flera leverantörer i Workfront för att kontrollera status, ge godkännanden osv. Om kryssrutan &quot;Dela hela systemet&quot; är ett alternativ, som kan väljas eller anges som standard, blir informationen tillgänglig för alla leverantörer.



Genom att avmarkera alternativet helt och hållet, gör du det så att en användare, med behörighet att dela, måste avgöra vilken eller vilka personer - antingen via ett företag, en grupp eller ett team - de vill dela objektet med.

</br>
</br>

**Bästa praxis**

Överväg att aktivera inställningen&quot;Tillåt aldrig användare att ta bort kommentarer&quot; under Ange ytterligare begränsningar på en åtkomstnivå.



**Här är varför**

Om du aktiverar det här alternativet tas tidigare kommunikation inte bort från Workfront. Vissa organisationer kräver att hela kommentarshistoriken sparas i granskningssyfte.

</br>
</br>

**Bästa praxis**

Begränsa antalet systemadministratörer till förmån för gruppadministratörer.



**Här är varför**

Systemadministratörer har tillgång till allt i Workfront, inklusive globala systeminställningar. De inställningsgruppadministratörer som kan komma åt styrs av systemadministratören och gäller endast den specifika gruppen.



Genom att ha gruppadministratörer kan systemadministratörerna delegera många olika ansvarsområden så att de kan fokusera på större bildobjekt i stället för det dagliga underhållet av Workfront. Gruppadministratörer kan enklare hålla kontakten med sina gruppers behov, vilket ger bättre service för användarna.

</br>
</br>


**Bästa praxis**

Kopiera en befintlig åtkomstnivå och gör ändringar i stället för att skapa en ny åtkomstnivå från grunden.



**Här är varför**

Genom att kopiera en befintlig åtkomstnivå får du en konsekvent bas för nya åtkomstnivåer och ser till att de ursprungliga inställningarna är identiska. Detta är också en tidsbesparande funktion eftersom systemadministratörer inte behöver ställa in en åtkomstnivå helt från början.

</br>
</br>

**Bästa praxis**

Dokumentera vad varje åtkomstnivå kan göra i rutan Beskrivning.



**Här är varför**

Var detaljerad med beskrivningen och ange inställningarna för varje objekttyp. Detta hjälper systemadministratörer - både idag och i framtiden - att veta exakt vad varje åtkomstnivå gör utan att behöva dyka in i själva åtkomstnivån för att kunna granska inställningarna.



Detta kan också göra det enklare att jämföra åtkomstnivåer i en rapport. Beskrivningsfältet kan snabbt läggas till i vyn för att snabbt se hur de skiljer sig och, möjligen, varför en annan åtkomstnivå skapades.

</br>
</br>

**Bästa praxis**

Begränsa dig till de åtkomstnivåer som krävs för att du ska kunna uppnå dina arbetsmål, helst fyra eller fem som fångar behoven hos de flesta användare i systemet.


**Här är varför**

Åtkomstnivån ser till att när ett Workfront-objekt delas med en användare har användaren de rättigheter som krävs för att redigera det, ta bort det osv. Du kan göra åtkomstnivåerna mer allmänna eftersom delning på enskilda objekt kan konfigureras som mer specifikt.


Dessutom kan färre åtkomstnivåer göra det enklare att underhålla ett system utan problem och implementera en strategi, vilket också kan leda till snabbare introduktion när man går med i företaget eller byter avdelning.

</br>
</br>

**Bästa praxis**

Tilldela minst två användare den globala systemadministratörens åtkomstnivå.

**Här är varför**

Mer än en person bör förstå varför Workfront har konfigurerats så som det var, hur det ska hanteras/underhållas och hur man ska stödja användare. Om en person är frånvarande, lämnar organisationen, är upptagen osv. säkerställer detta att det finns en annan person som har informationen och kunskapen för att hantera systemet.

</br>
</br>

**Bästa praxis**

Begränsa vad användare kan göra med Workfront-objekt genom delning, i stället för att ta bort en funktion på åtkomstnivå.


**Här är varför**

Åtkomstnivåerna styr vad användare kan göra med specifika objekt på global nivå. Delningsbehörigheterna för varje projekt, uppgift, portfölj, dokument osv. styr vad en enskild användare kan göra med det specifika objektet. I stället för att ta bort en funktion för alla med en viss åtkomstnivå kan du finjustera delningsbehörigheterna för specifika objekt så att användarna har begränsade kontroller.
