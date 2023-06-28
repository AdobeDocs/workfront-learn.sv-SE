---
title: God praxis - korrektur
description: Utforska rekommendationer från Adobe Workfront experter om hur man ställer in, hanterar och använder korrektur i Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# God praxis - korrektur

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Korrektur på Workfront

* Skapa korrekturmallar för arbetsflöden.

* Inaktivera inställningen&quot;Skicka e-post från Workfront när en kommentar görs på ett korrektur&quot; i Workfront-inställningarna.

* Använd bara Skrivskyddat eller Granskare för inställningen &quot;Roller för icke-mottagare som öppnar ett dokumentkorrektur&quot; i Workfront.

* Justera inställningarna så att användarna ser deadlines i 12-timmarsformat.

* Fastställ en standardkorrekturdeadline som en del av systeminställningarna.

* Dölj alternativet Ej relevant bevisbeslut.

* Ändra inte ordningen på alternativen för korrekturval i korrekturinställningarna.

* Ange standardvärden för korrekturroller och e-postaviseringar.

* Ställ in korrekturförfattarens korrekturroll till Granskare.

* Undvik att använda korrekturrollen för godkännare.

* Undvik e-postaviseringsalternativet Alla aktivitetskorrektur.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Skapa korrekturmallar för arbetsflöden.

**Här är varför**

Mallar snabbar inte bara upp och effektiviserar korrekturläsning och tilldelningsprocessen, de ger också ett enhetligt korrekturflöde för liknande typer av material. De ser också till att varje korrekturmottagare tilldelas rätt korrekturroll och e-postavisering och att en deadline har ställts in.

</br>
</br>

**Bästa praxis**

Inaktivera inställningen&quot;Skicka e-post från Workfront när en kommentar görs på ett korrektur&quot; i Workfront-inställningarna.



**Här är varför**

När den här inställningen är aktiverad (vilket den är som standard) kan användare få flera e-postmeddelanden för varje kommentar i ett korrektur - en från korrekturfunktionen och en från Workfront. De här dubblettmeddelandena orsakar e-postmeddelanden som stör och förvirrar, samt en fullständig e-postinkorg, vilket i slutänden kan leda till att användare ignorerar korrekturmeddelanden som de får. Det kan i sin tur betyda missade deadlines.



**Anteckning**: Den här inställningen finns på Workfront huvudmeny > Inställningar > E-post > Granska och godkänn.

</br>
</br>

**Bästa praxis**

Använd bara Skrivskyddat eller Granskare för inställningen &quot;Roller för icke-mottagare som öppnar ett dokumentkorrektur&quot; i Workfront.



**Här är varför**

De andra alternativen för den här inställningen kräver att du fattar ett korrekturbeslut, vilket kan leda till att korrekturläsningen inte fungerar som det ska. Vanligtvis behöver de som inte läggs till i korrekturarbetsflödet bara visa korrekturet eller göra kommentarer, inte godkänna korrekturet, så skrivskyddet eller granskningsalternativen är det bästa valet.



**Anteckning**: Den här inställningen finns i Workfront huvudmeny > Inställningar > Granska och godkänn.

</br>
</br>

**Bästa praxis**

Justera inställningarna så att användarna ser deadlines i 12-timmarsformat.



**Här är varför**

Välj alternativet F j, Y, gi:a i korrekturinställningarna för användare som vill se korrekturtider i AM/PM-format. För områden där en 12-timmarsklocka används är det här ett bra sätt att förtydliga tidsgränsen.



**Anteckning**: Du hittar den här inställningen genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Användare > och redigera datumformatfältet för varje användare.

</br>
</br>

**Bästa praxis**

Fastställ en standardkorrekturdeadline som en del av systeminställningarna.



**Här är varför**

När en standardgräns för korrektur har angetts - överföringsdatumet + x antal arbetsdagar - gäller att om den som skapat beviset glömmer att lägga till en deadline, tillämpar Workfront automatiskt denna deadline för varje korrektur som överförts.



**Anteckning**: Du hittar den här inställningen genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Inställningar > Korrekturinställningar > Deadline (+ arbetsdagar).

</br>
</br>


**Bästa praxis**

Dölj alternativet Ej relevant bevisbeslut.



**Här är varför**

Det här beslutsalternativet orsakar ofta förvirring bland godkännare, eftersom organisationer ofta inte definierar när alternativet Ej relevant ska användas. Alternativet Ej relevant anger vanligtvis att beviset inte är relevant för bevismottagaren och att de inte behöver fatta ett godkänt eller avvisat beslut. Om du väljer Inte relevant kan korrekturarbetsflödet fortsätta.


Alternativet Ej relevant behövs inte i de flesta korrekturarbetsflöden.

**Anteckning**: Du hittar den här inställningen genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Beslut.

</br>
</br>

**Bästa praxis**

Ändra inte ordningen på alternativen för korrekturval i korrekturinställningarna.



**Här är varför**

Varje inställning för korrekturval innehåller ett specifikt värde/vikt som, om den beställs på nytt, kan skapa förvirring i dina korrekturkonfigurationer. Beslutsordningen och värde/vikt används som styrkande fasaktiveringsutlösare och vid rapportering.



**Anteckning**: Du hittar den här inställningen genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Beslut.

</br>
</br>

**Bästa praxis**

Ange standardvärden för korrekturroller och e-postaviseringar.



**Här är varför**

Dessa inställningar fylls i automatiskt när du tilldelar ett korrekturarbetsflöde, snabbar upp processen och bidrar till att korrekturarbetsflödena blir enhetliga.



**Anteckning**: Användarens standardinställningar hittar du genom att gå till Workfront huvudmeny > Korrektur > Kontoinställningar > Användare > och välja den användare som du vill ange standardinställningar för.

</br>
</br>

**Bästa praxis**

Ställ in korrekturförfattarens korrekturroll till Granskare.



**Här är varför**

Med korrekturrollen som granskare kan du försäkra dig om att den som skapar korrekturet kan göra kommentarer och komma åt kommentarer som andra lämnar. För det mesta behöver inte den som skapat beviset fatta beslut om ett bevis som de har överfört. Alla korrekturroller för godkännare, granskare och godkännare, författare eller moderator kräver ett beslut. Om korrekturförfattaren tilldelas en av dessa korrekturroller men aldrig fattar något beslut, kan detta påverka korrekturernas deadlines negativt.

</br>
</br>

**Bästa praxis**

Undvik att använda korrekturrollen för godkännare.



**Här är varför**

Godkännarens korrekturroll tillåter inte användaren att kommentera det här korrekturet. Detta kan leda till att en användare avvisar korrekturet utan någon förklaring eftersom han/hon inte kunde göra några kommentarer. Använd korrekturrollen Granskare och godkännare i stället så att användaren kan ge feedback.

</br>
</br>

**Bästa praxis**

Undvik e-postaviseringsalternativet Alla aktivitetskorrektur.

**Här är varför**

Med det här alternativet skickas ett e-postmeddelande med korrektur varje gång något händer med ett korrektur - en kommentar görs, ett svar skickas, ett beslut fattas osv. Mottagaren ser i stort sett korrekturaktiviteten när den utförs.

För korrekturläsare och skapare fungerar e-postvarningen för beslut bäst för korrekturarbetsflöden i flera steg och det slutliga beslutet fungerar bäst för arbetsflöden i ett enda steg. I allmänhet kan alla andra anges till Inaktiverat, såvida de inte vill bli informerade om andra personer som gör kommentarer eller fattar beslut (i vilket fall ett av alternativen för att sammanfatta e-post kanske fungerar bäst).
