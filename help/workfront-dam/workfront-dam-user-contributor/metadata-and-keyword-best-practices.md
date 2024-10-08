---
title: Förstå metadata och nyckelordsrutiner
description: Lär dig hur du använder metadata och nyckelord i [!UICONTROL Workfront DAM] för att beskriva en resurs och öka sökbarheten för organisationens resurser.
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
jira: KT-10107
exl-id: ad5a19a7-556a-4b38-9cc4-7e29e5afe1de
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Förstå metadata och nyckelordsrutiner

## Metadata best practices

Metadata är alla data som används för att beskriva en tillgång. Metadatafält har ett namn och användare kan redigera eller ändra informationen i många av dessa fält. Vissa metadatafält fylls i av programmet eller enheten som resursen kom från och kan inte redigeras.

Om du använder konsekventa metadata blir det lättare att söka efter organisationens resurser. Dessutom behåller resurser som hämtats från [!UICONTROL Workfront DAM] sina metadata, vilket ger ett annat skyddslager för dina resurser om de lämnar [!UICONTROL Workfront DAM].

Här följer några tips om hur du kan använda din organisations metadatainsatser:

* Lägg alltid till ägar- eller kreditinformation till dina resurser för identifiering utanför [!UICONTROL Workfront DAM].
* Lägg till användningsvillkor för rättighetshanterade resurser för att förhindra missbruk.
* Lägg till metadata i dina resurser så snart du överför dem.
* Implementera fördefinierade listrutemenyer för vanliga data för att förhindra inkonsekvenser.
* Utbilda medarbetare som ansvarar för att lägga till metadata i organisationens metadatastrategi.
* Informera externa leverantörer om dina metadatakrav (t.ex. måste fotona skickas in med användarvillkor, krediter och platsmetadata redan tillagda).
* Genomför regelbundna granskningar för att säkerställa att metadata läggs till korrekt.

## Metadatastrategi

Organisationen har förmodligen utvecklat en metadatastrategi. Om du överför resurser till [!UICONTROL Workfront DAM] bör du ta reda på hur din organisation hanterar:

* Vem ansvarar för att lägga till metadata.
* Vilka metadata krävs.
* När läggs metadata till.
* Hur ofta söks resurser efter korrekta metadata.
* Vem ansvarar för metadatakontrollerna.

## Bästa praxis för nyckelord

Nyckelord är en delmängd av metadata. Nyckelord är ofta generiska, beskrivande termer om innehållet i resursen. Den här informationen läggs till i resursen, ofta manuellt efter överföringen. Alla nyckelord placeras i ett fält (kallas nyckelord). Ett foto på Eiffeltornet i Paris kan t.ex. innehålla nyckelord som landmärke, turism eller ljus.

Nyckelord är sökbara, så det är viktigt att nyckelord anges på resurser på ett konsekvent sätt.

Din organisation kan implementera en nyckelordstonomi, som är en kontrollerad lista med nyckelord som du kan välja mellan när du redigerar en resurs i [!UICONTROL Workfront DAM].

Om din organisation tillåter dig att ange nyckelord manuellt bör du tänka på dessa tips.

* Var konsekvent med akronymer och förkortningar. Använd inte nyckelord för en resurs med&quot;AZ&quot; och en annan resurs med&quot;Arizona&quot;.
* Var konsekvent i plural jämfört med singular. Välj ett format eller använd alltid båda. Använd till exempel &quot;fötter&quot; och &quot;händer&quot; eller &quot;fot, fötter&quot; och &quot;hand, händer&quot;.
* Var konsekvent i hur du beskriver en åtgärd eller aktivitet, t.ex. använd&quot;springa&quot; och&quot;simma&quot; eller&quot;run&quot; och&quot;simma&quot;.
* Var inte för smal. &quot;Keokuk, IA&quot; kan vara för smalt för ett nyckelord och helt oidentifierbart för användarna. &quot;Southeast Iowa&quot; vore bättre.
* Var inte för bred. &quot;Universitet&quot; kanske inte fungerar, särskilt inte om allt i ditt system gäller ett universitet. Bestäm vad som ska skilja på resurserna, till exempel ett specifikt kollegienamn.
* Var uppmärksam på relevansen. Bara för att varje resurs har en projektkod betyder det inte att den är användbar för användare som använder nyckelord för att hitta resurser. Om den här informationen behöver behållas med resursen kan du lägga till den i ett annat metadatafält.
* Använd inte för få nyckelord, annars hjälper de inte till att begränsa sökresultaten.
* Förlita dig inte på nyckelord för varje datadel. Använd metadatafält för information som fotografens namn eller plats.
