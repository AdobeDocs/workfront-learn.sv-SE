---
title: Utvecklingsverktyget
description: Förbättra dina möjligheter att felsöka ett scenario och underlätta komplexa konfigurationer med DevTool.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11057
thumbnail: KT11057.png
exl-id: 13080212-26cf-4e5f-8f0b-fc59a6f66eb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Utvecklingsverktyget

Förbättra dina möjligheter att felsöka ett scenario och underlätta komplexa konfigurationer med utvecklingsverktyget.

## Översikt över övningar

Installera och använd de olika områdena i Workfront Dev-verktyget för att fördjupa dig i frågor/svar och avancerade scenariodesignknep.

>[!NOTE]
>
>Workfront Fusion Dev-verktyget är bara tillgängligt i webbläsaren Chrome när du använder [Kromutvecklare](https://developer.chrome.com/docs/devtools/).

![Devtool Image 1](../12-exercises/assets/devtool-walkthrough-1.png)

## Steg som ska följas

**Installera utvecklingsverktyget.**

1. Ladda ned dokumentet&quot;workfront-fusion-devtool.zip&quot; som finns i mappen Fusion Exercise Files i testenheten.
1. Extrahera zip-filerna till en mapp.
1. Öppna en flik i Chrome och ange **chrome://extensions**.
1. Växla i utvecklarläget med knappen längst upp till höger och klicka sedan på knappen &quot;Läs in ej packad&quot; som visas längst upp till vänster. Markera mappen som innehåller utvecklingsverktyget (här packade du upp den).

   ![Devtool Image 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. När du packat upp det visas utvecklingsverktyget bland dina andra tillägg.

   ![Devtool Image 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **Använd liveströmmen.**

1. Börja med att öppna scenariot&quot;Använda datalager för att synkronisera data&quot;.
1. Öppna utvecklingsverktyget genom att skriva F12 eller funktionen F12. Du kan också klicka på menyn med tre punkter i adressfältet i Chrome och navigera till Utvecklarverktyg.

   ![Devtool Image 4](../12-exercises/assets/navigate-to-devtools.png)

1. Klicka på fliken Workfront Fusion och välj sedan Live Stream i listan till vänster.
1. Klicka på Kör en gång för att se händelser allt eftersom de inträffar.
1. Klicka på en händelse för att se flikarna till höger för Request Headers, Request Body, Response Headers och Response Body.

   ![Devtool Image 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **Använda felsökningsprogrammet för scenarier**

1. Välj Felsökning för scenario och klicka på en modul för att visa information om åtgärderna i den modulen.

   ![Devtool Image 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. Navigera till fliken Historik. Klicka på Information om en körning för att undersöka modulens åtgärdsinformation för en specifik körning.

   ![Devtool Image 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **Använda verktygen**

1. Gå tillbaka till scenariodesignern och välj Verktyg i utvecklingsverktyget. Då visas tillgängliga verktyg.

   ![Devtool Image 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ Fokusera på en modul - Hitta och öppna en modul snabbt med hjälp av modul-ID:t.
+ Sök efter modul(er) efter mappning - Sök i ett scenario med hjälp av ett nyckelord för att hitta mappade värden och/eller nycklar i moduler.
+ Hämta appmetadata - Se metadata för den valda appen som ett scenario.
+ Kopiera mappning - Kopierar mappning från en modul till en annan. Du kan också klona modulen i designern.
+ Kopiera filter - Kopierar ett filter. Filtret tilldelas alltid till modulen till höger.
+ Växla anslutning - Verktyget tar anslutningen från den valda modulen och ställer in samma anslutning till alla moduler i samma program i scenariot. Detta är användbart om du måste ändra anslutningen under hela det slutförda scenariot. Förlora inte all mappning och spara tid med det här verktyget.
+ Växla variabel - Söker efter alla förekomster av den angivna variabeln i hela scenariot, eller i en modul, och ersätter dem med den nya. Jokertecken stöds inte. Om du av misstag har mappat ett värde i hela scenariot kan det hjälpa dig att enkelt växla till rätt värde.
+ Växla app - Byter ut den angivna appen mot en annan.
+ Base 64 - Koda angivna data till Base64 eller avkoda Base64. Användbart när du vill söka efter vissa data i den kodade begäran.
+ Kopiera modulnamn - Kopierar det valda modulnamnet till Urklipp.
+ Mappa om källa - Ändra mappningskälla från en modul till en annan. Du måste först lägga till modulen som ska användas som en källmodul i flödet i ett scenario.
+ Migrera operativsystem - specifikt för att uppgradera Google Sheets-moduler (äldre) till den senaste Google Sheets-versionen. En ny version av modulen läggs till precis efter den äldre versionen av modulen i scenarioflödet.
