---
title: Kopiera ett befintligt mål
description: Lär dig hur du kopierar ett befintligt mål i [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Kopiera ett befintligt mål

Säg att det är slutet på ett kvartal och du vill återskapa ett befintligt mål för nästa period. Eller så slutförde du inte målet och behöver förlänga till nästa tidsperiod. Vilket är det bästa alternativet för att skapa det målet? Du vill kopiera och ändra ett befintligt mål.

Att kopiera ett befintligt mål är också användbart om flera teammedlemmar har liknande mål och du måste skapa ett mål för varje mål.

<!--
Pro-tips graphic
-->

Här är några saker att tänka på innan du kopierar mål:

* All information från det ursprungliga målet kopieras, med undantag för målperioden (eftersom den redan finns).
* Du kan kopiera resultat från ett befintligt mål och de överförs till det nya målet.
* Kopierade resultat tilldelas som standard till samma ägare.
* Du kan inte kopiera förloppet för det befintliga målet till ett nytt mål.
* Du kan inte kopiera aktiviteter för ett mål när du kopierar ett mål.

## Så här kopierar du ett mål

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
