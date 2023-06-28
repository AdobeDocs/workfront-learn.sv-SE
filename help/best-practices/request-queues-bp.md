---
title: Bästa praxis - Begäranköer
description: Utforska rekommendationer om god praxis från Adobe Workfront experter om hur man ställer in, hanterar och använder Workfront begärandeköer.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
jira: KT-10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# Bästa praxis - Begäranköer

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för frågekö

* Ta med en beskrivning för varje element i en begärandekö - begärandeköprojektet, ämnesgrupper, köämnen och routningsregler.

* Skapa en projektstatus med namnet &quot;Begärankö&quot; eller &quot;Operativ&quot; som motsvarar &quot;Aktuell&quot; för att skilja begärandeköprojekt från andra projekt.

* Om du planerar att använda utleveransgodkännanden med begäranden som skickas via en kö skapar du en utgivningsstatus med namnet Avvisat.

* Tilldela anpassade&quot;universella&quot; formulär till köer för att hämta in så mycket data som möjligt i hela företaget.

* Undvik att dela begärandeköer med&quot;alla&quot;. Ställ in köinformationsinställningarna så att användarna bara ser de köer som är relevanta för deras behov.

* Bygg och tilldela en kontrollpanel med begärandekörapporter så att trafikansvariga, systemadministratörer och tilldelade användare kan arbeta direkt med problem.

* Använd layoutmallar för att ta bort inställningsalternativen för begärandekön från den vänstra panelmenyn för projekt för användare som inte behöver skapa köer.

* Skapa en kö för systemadministratörsförfrågningar där användare kan ställa Workfront-relaterade frågor, göra förfrågningar om systeminställningar, schemalägga ny användarutbildning osv.

* Granska begärandeköer regelbundet för att identifiera och ta bort delning av köer som inte används.

* Använd ämnesgrupper för att ordna mer än 10 köämnen i en begärandekö för att skapa kortare och enklare listor.

* Styr det totala antalet begäranköer som är tillgängliga för användare genom att dela upp en begärandekö med ämnesgrupper och köämnen, i stället för att skapa flera köer.

* Ställ in routningsregler för varje köämne. Ange som minimum en standardregel för routning.

* Utnyttja ämnesgrupper och köämnen när selektiv routning behövs.

* Skicka förfrågningar till ett team istället för till en individ.


</br>
</br>


## Varför är detta de bästa sätten?


**Bästa praxis**

Ta med en beskrivning för varje element i en begärandekö - begärandeköprojektet, ämnesgrupper, köämnen och routningsregler.

**Här är varför**

Med beskrivningar kan gruppadministratörer, framtida systemadministratörer och andra som underhåller begärandeköer veta exakt vad varje del av begärandekön gör.

Beskrivningsinformationen visas också när du hovrar över informationsikonen i fältet i det nya fönstret för begäran.

Beskrivningen behöver inte vara lång, bara en kort kommentar om syftet med eller användningen av elementet.

</br>
</br>

**Bästa praxis**

Skapa en projektstatus med namnet &quot;Begärankö&quot; eller &quot;Operativ&quot; som motsvarar &quot;Aktuell&quot; för att skilja begärandeköprojekt från andra projekt.

**Här är varför**

En frågekö som finns i ett projekt och som måste ha samma status som Aktuell för att kön ska vara aktiv.

För att kunna skilja en begäran från faktiska arbetsprojekt med statusen&quot;Aktuell&quot; skapar du en status som bara ska användas på begärandeköer som kallas&quot;Begärandekö&quot; eller&quot;Driftsätt&quot;. Du kan sedan använda den här statusen för att exkludera eller ta med projekt i frågekö när du skriver rapporter.

</br>
</br>

**Bästa praxis**

Skapa en utgivningsstatus med namnet&quot;Avvisat&quot; när du använder utgivningsgodkännanden och ange statusen&quot;Avvisat&quot; för alternativet Om avvisat.

**Här är varför**

Genom att använda statusen&quot;Avvisat&quot; klargörs det att begäran granskades och avvisades.

</br>
</br>

**Bästa praxis**

Tilldela anpassade&quot;universella&quot; formulär till köer för att hämta in så mycket data som möjligt i hela företaget.

**Här är varför**

Ett anpassat universellt formulär samlar in den standardinformation som behövs för begäran, oavsett vilken typ av begäran som skickas.

Ett anpassat &quot;universellt&quot; formulär minskar antalet anpassade formulär som du behöver skapa och underhålla. Det säkerställer också att alla förfrågningar samlar in samma information på samma sätt, vilket leder till enhetlig rapportering och dataanalys.

</br>
</br>

**Bästa praxis**

Undvik att dela begärandeköer med&quot;alla&quot;.  Ställ in köinformationsinställningarna så att användarna bara ser de köer som är relevanta för deras behov.

**Här är varför**

I de flesta fall behöver en begärandekö bara delas med en viss uppsättning personer, som ett team, en leverantör, kunder osv. När beställarna bara ser det de behöver i listan över begärandeköer blir det enkelt att hitta och navigera.

</br>
</br>


**Bästa praxis**

Bygg och tilldela en kontrollpanel med begärandekörapporter så att trafikansvariga, systemadministratörer och tilldelade användare kan arbeta direkt med problem.

**Här är varför**

Att ge användarna snabb och enkel åtkomst till inkommande förfrågningar innebär att arbetet inte går förlorat i flytten.

</br>
</br>

**Bästa praxis**

Använd layoutmallar för att ta bort inställningsalternativen för begärandekön från den vänstra panelmenyn för projekt för användare som inte behöver skapa köer.


**Här är varför**

Detta garanterar att alla begärandeköer går igenom rätt process för att skapas (t.ex. granskas av en styrkommitté) och konfigureras korrekt av antingen en system- eller gruppadministratör.

Dessutom är det här ett sätt att ordna kölistan och fokusera på de typer av förfrågningar som organisationen behöver.

</br>
</br>

**Bästa praxis**

Skapa en kö för systemadministratörsförfrågningar där användare kan ställa Workfront-relaterade frågor, göra förfrågningar om systeminställningar, schemalägga ny användarutbildning osv.

**Här är varför**

Detta är en central plats där användare kan skicka frågor och där administratörer kan samla in, övervaka och besvara Workfront-relaterade frågor.

Dessutom kan den här informationen användas för att visa ledarskap för tid, arbete och värde för systemadministratörsrollen samt som en motivering för ytterligare systemadministratörer.

</br>
</br>


**Bästa praxis**

Granska begärandeköer regelbundet för att identifiera och ta bort delning av köer som inte används.

**Här är varför**

Med en regelbunden granskning av inställningarna och objekten i ditt Adobe Workfront-system blir det enklare att hålla det rent och fritt från onödiga objekt. Om en kö inte längre används eller övervakas bör du se till att användarna inte längre kan komma åt den, så att arbetsförfrågningar inte hamnar i ett tomrum.

</br>
</br>


**Bästa praxis**

Använd ämnesgrupper för att ordna mer än 10 köämnen i en begärandekö för att skapa kortare och enklare listor.

**Här är varför**

Ämnesgrupper gör användarna mer benägna att använda och skapar mindre förvirring genom att minska den inledande listan med alternativ att välja bland. På så sätt kan användarna enkelt hitta det de söker utan att överbelasta dem när de försöker skicka in en förfrågan.

Dessutom ger det systemadministratörer och/eller begärandeköhanterare möjlighet att skapa en smidig navigeringssökväg för användare och ett bättre sätt att organisera och rapportera om de typer av förfrågningar som skickas.

</br>
</br>

**Bästa praxis**

Styr det totala antalet begäranköer som är tillgängliga för användare genom att dela upp en begärandekö med ämnesgrupper och köämnen, i stället för att skapa flera köer.

**Här är varför**

Alltför många begärandeköer gör det svårt för användarna att hitta det de behöver.

Färre köer hjälper även trafiksamordnare, systemadministratörer och andra att hantera köerna, så att de kan hitta den information de behöver snabbare utan att behöva navigera till flera projekt i kön för begäranden.

Skapa flera begärandeköer om olika åtkomst behövs för olika begärandeköer eller om det skulle vara förvirrande för användarna att konsolidera köer.

</br>
</br>

**Bästa praxis**

Ställ in routningsregler för varje köämne. Ange som minimum en standardregel för routning.

**Här är varför**

Routningsregler säkerställer att någon alltid tilldelas den inkommande begäran så att arbetet inte faller igenom sprickorna.

</br>
</br>

**Bästa praxis**

Utnyttja ämnesgrupper och köämnen när selektiv routning behövs.

**Här är varför**

Routningsregler kan inte tillämpas på fält i ett anpassat formulär. Så om olika typer av förfrågningar måste dirigeras till olika team/individer, ska varje typ av begäran ha ett eget ämne i grupp/kö så att arbetet kan dirigeras korrekt.

</br>
</br>

**Bästa praxis**

Skicka förfrågningar till ett team istället för till en individ.

**Här är varför**

När förfrågningar skickas till teamet ger det hela teamet insyn i de förfrågningar som görs och vad det kommande arbetet kan innebära. Alla kan se Team-sidan för nya objekt eller hålla reda på vad som är nytt med en rapport på en kontrollpanel.

Den ser också till att när trafikchefen eller någon annan person som ansvarar för att granska eller tilldela inkommande förfrågningar inte är tillgänglig, så blir en säkerhetskopia automatiskt tillgänglig och har tillgång till informationen om förfrågan.
