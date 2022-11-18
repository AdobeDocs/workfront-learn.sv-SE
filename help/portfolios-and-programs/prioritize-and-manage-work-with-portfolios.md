---
title: Prioritera och hantera material med portfolior
description: Lär dig att prioritera och hantera arbete med portföljer i [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: prioritize-and-manage-work-with-portfolios.png
type: Tutorial
role: User
level: Intermediate
exl-id: b8b91ae8-f0e1-4cab-bf2c-6b8ca9746ea3
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# Prioritera och hantera material med portfolior

All information som anges i [!UICONTROL Affärsärende] läggs upp till portföljen och till standardvyn i [!UICONTROL Optimering för Portfolio] -avsnitt.

![En bild av [!UICONTROL Portfolio Optimizer] område med information från [!UICONTROL Affärsärende]](assets/10-portfolio-management9.png)

Nu är det dags att använda den här informationen för att analysera vilka projekt som ska läggas på snabbspåret till produktionen och vilka som kan sitta vid sidan och fram till nästa runda. The [!UICONTROL Optimering för Portfolio] kommer att hjälpa till enormt med det.

The [!UICONTROL Portfolio Optimizer] kan hjälpa dig på bästa sätt om:

* The [!UICONTROL Affärsärende] har slutförts och lämnats in för projekten.
* Samma portfölj definieras för de projekt som du vill jämföra.
* Du anger en budget som representerar det totala finansiella taket för de valda projekten.

## Optimeringskriterier

När du öppnar en portfölj visas ett alternativ på den vänstra panelmenyn som heter [!UICONTROL Optimering för Portfolio]. Det här verktyget använder en standarduppsättning med kriterier för att jämföra och prioritera projekt.

Dessa kriterier är följande:

* Låg kostnad
* Hög justering
* Högt värde
* Låg risk att dra nytta av
* Hög avkastning

När du klickar på ikonen Optimera öppnas en uppsättning skjutreglage som är kopplade till ett av villkoren. Du kan ange vilka villkor som ska ha högre prioritet genom att flytta skjutreglaget åt höger eller en lägre prioritet genom att trycka på skjutreglaget åt vänster.

![En bild av [!UICONTROL Portfolio Optimizer] område med information från [!UICONTROL Affärsärende]](assets/11-portfolio-management10.png)

Med hjälp av dessa kriterier [!DNL Workfront] genererar ett poängvärde mellan 1 och 100. Projekt med ett högre värde anger att de bättre justeras mot den riktning du vill att portföljen ska gå.

![En bild av [!UICONTROL Portfolio Optimizer] område med information om projektpoäng](assets/12-portfolio-management14.png)

>[!NOTE]
>
>The [!UICONTROL Portfolio Optimizer] kommer inte att få projektet att spelas upp, även om alla avsnitt i [!UICONTROL Affärsärende] fylls i, såvida inte [!UICONTROL Affärsärende] har skickats till portföljen via [!DNL Workfront]. I stället för ett musikspår visas en varningssymbol i [!UICONTROL Poäng] kolumn i [!UICONTROL Portfolio Optimizer]. Håll pekaren över varningssymbolen för att se vilka delar av [!UICONTROL Affärsärende] måste fyllas i så att du kan göra det.

![En bild av en varningssymbol i [!UICONTROL Poäng] kolumn i [!UICONTROL Portfolio Optimizer].](assets/13-portfolio-management12.png)

## Prioritera projekt

Nu när projekten har testats kan du snabbt och enkelt ordna om listan.

Genom att klicka på [!UICONTROL Poäng] kolumnrubriken sorteras projekten om och visas antingen från det högsta till det lägsta resultatet eller från det lägsta till det högsta. Du kan också ordna projekt manuellt genom att klicka på fältikonen till vänster om talet och släppa projekten i den ordning du vill ha dem.

Det kan finnas projekt i listan som du inte vill jämföra. Om du inte vill se dem i listan avmarkerar du dem och döljer dem sedan genom att dra reglaget åt höger, så att knappens bakgrund är blå. Om du vill ta med de här projekten drar du reglaget åt vänster så att gråskalebilden visas.

![En bild av ett omarkerat projekt i [!UICONTROL Portfolio Optimizer].](assets/14-portfolio-management13.png)

På så sätt kan du se bara de projekt du vill jämföra med varandra. När projekten har sorterats, filtrerats och sorterats kan ni nu fatta ett välgrundat beslut om huruvida ni behöver ändra kriterierna för att prioritera projekt.

Kom ihåg: [!DNL Workfront] har byggt upp portföljerna och optimeringsverktyget för att underlätta processen att prioritera projekt. Du behöver dock inte använda de föreslagna villkoren. Om allt verktyget gör är att ge dig ett försprång eller en grund att arbeta utifrån, så är det bra.

Om projekten ligger i prioritetsordning och du är redo att slutföra prioriteringen i [!DNL Workfront]klickar du på **[!UICONTROL Ange prioritet]** i det övre vänstra hörnet så numreras projekten från 1 upp och det numret används för att ställa in [!UICONTROL Portfolio Prioritet] i varje projekt.

Om du vill behålla dessa siffror måste du klicka på **[!UICONTROL Spara]** längst ned.

![En bild som använder [!UICONTROL Ange prioritet] för att prioritera projekt i [!UICONTROL Portfolio Optimizer].](assets/15-portfolio-management15.png)

<!-- 
Pro-tips graphic
-->

* Du kan visa prioriteten för projekt enligt inställningen via [!UICONTROL Portfolio Optimizer] i [!UICONTROL Resursplanering]. Klicka på **[!UICONTROL Inställningar]** och aktivera **[!UICONTROL Visa Portfolio-prioriteringar]** alternativ. Skärmen uppdateras och portföljens prioriteringar visas i den vänstra kolumnen. Klicka på **[!UICONTROL Order]** alternativ längst upp i kolumnen för att justera [!UICONTROL Resursplanering] Prioriteringar med portföljens prioriteringar. Glöm inte att spara när du är klar.

   ![En bild av [!UICONTROL Prioriteringarna i Portfolio] kolumn i [!UICONTROL Resursplanering].](assets/16-portfolio-management17.png)

## Hantera ändringar

Portfolio är definitivt inte ett botemedel, men de kan minska smärtan av förändrade prioriteringar. Det som en gång tog dagar kan nu ta timmar eller till och med några minuter.

När nya projekt läggs till i en portfölj måste de fortfarande analyseras och prioriteras. Genom att använda [!UICONTROL Affärsärende] och optimeringspoängen kan du enkelt jämföra nya projekt med begärda, planerade och aktuella projekt.

![En bild av projektet [!UICONTROL Status] kolumn i [!UICONTROL Portfolio Optimizer].](assets/17-project-management16.png)

Om du under jämförelsen ser att nya projekt bör ha högre prioritet kan du antingen sortera om listan baserat på optimeringspoängen eller dra och släppa dem högre upp i listan. När du är klar klickar du bara på **[!UICONTROL Ange prioritet]** , spara och jobbet är klart.

<!-- Learn more graphic and documentation article links

* Portfolio Optimizer overview 
* Optimize projects in the Portfolio Optimizer 
* Overview of the Portfolio Optimizer score 
* Prioritizing projects in the Portfolio Optimizer

-->
