---
title: Skapa mål i [!DNL Workfront Goals]
description: Lär dig skapa mål i [!DNL Workfront Goals] med tre olika alternativ.
activity: use
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 10122
exl-id: 784b353f-cc6b-4a4b-9935-9e5d25c532b4
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# Skapa mål i [!DNL Workfront Goals]

I [!DNL Workfront Goals], chefer och företagsledare kan se hur hela organisationen utvecklas på varje nivå, ända ned till individen. [!DNL Workfront Goals] ger synlighet så att ni får viktiga åtgärdbara insikter för att lyfta fram de högsta prioriteringarna, identifiera riskmål, diagnostisera problem i realtid och proaktivt kurskorrigera.

[!DNL Workfront Goals] kan även enskilda medarbetare se hur deras arbete bidrar till helheten. Arbetet är mer meningsfullt när individer kan se var deras arbete är viktigt.

Det finns tre sätt att skapa mål med [!DNL Workfront]:

## Skapa ett helt nytt mål

Här är några saker att tänka på när du skapar mål från grunden:

* Du kan inte skapa mål med tidigare slutdatum.
* Alla i organisationen bör välja samma tidsramar när de skapar liknande mål som är justerade.
* Anpassade datum begränsas av det första datum du valde. Det innebär att om du väljer&quot;kvartal&quot; och ett anpassat datum, kan det anpassade datumet inte ligga efter kvarteret.
* Det nya målets status är alltid i utkastläge tills du aktiverar det genom att lägga till en aktivitet eller ett resultat.

I den här videon får du lära dig att:

* Navigera i [!UICONTROL Mållista] för att lägga till ett nytt mål

>[!VIDEO](https://video.tv.adobe.com/v/335191/?quality=12)

## Kopiera ett befintligt mål

Säg att det är slutet på ett kvartal och du vill återskapa ett befintligt mål för nästa period. Eller så slutförde du inte målet och behöver förlänga till nästa tidsperiod. Vilket är det bästa alternativet för att skapa det målet? Du vill kopiera och ändra ett befintligt mål.

Att kopiera ett befintligt mål är också användbart om flera teammedlemmar har liknande mål och du måste skapa ett mål för varje mål.

Här är några saker att tänka på innan du kopierar mål:

* All information från det ursprungliga målet kopieras, med undantag för målperioden (eftersom den redan finns).
* Du kan kopiera resultat från ett befintligt mål och de överförs till det nya målet.
* Kopierade resultat tilldelas som standard till samma ägare.
* Du kan inte kopiera förloppet för det befintliga målet till ett nytt mål.
* Du kan inte kopiera aktiviteter för ett mål när du kopierar ett mål.

### Så här kopierar du ett mål

1. Klicka på ett målnamn för att öppna **[!UICONTROL Målinformation]** -panelen.
1. Klicka på ikonen med tre punkter och välj sedan **[!UICONTROL Kopiera]**.
1. Uppdatera någon av följande information för det kopierade målet:
   * **Nytt mål**- Det här är namnet på det nya målet. Standardvärdet är namnet på det ursprungliga målet.
   * **Period**- Den tidsperiod under vilken du vill uppnå målet. Välj en tidsperiod i listrutan eller klicka på Definiera anpassade datum för att ange en anpassad tidsperiod. Standardperioden är alltid aktuellt kvartal.
   * **Ägare**- Målets ägare. Detta kan vara en användare, ett team, en grupp eller ett företag. Standardvärdet är ägaren till det ursprungliga målet.
   * **Beskrivning**—Ytterligare information om målet.

1. Kontrollera **[!UICONTROL Kopiera resultat]** om det ursprungliga målet hade lagt till resultat och du vill kopiera dem till det nya målet. Resultatet av det kopierade målet har samma ägare, namn och uppmätta värden som det ursprungliga målets resultat.

1. Klicka **[!UICONTROL Spara]**. Det kopierade målet sparas med statusen Utkast.

   ![En bild av [!UICONTROL Målinformation] panel i [!DNL Workfront Goals] med [!UICONTROL Kopiera] option](assets/03-workfront-goals-copy-a-goal.png)

1. Klicka **[!UICONTROL Aktivera]**, som uppdaterar målstatusen till Aktiv. Målet måste ha en associerad aktivitet eller ett associerat resultat för att&quot;aktivera&quot;.

1. Klicka på **X** i det övre högra hörnet av [!UICONTROL Målinformation] för att stänga den.

Om du har kopierat ett mål som inte har slutförts under en tidigare tidsperiod och vill fortsätta arbeta med det under följande tidsperiod gör du följande:

1. Gå till det ursprungliga målet i **[!UICONTROL Mållista]**, **[!UICONTROL Checka in]** eller **[!UICONTROL Puls]** -avsnitt.
1. Kommentera målet för att ange att det kopierades och att ett mer aktuellt mål skapades.
1. Stäng det ursprungliga målet om du vill behålla de framsteg som gjordes under den ursprungliga tidsperioden. Klicka på ikonen med tre punkter i dialogrutan **[!UICONTROL Målinformation]** panel och markera **[!UICONTROL Stäng]** på menyn.
1. Uppdatera [!UICONTROL Inledande] värdet för det nya resultatet så att det matchar **[!UICONTROL Mål]** värdet på föregående resultat, så ditt nya målförlopp börjar beräkna från den punkt som uppnåddes under föregående period.

## Konvertera ett resultat eller en aktivitet till ett mål

Det sista alternativet för att skapa mål i [!DNL Workfront Goals] är genom att konvertera resultaten och/eller aktiviteterna för ett befintligt mål till ett annat mål. Det konverterade resultatet/aktiviteten blir ett underordnat mål till det ursprungliga målet.

Du kan göra detta när ett resultat/en aktivitet är större än förväntat och det skulle vara bra att omvandla resultatet/aktiviteten till ett faktiskt mål. Tänk på detta som en metod som går nerifrån och upp när det gäller att anpassa målen.

Tänk på följande innan du konverterar ett resultat eller en aktivitet till ett mål:

* Det konverterade resultatet eller aktiviteten kan bli det underordnade målet för det ursprungliga målet. De två målen blir anpassade.
* Det konverterade resultatet eller den konverterade aktiviteten kan tas bort från det ursprungliga målet och läggas till som ett resultat eller en aktivitet i det nya målet.
* Det nya målet blir en enda förloppsindikator för det ursprungliga målet, om det inte finns några ytterligare resultat eller aktiviteter i det ursprungliga målet.

I den här videon får du lära dig att:

* Konvertera en aktivitet till ett justerat mål

>[!VIDEO](https://video.tv.adobe.com/v/335192/?quality=12)

Nu när du har utforskat de tre sätten att skapa mål i [!DNL Workfront Goals], vi arbetar med att aktivera de målen.
