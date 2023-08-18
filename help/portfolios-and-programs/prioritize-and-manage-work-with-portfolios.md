---
title: Använd [!UICONTROL Portfolio Optimizer] att prioritera och hantera arbete
description: Lär dig använda [!UICONTROL Portfolio Optimizer] att prioritera och hantera projekt i en portfölj.
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: prioritize-and-manage-work-with-portfolios.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13835
role: User
level: Intermediate
exl-id: b8b91ae8-f0e1-4cab-bf2c-6b8ca9746ea3
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Använd [!UICONTROL Portfolio Optimizer] att prioritera och hantera arbete

Informationen som anges i [!UICONTROL Affärsärende] för varje projekt i din portfölj omvandlas till portföljen och till rubriken i [!UICONTROL Optimering för Portfolio] -avsnitt.

![En bild av [!UICONTROL Portfolio Optimizer] område med information från [!UICONTROL Affärsärende]](assets/10-portfolio-management9.png)

Nu är det dags att använda den här informationen för att analysera vilka projekt som ska läggas på snabbspåret till produktionen och vilka som kan sitta vid sidan till nästa runda. The [!UICONTROL Optimering för Portfolio] kommer att hjälpa till enormt med det.

The [!UICONTROL Portfolio Optimizer] kan hjälpa dig på bästa sätt om:

* The [!UICONTROL Affärsärende] har slutförts och skickats in för alla projekt.
* Du klickar på [!UICONTROL Skicka] knappen i [!UICONTROL Affärsärende] så att Workfront beräknar poängen för ett projekt.
* Du anger en budget som representerar det totala finansiella taket för de valda projekten.

## Optimeringskriterier

The [!UICONTROL Portfolio Optimizer] använder en standarduppsättning med kriterier för att jämföra och prioritera projekt.

Dessa kriterier är följande:

* Låg kostnad
* Hög justering
* Högt värde
* Låg risk att dra nytta av
* Hög avkastning

När du klickar på ikonen Optimera öppnas en uppsättning skjutreglage som är kopplade till ett av villkoren. Du kan ange vilka villkor som ska ha högre prioritet genom att flytta skjutreglaget åt höger eller en lägre prioritet genom att trycka på skjutreglaget åt vänster.

![En bild av [!UICONTROL Portfolio Optimizer] område med information från [!UICONTROL Affärsärende]](assets/11-portfolio-management10.png)

Dessa kriterier används [!DNL Workfront] genererar en projektpoäng mellan 1 och 100. Projekt med ett högre värde anger att de bättre justeras mot den riktning du vill att portföljen ska gå.

![En bild av [!UICONTROL Portfolio Optimizer] område med information om projektpoäng](assets/12-portfolio-management14.png)

>[!NOTE]
>
>The [!UICONTROL Portfolio Optimizer] kommer inte att få projektet att spelas upp, även om alla avsnitt i [!UICONTROL Affärsärende] fylls i, såvida inte [!UICONTROL Affärsärende] har skickats till portföljen via [!DNL Workfront]. I stället för ett musikspår visas en varningssymbol i [!UICONTROL Poäng] kolumn i [!UICONTROL Portfolio Optimizer]. Håll muspekaren över varningssymbolen om du vill ha mer information om hur du betygsätter projektet.

![En bild av en varningssymbol i [!UICONTROL Poäng] kolumn i [!UICONTROL Portfolio Optimizer].](assets/13-portfolio-management12.png)

## Prioritera projekt

Nu när projekten har testats kan du snabbt och enkelt ordna om listan.

Klicka på [!UICONTROL Poäng] kolumnrubriken sorteras projekten om och visas antingen från det högsta till det lägsta resultatet eller från det lägsta till det högsta. Du kan beställa projekt manuellt genom att klicka på fältikonen till vänster om talet och släppa projekten i den ordning du vill ha dem.

Det kan finnas projekt i listan som du inte vill jämföra. Om du inte vill se dem i listan avmarkerar du dem och döljer dem sedan genom att dra reglaget åt höger, så att knappens bakgrund är blå. Om du vill ta med de här projekten drar du reglaget åt vänster så att gråskalebilden visas.

![En bild av ett omarkerat projekt i [!UICONTROL Portfolio Optimizer].](assets/14-portfolio-management13.png)

På så sätt kan du se bara de projekt du vill jämföra med varandra. När projekten har sorterats, filtrerats och sorterats kan ni nu fatta ett välgrundat beslut om huruvida ni behöver ändra kriterierna för att prioritera projekt.

Kom ihåg: [!DNL Workfront] har byggt upp portföljerna och optimeringsverktyget för att underlätta processen att prioritera projekt. Du behöver dock inte använda de föreslagna villkoren. Om allt verktyget gör är att ge dig ett försprång eller en grund att jobba från, så är det bra.

Om projekten ligger i prioritetsordning och du är redo att slutföra prioriteringen i [!DNL Workfront]klickar du på **[!UICONTROL Ange prioritet]** i det övre vänstra hörnet så numreras projekten från 1 upp och det numret används för att ställa in [!UICONTROL Portfolio Prioritet] i varje projekt.

Om du vill behålla dessa siffror måste du klicka på **[!UICONTROL Spara]** längst ned.

![En bild som använder [!UICONTROL Ange prioritet] för att prioritera projekt i [!UICONTROL Portfolio Optimizer].](assets/15-portfolio-management15.png)

<!-- 
Pro-tips graphic
-->

* Du kan visa prioriteten för projekt enligt inställningen via [!UICONTROL Portfolio Optimizer] i [!UICONTROL Resursplanering]. Klicka på **[!UICONTROL Inställningar]** ikonen och aktivera **[!UICONTROL Visa Portfolio-prioriteringar]** alternativ. Skärmen uppdateras och portföljens prioriteringar visas i den vänstra kolumnen. Klicka på **[!UICONTROL Beställning]** alternativ längst upp i kolumnen för att justera [!UICONTROL Resursplanering] Prioriteringar med portföljens prioriteringar. Glöm inte att spara när du är klar.

  ![En bild av [!UICONTROL Prioriteringarna i Portfolio] kolumn i [!UICONTROL Resursplanering].](assets/16-portfolio-management17.png)

## Hantera ändringar

Portfolio är definitivt inte ett botemedel, men de kan minska smärtan av förändrade prioriteringar. Det som en gång tog dagar kan nu ta timmar eller till och med några minuter.

När nya projekt läggs till i en portfölj måste de fortfarande analyseras och prioriteras. Genom att använda [!UICONTROL Affärsärende] och optimeringspoängen kan du enkelt jämföra nya projekt med begärda, planerade och aktuella projekt.

![En bild av projektet [!UICONTROL Status] kolumn i [!UICONTROL Portfolio Optimizer].](assets/17-project-management16.png)

Om du under jämförelsen ser att nya projekt bör ha högre prioritet kan du antingen sortera om listan baserat på optimeringspoängen eller dra och släppa dem högre upp i listan. Klicka bara på **[!UICONTROL Ange prioritet]** , spara och jobbet är klart.

<!-- Learn more graphic and documentation article links

* Portfolio Optimizer overview 
* Optimize projects in the Portfolio Optimizer 
* Overview of the Portfolio Optimizer score 
* Prioritizing projects in the Portfolio Optimizer

-->
