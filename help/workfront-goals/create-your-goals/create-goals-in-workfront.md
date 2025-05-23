---
title: Skapa mål
description: Lär dig hur du skapar mål i [!DNL Workfront Goals] med tre olika alternativ.
activity: use
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-10122
doc-type: video
exl-id: 784b353f-cc6b-4a4b-9935-9e5d25c532b4
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Skapa mål

I [!DNL Workfront Goals] kan chefer och företagsledare se hur hela organisationen utvecklas på varje nivå, ända ned till individen. [!DNL Workfront Goals] ger synlighet så att du kan få viktiga åtgärdbara insikter för att förbättra de högsta prioriteterna, identifiera riskmål, diagnostisera problem i realtid och proaktivt kurskorrigera.

[!DNL Workfront Goals] tillåter även enskilda medarbetare att se hur deras arbete bidrar till helheten. Arbetet är mer meningsfullt när individer kan se var deras arbete är viktigt.

Det finns tre sätt att skapa mål med [!DNL Workfront]:

## Skapa ett helt nytt mål

Här är några saker att tänka på när du skapar mål från grunden:

* Alla i organisationen bör välja samma tidsramar när de skapar liknande mål som är justerade.
* Det nya målets status är alltid Utkast tills du aktiverar det genom att lägga till en aktivitet, ett projekt eller ett resultat.

I den här videon får du lära dig att:

* Navigera i avsnittet [!UICONTROL Mållista] för att lägga till ett nytt mål

>[!VIDEO](https://video.tv.adobe.com/v/335191/?quality=12&learn=on&enablevpops)

## Kopiera ett befintligt mål

Säg att det är slutet på ett kvartal och du vill återskapa ett befintligt mål för nästa period. Eller så slutförde du inte målet och behöver förlänga till nästa tidsperiod. Vilket är det bästa alternativet för att skapa det målet? Du vill kopiera och ändra ett befintligt mål.

Att kopiera ett befintligt mål är också användbart om flera teammedlemmar har liknande mål och du måste skapa ett mål för varje mål.

Här är några saker att tänka på innan du kopierar mål:

* All information från det ursprungliga målet kopieras, med undantag för målperioden.
* Du kan kopiera resultat från ett befintligt mål och de överförs till det nya målet.
* Kopierade resultat tilldelas som standard till samma ägare.
* Du kan inte kopiera förloppet för det befintliga målet till ett nytt mål.
* Du kan inte kopiera aktiviteter för ett mål när du kopierar ett mål.

### Kopiera ett mål

1. Klicka på ett målnamn för att öppna panelen **[!UICONTROL Målinformation]**.
1. Klicka på ikonen med tre punkter bredvid målnamnet och välj sedan **[!UICONTROL Kopiera]**.
1. Uppdatera någon av följande information för det kopierade målet:
   * **Målnamn** - Det här är namnet på det nya målet. Standardvärdet är&quot;Kopia av&quot; följt av namnet på det ursprungliga målet.
   * **Period** - Den tidsperiod under vilken du vill uppnå målet. Välj en tidsperiod i listrutan eller klicka på Definiera anpassade datum för att ange en anpassad tidsperiod. Standardperioden är alltid aktuellt kvartal.
   * **Ägare** - Målets ägare. Detta kan vara en användare, ett team, en grupp eller ett företag. Standardvärdet är ägaren till det ursprungliga målet.
   * **Beskrivning** - Ytterligare information om målet.

1. Markera rutan **[!UICONTROL Kopiera resultat]** om det ursprungliga målet hade lagt till resultat och du vill kopiera dem till det nya målet. Resultatet av det kopierade målet har samma ägare, namn och uppmätta värden som det ursprungliga målets resultat.

1. Klicka på **[!UICONTROL Kopiera mål]**. Det kopierade målet sparas med statusen Utkast.

   ![En bild av panelen [!UICONTROL Målinformation] i [!DNL Workfront Goals] med alternativet [!UICONTROL Kopiera]](assets/03-workfront-goals-copy-a-goal.png)

1. Klicka på ikonen med tre punkter och välj sedan **[!UICONTROL Aktivera]**, som uppdaterar målstatusen till Aktiv. Målet måste ha en associerad aktivitet eller ett associerat resultat för att&quot;aktivera&quot;.

Om du har kopierat ett mål som inte har slutförts under en tidigare tidsperiod och vill fortsätta arbeta med det under följande tidsperiod gör du följande:

1. Gå till det ursprungliga målet i **[!UICONTROL mållistan]**.
1. Lägg till en uppdatering till målet för att ange att det kopierades och att ett mer aktuellt mål skapades.
1. Stäng det ursprungliga målet om du vill behålla de framsteg som gjordes under den ursprungliga tidsperioden. Klicka på ikonen med tre punkter bredvid målnamnet och välj **[!UICONTROL Stäng]** på menyn.
1. Uppdatera värdet [!UICONTROL Inledande] för det nya resultatet så att det matchar värdet **[!UICONTROL Mål]** för det föregående resultatet, så att det nya målförloppet börjar beräkna från den punkt som uppnåddes under den föregående perioden.

## Konvertera ett resultat eller en aktivitet till ett mål

Det sista alternativet för att skapa mål i [!DNL Workfront Goals] är att konvertera resultaten och/eller aktiviteterna för ett befintligt mål till ett annat mål. Det konverterade resultatet/aktiviteten blir ett underordnat mål till det ursprungliga målet.

Du kan göra detta när ett resultat/en aktivitet är större än förväntat och det skulle vara bra att omvandla resultatet/aktiviteten till ett faktiskt mål. Tänk på detta som en metod som går nerifrån och upp när det gäller att anpassa målen.

Tänk på följande innan du konverterar ett resultat eller en aktivitet till ett mål:

* Det konverterade resultatet eller aktiviteten blir det underordnade målet för det ursprungliga målet, och de två målen justeras.
* Det nya målet blir en enda förloppsindikator för det ursprungliga målet, om det inte finns några ytterligare resultat eller aktiviteter i det ursprungliga målet. Du måste lägga till resultat och aktiviteter i det underordnade målet för att kunna spåra förloppet.
* Det går inte att ångra konverteringen av ett resultat eller en aktivitet till ett mål. När det konverterats kan det nya underordnade målet aldrig igen bli ett resultat eller en aktivitet för det överordnade målet.

I den här videon får du lära dig att:

* Lägg till en aktivitet och konvertera den till ett justerat mål

>[!VIDEO](https://video.tv.adobe.com/v/335192/?quality=12&learn=on&enablevpops)

