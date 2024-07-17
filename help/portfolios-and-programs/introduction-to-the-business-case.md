---
title: Förstå [!UICONTROL affärsärendet]
description: Lär dig hur du använder [!UICONTROL affärsärendet] i Workfront för att utvärdera begärda projekt och jämföra dem med andra projekt i din portfölj.
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: introduction-to-the-business-case.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13836
role: User
level: Intermediate
exl-id: febb7378-81d4-4348-ac57-e9c4756966c0
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Förstå [!UICONTROL affärsärendet]

Som chef är det ditt mål att se till att projekten bidrar till företagets övergripande mål och initiativ på ett positivt sätt. För att kunna fatta välgrundade beslut behöver du information från projektledarna om vad de behöver för att kunna gå vidare med sina projekt. Detta kan du göra genom [!UICONTROL affärsärendet].

## Vad är ett [!UICONTROL affärsärende]?

Tänk på ett [!UICONTROL affärsärende] som en plan eller ett förslag för det arbete som behöver utföras. Den innehåller preliminära uppskattningar på hög nivå som hjälper er att planera och hantera portföljer. Det är där potentiella kostnader, resurser och risker läggs in för att skapa ett&quot;fall&quot; för varför projektet skulle gynna företaget.

## [!UICONTROL Affärsfall]-fält rekommenderas för projektprioritering

Varje avsnitt i [!UICONTROL affärsärendet] innehåller unik och viktig information om projektet. Låt oss titta på avsnitten som matar in information till verktyget [!UICONTROL Portfolio Optimizer] som hjälper dig att prioritera projekten i din portfölj.

## [!UICONTROL Projektinformation]

Den mesta informationen som anges i avsnittet [!UICONTROL Projektinformation] omfattar allmän projektinformation, till exempel projektets sponsor och det program som projektet tillhör.

Det finns dock en informationsdel som kan påverka projektets prioritering -[!UICONTROL Planerad förmån].

![En bild av området [!UICONTROL Planerad förmån] i avsnittet [!UICONTROL Projektinformation] i [!UICONTROL Affärsärende]](assets/05-portfolio-management4.png)

Den [!UICONTROL planerade förmånen] representerar det beräknade belopp som ditt företag kan ha nytta av om projektet har slutförts.

Det här är ett av avsnitten som kan vara en startpunkt för att få ditt företag att gå framåt med det här projektet. Om du kan visa att projektet kommer att bidra avsevärt till företagets resultat, är chansen högre att projektet kommer att föras vidare snabbare.

## [!UICONTROL Utgifter]

[!UICONTROL Utgifter] representerar icke-arbetskostnader som kan uppstå under ett projekts livslängd.

![En bild av avsnittet [!UICONTROL Utgifter] i [!UICONTROL Affärsärende]](assets/06-portfolio-management5.png)

Exempelvis kan utgifter för en användarkonferens omfatta betalning för en plats, artiklar för presentväskor eller skyltar för en handelsplatslobby.

## [!UICONTROL Resursbudgetering]

I avsnittet [!UICONTROL Resursbudgetering] kan du beräkna vilken arbetsinsats du tror kommer att behövas för att projektet ska kunna gå vidare. Informationen hämtas från [!DNL Workfront's] [!UICONTROL Resursplanering].

![En bild av avsnittet [!UICONTROL Resursbudgetering] i [!UICONTROL Affärsärende]](assets/07-portfolio-management6.png)

Genom att ange beräknade behov för varje jobbroll skapar detta en möjlig budget som behövs för projektet och ger insikt i hur stor del av portföljens budget som kan användas för projektet.

>[!NOTE]
>
>Du måste ha konfigurerade resurspooler i [!DNL Workfront] för att kunna använda det här avsnittet av [!UICONTROL affärsärendet].

## [!UICONTROL Risker]

Du hoppas alltid att projektet kommer att flyta smidigt. Men det är viktigt att identifiera risker och planera för dem därefter. Det är där avsnittet [!UICONTROL Risker] i [!UICONTROL Affärsärende] kan hjälpa.

![En bild av avsnittet [!UICONTROL Risker] i [!UICONTROL Affärsärende]](assets/08-portfolio-management7.png)

Du borde brainstorma med ditt team och identifiera eventuella risker för projektet. För risker där du kan uppskatta kostnaden om risken uppstår och sannolikheten för att den inträffar, ska du vara säker och ange dessa värden. Workfront multiplicerar den potentiella kostnaden med sannolikheten och placerar den i en [!UICONTROL potentiell risk]-fond som subtraheras från projektets [!UICONTROL planerade förmån] när dess [!UICONTROL nettovärde] beräknas.

## [!UICONTROL Styrkort]

[!UICONTROL Med styrkort] kan du avgöra hur väl ett föreslaget projekt passar ihop med de övergripande mål och initiativ som angetts för antingen portföljen eller företaget.

Varje styrkort har en lista med frågor och svar som har värden kopplade till sig. När styrkortet har fyllts i kan [!DNL Workfront] beräkna hur justerat projektet är med organisationens förbestämda mål.

![En bild av avsnittet [!UICONTROL Styrkort] i [!UICONTROL Affärsärende]](assets/09-portfolio-management8.png)

>[!NOTE]
>
>Projektledare kan inte se de värden som tilldelats varje svar. Endast användare som skapar styrkort kan se värdena.

## [!UICONTROL Affärsärende] krävs inte

[!UICONTROL Affärsärendet] är flexibelt. Du kan fylla i bara några få avsnitt eller inga alls. Inget av fälten är obligatoriska. Men ju mer information du fyller i desto enklare är det att analysera och prioritera projekt som varierar för samma budget eller resurser.

När [!UICONTROL Affärsärende] har fyllts i klickar du på knappen **[!UICONTROL Skicka]** på sammanfattningspanelen till höger i fönstret. Detta ändrar projektstatus till [!UICONTROL Begärd]. Nu kan du använda [!UICONTROL Portfolio-optimering] för att prioritera projekt i samma portfölj.

>[!NOTE]
>
>Justeringspoängen i sammanfattningspanelen [!UICONTROL Affärsärende] genereras när du fyller i styrkortet. Justeringspoängen är ett av de värden som används för att beräkna poängen för [!UICONTROL Portfolio Optimizer].

<!-- 
Learn more graphic and links to documentation articles
* Overview of areas of the business case 
* Create a business case for a project   
* Create a scorecard 
* Apply a scorecard to a project and generate an alignment score 
-->
