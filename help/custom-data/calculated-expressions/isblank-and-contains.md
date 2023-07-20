---
title: Använd uttrycken ISBLANK och CONTAINS
description: Lär dig hur du använder och skapar ISBLANK- och CONTAINS-uttrycken i ett beräkningsfält i Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Använd uttrycken ISBLANK och CONTAINS

Både CONTAINS- och ISBLANK-uttrycken används för att ge enkla true- eller false-värden. Skillnaden är att ISBLANK-uttrycket kontrollerar om fältet innehåller ett värde alls medan CONTAINS-textuttrycket söker efter en viss sträng i ett fält.

Om du till exempel vill se om ett projekt har en beskrivning använder du uttrycket ISBLANK. Om beskrivningsfältet är tomt returnerar uttrycket värdet true. Om beskrivningsfältet inte är tomt returneras värdet false.

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/isblank01.png)

Om du vill söka efter ett specifikt värde i beskrivningen, t.ex.&quot;välgörenhetshändelse&quot;, använder du textuttrycket CONTAINS. Om det finns en&quot;välgörenhetshändelse&quot; i beskrivningen, anges&quot;true&quot; i beräkningsfältet. &quot;false&quot; visas om det inte finns någon &quot;välgörenhetshändelse&quot;.

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/isblank02.png)

## ISBLANK

Textuttrycket ISBLANK innehåller namnet på uttrycket och en datapunkt.

**ISBLANK({datapunkt})**

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/isblank03.png)

I exemplet ovan, där du vill veta om projektet har en beskrivning, skulle uttrycket vara:

ISBLANK({description})

## INNEHÅLLER

I CONTAINS-textuttrycket ingår namnet på uttrycket, ordet eller frasen som du söker efter och fältet som ska sökas in.

**CONTAINS(&quot;fras&quot;,{fields})**

Se till att placera citattecken runt ordet eller frasen du söker efter, annars är uttrycket inte giltigt.

I exemplet ovan (söker efter&quot;välgörenhetshändelse&quot; i projektbeskrivningen) skulle uttrycket vara:

**CONTAINS(&quot;välgörenhetshändelse&quot;),{description})**

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/isblank04.png)

**Anteckning**: CONTAINS-uttrycket är skiftlägeskänsligt. Om&quot;välgörenhetshändelse&quot; till exempel har inledande versal i beskrivningsfältet, ska frasen ha inledande versal i uttrycket.

**CONTAINS(&quot;välgörenhetshändelse&quot;),{description})**

Uttrycken ISBLANK och CONTAINS är bra att använda om du vill se om det finns ett värde. Det kan dock vara mer användbart att veta vad värdet är, att faktiskt se det eller att ha någon typ av beskrivning för att få bättre insikt.

I stället för att bara veta att ett projekt har konverterats från en begäran vill du till exempel veta namnet på den ursprungliga begäran.

I så fall använder du CONTAINS-uttrycket tillsammans med ett IF-uttryck.

Oftast används textuttrycken ISBLANK och CONTAINS med ett IF-textuttryck.
