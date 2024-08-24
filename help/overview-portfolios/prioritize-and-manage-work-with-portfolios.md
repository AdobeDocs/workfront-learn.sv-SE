---
title: Använd [!UICONTROL Portfolio-optimering] för att prioritera och hantera arbete
description: Lär dig hur du använder [!UICONTROL Portfolio-optimering] för att prioritera och hantera projekt i en portfölj.
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: prioritize-and-manage-work-with-portfolios.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13835
role: User
level: Intermediate
hide: true
source-git-commit: d7347d41099e0faf6b47a6fe0e58091105e4e41d
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Använd [!UICONTROL Portfolio-optimering] för att prioritera och hantera arbete

Informationen som anges i [!UICONTROL Affärsärende] för varje projekt i din portfölj sammanställs till portföljen och till rubriken i avsnittet [!UICONTROL Optimering av Portfolio] .

![En bild av området [!UICONTROL Portfolio Optimizer] med information från [!UICONTROL Affärsfall]](assets/10-portfolio-management9.png)

Nu är det dags att använda den här informationen för att analysera vilka projekt som ska läggas på snabbspåret till produktionen och vilka som kan sitta vid sidan till nästa runda. Verktyget [!UICONTROL Optimering av Portfolio] är till stor hjälp.

[!UICONTROL Portfolio-optimering] kan hjälpa dig bäst om:

* [!UICONTROL Affärsärendet] har slutförts och skickats in för alla projekt.
* Du klickar på knappen [!UICONTROL Skicka] i [!UICONTROL Affärsärende] så att Workfront beräknar poängen för ett projekt.
* Du anger en budget som representerar det totala finansiella taket för de valda projekten.

## Optimeringskriterier

[!UICONTROL Portfolio-optimering] använder en standarduppsättning med villkor för att jämföra och prioritera projekt.

Dessa kriterier är följande:

* Låg kostnad
* Hög justering
* Högt värde
* Låg risk att dra nytta av
* Hög avkastning

När du klickar på ikonen Optimera öppnas en uppsättning skjutreglage som är kopplade till ett av villkoren. Du kan ange vilka villkor som ska ha högre prioritet genom att flytta skjutreglaget åt höger eller en lägre prioritet genom att trycka på skjutreglaget åt vänster.

![En bild av området [!UICONTROL Portfolio Optimizer] med information från [!UICONTROL Affärsfall]](assets/11-portfolio-management10.png)

Med hjälp av dessa kriterier genererar [!DNL Workfront] en projektpoäng mellan 1 och 100. Projekt med ett högre värde anger att de bättre justeras mot den riktning du vill att portföljen ska gå.

![En bild av området [!UICONTROL Portfolio Optimizer] med information om projektresultat](assets/12-portfolio-management14.png)

>[!NOTE]
>
>[!UICONTROL Portfolio-optimering] kommer inte att göra några poäng i projektet, även om alla avsnitt i [!UICONTROL affärsärendet] har fyllts i, såvida inte [!UICONTROL affärsärendet] har skickats till portföljen via [!DNL Workfront]. I stället för ett poängtal visas en varningssymbol i kolumnen [!UICONTROL Poäng] i [!UICONTROL Portfolio-optimering]. Håll muspekaren över varningssymbolen om du vill ha mer information om hur du betygsätter projektet.

![En bild av en varningssymbol i kolumnen [!UICONTROL Poäng] i [!UICONTROL Portfolio-optimering].](assets/13-portfolio-management12.png)

## Prioritera projekt

Nu när projekten har testats kan du snabbt och enkelt ordna om listan.

Genom att klicka på kolumnrubriken [!UICONTROL Poäng] sorteras projekten om och listas antingen från det högsta till det lägsta resultatet eller från det lägsta till det högsta. Du kan beställa projekt manuellt genom att klicka på fältikonen till vänster om talet och släppa projekten i den ordning du vill ha dem.

Det kan finnas projekt i listan som du inte vill jämföra. Om du inte vill se dem i listan avmarkerar du dem och döljer dem sedan genom att dra reglaget åt höger, så att knappens bakgrund är blå. Om du vill ta med de här projekten drar du reglaget åt vänster så att gråskalebilden visas.

![En bild av ett omarkerat projekt i [!UICONTROL Portfolio-optimering].](assets/14-portfolio-management13.png)

På så sätt kan du se bara de projekt du vill jämföra med varandra. När projekten har sorterats, filtrerats och sorterats kan ni nu fatta ett välgrundat beslut om huruvida ni behöver ändra kriterierna för att prioritera projekt.

Kom ihåg att [!DNL Workfront] skapade portföljerna och optimeringsverktyget för att underlätta processen att prioritera projekt. Du behöver dock inte använda de föreslagna villkoren. Om allt verktyget gör är att ge dig ett försprång eller en grund att jobba från, så är det bra.

Om projekten däremot ligger i prioritetsordning och du är redo att slutföra prioriteten i [!DNL Workfront] klickar du på knappen **[!UICONTROL Ange prioritet]** i det övre vänstra hörnet så numreras projekten från 1 upp och används för att ställa in fältet [!UICONTROL Portfolio prioritet] i varje projekt.

Om du vill behålla dessa siffror måste du klicka på knappen **[!UICONTROL Spara]** längst ned.

![En bild på hur du använder knappen [!UICONTROL Ange prioritet] för att prioritera projekt i [!UICONTROL Portfolio-optimering].](assets/15-portfolio-management15.png)

<!-- 
Pro-tips graphic
-->

* Du kan visa prioriteten för projekt enligt inställningen med [!UICONTROL Portfolio-optimering] i [!UICONTROL Resursplanering]. Klicka på ikonen **[!UICONTROL Inställningar]** och aktivera alternativet **[!UICONTROL Visa Portfolio-prioritet]**. Skärmen uppdateras och portföljens prioriteringar visas i den vänstra kolumnen. Klicka på alternativet **[!UICONTROL Beställning]** längst upp i kolumnen om du vill justera prioriteterna för [!UICONTROL Resursplanering] efter portföljens prioriteringar. Glöm inte att spara när du är klar.

  ![En bild av kolumnen [!UICONTROL Portfolio Prioriteter] i [!UICONTROL Resursplaneraren].](assets/16-portfolio-management17.png)

## Hantera ändringar

Portfolio är definitivt inte ett botemedel, men de kan minska smärtan av förändrade prioriteringar. Det som en gång tog dagar kan nu ta timmar eller till och med några minuter.

När nya projekt läggs till i en portfölj måste de fortfarande analyseras och prioriteras. Genom att använda [!UICONTROL Affärsärende] och optimeringspoängen kan du enkelt jämföra nya projekt med begärda, planerade och aktuella projekt.

![En bild av projektkolumnen [!UICONTROL Status] i [!UICONTROL Portfolio-optimering].](assets/17-project-management16.png)

Om du under jämförelsen ser att nya projekt bör ha högre prioritet kan du antingen sortera om listan baserat på optimeringspoängen eller dra och släppa dem högre upp i listan. När du är klar klickar du bara på knappen **[!UICONTROL Ange prioritet]**, sparar så är jobbet klart.

<!-- Learn more graphic and documentation article links

* Portfolio Optimizer overview 
* Optimize projects in the Portfolio Optimizer 
* Overview of the Portfolio Optimizer score 
* Prioritizing projects in the Portfolio Optimizer

-->
