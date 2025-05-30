---
title: Avancerad aggregeringsövning
description: Ring en webbtjänst för att returnera information om flera länder och identifiera populationen, grupperad efter underregion.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
recommendations: noDisplay,catalog
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Avancerad aggregeringsövning

Lär dig hur du använder grupperingar när du aggregerar.

## Översikt över övningar

Ring en webbtjänst om du vill returnera information om flera länder och identifiera den totala befolkningen i alla länder, grupperade efter underregion.

![Avancerad aggregeringsbild 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## Steg som ska följas

**Hämta landsuppgifter.**

![Avancerad aggregeringsbild 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. Skapa ett nytt scenario och ge det namnet&quot;Avancerad aggregering&quot;.
1. Ställ in utlösarmodulen på en HTTP - Gör en begärandemodul.
1. Använd den här URL:en, `https://restcountries.com/v2/lang/es`, som ger dig en lista över alla länder där spanska talas.
1. Låt metoden vara Get.
1. Klicka i kryssrutan Tolka svar.
1. Byt namn på den här modulen till Hämta länder.
1. Klicka på Spara och kör en gång.

   **Utdata är ett enskilt paket, men de ingår i en array med 24 samlingar, en för varje spansktalande land.**

   ![Avancerad aggregeringsbild 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **Du måste samla in underregionsinformation för vart och ett av länderna, så du måste göra en ytterligare HTTP-begäran.**

1. Lägg till ytterligare en begäran om att få information om underregioner. Det kommer bara att återlämna det första landet, men det är okej för tillfället. Lägg till ytterligare en HTTP Gör en begärandemodul och använd URL `https://restcountries.com/v2/name/{country name}`.
1. Om du vill hämta namnet på det första landet går du till mappningspanelen och klickar på Data och sedan på Namn i arrayen. [1] i datafältet betyder att det returnerar det första objektet i arrayen.

   + Klicka på numret och ändra indexet om det behövs, men i det här fallet vill du bara ha det första objektet.

![Avancerad aggregeringsbild 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. Markera Analysera svar på mappningspanelen och klicka sedan på OK.
1. Byt namn på&quot;Hämta landsuppgifter&quot;.
1. Klicka på Spara och sedan Kör en gång.

   + Resultatet är information för ett enskilt land.

1. Om du vill få de andra länderna måste du iterera genom arrayen. Lägg till en iterator, som tar en lista över saker och matar ut ett paket för varje objekt i listan.

   **Lägg till iteratorn och aggregatorn.**

1. Högerklicka mellan HTTP-modulerna och lägg till Iterator Flow Control-modulen.
1. Välj Data i modulen Hämta länder i fältet Array.

   ![Avancerad aggregeringsbild 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. I modulen Hämta landsuppgifter uppdaterar du URL-fältet så att det tar namnfältet från iteratorn i stället för från modulen Hämta länder.

   ![Avancerad aggregeringsbild 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. Lägg nu till en numerisk aggregator efter Hämta landsuppgifter för att gruppera och summera populationerna.
1. Källmodulen är iteratorn.
1. Sammanställningsfunktionen är SUM.
1. Värdet är [data:population] från modulen Hämta landsuppgifter.
1. Klicka på alternativet Visa avancerade inställningar längst ned och gruppera efter [data:subregion] i modulen Hämta landsuppgifter.

   ![Avancerad aggregeringsbild 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **Slutför med en textaggregator för att sammanställa det du grupperade i den numeriska aggregatorn.**

1. Lägg till en textaggregator i slutet.
1. Källmodulen är den numeriska aggregatorn.
1. I textområdet infogar du &quot;Den totala populationen av [KEY] är [result].&quot;

   ![Avancerad aggregeringsbild 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. Spara och kör en gång.

   + Granska utdata från den sista modulen.
