---
title: Skapa ett begärandeflöde
description: Optimera hanteringen av förfrågningar genom att skapa hanteringsregler för effektiva tilldelningar, organisera förfrågningar med kapslade ämnesgrupper, länka köämnen till arbetsflöden, testa funktionen för begärandeflöde och göra flexibla justeringar för att säkerställa exakthet och effektivitet.
activity: deploy
feature: Work Management
type: Tutorial
role: Admin, User
level: Intermediate
team: Technical Marketing
thumbnail: 335223.jpeg
jira: KT-8960
last-substantial-update: 2024-09-11T00:00:00Z
recommendations: noDisplay,catalog
exl-id: 194df349-541d-4940-a6a5-b5d47cb58cf4
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Skapa ett begärandeflöde

>[!PREREQUISITES]
>
>* [Skapa en begärandekö](/help/manage-work/request-queues/create-a-request-queue.md)
>* [Förstå inställningarna för ett begärandeflöde](/help/manage-work/request-queues/understand-settings-for-a-flow-request.md)

I den här videon får du en stegvis guide om hur du skapar ett begärandeflöde genom att konfigurera köämnen, ämnesgrupper och routningsregler. &#x200B; Processen börjar med att skapa routningsregler som definierar hur begäranden tilldelas. &#x200B; Därefter skapas ämnesgrupper för att organisera begäranden. &#x200B; Dessa grupper kan läggas till i köer och det finns ingen gräns för hur många ämnesgrupper som kan skapas.
I videon visas sedan hur du skapar köämnen, som är länkade till routningsregler, ämnesgrupper, anpassade formulär, godkännandeprocesser och standardtider.
Slutligen visar videon hur du testar konfigurationen genom att skicka en begäran för att säkerställa att den dirigeras korrekt. &#x200B; Om det uppstår problem kan du justera kön. &#x200B; I videon betonas vikten av att verifiera strukturen och funktionaliteten i begärandeflödet för att säkerställa korrekt routning och organisation.

>[!VIDEO](https://video.tv.adobe.com/v/3433826/?quality=12&learn=on&captions=swe)

## Viktiga uppgifter

* **Konfigurering av routningsregler:** Routningsregler avgör hur begäranden tilldelas, oavsett om de tilldelas till team (t.ex. Creative team) eller enskilda (t.ex. Jennifer Campbell eller Mark Lewis). &#x200B; Dessa regler skapas genom att de namnges, beskrivningar läggs till och standardtilldelningar eller -team väljs.
* **Skapa ämnesgrupper:** Med ämnesgrupper kan du ordna förfrågningar i kategorier som &quot;Digital&quot; och &quot;Skriv ut&quot; &#x200B; Det finns ingen gräns för hur många ämnesgrupper som kan skapas, och de kan kapslas upp till 10 nivåer djupt.
* **Konfiguration av köämnen:** Köämnen är länkade till routningsregler, ämnesgrupper, anpassade formulär, godkännandeprocesser och standardtider. &#x200B; Ett köämne med namnet&quot;Broschyrer&quot; kan till exempel kopplas till ämnesgruppen Skriv ut och dirigeras till Creative team.
* **Testar begärandeflödet:** När begärandekön har konfigurerats är det viktigt att testa flödet genom att skicka en begäran för att säkerställa korrekt routning och funktionalitet. &#x200B; Alla problem kan åtgärdas genom att köinställningarna görs om. &#x200B;
* **Flexibilitet i justeringar:** Systemet tillåter ändringar i routningsregler, ämnesgrupper och köämnen om det finns något som inte passar, vilket säkerställer att förfrågningsflödet förblir effektivt och korrekt.


## Rekommenderade självstudiekurser i detta ämne

* [Skapa en kö för feedback från systemadministratörer](/help/manage-work/request-queues/create-a-system-admin-feedback-request-queue.md)
* [Svar på vanliga frågor om begärandeköer](/help/manage-work/request-queues/request-queue-faq.md)


