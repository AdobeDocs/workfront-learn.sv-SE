---
title: Genomgång av routrar
description: Lär dig hur du använder en router för att skicka Pokemon kontra superhjältar i paket längs rätt sökväg i  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Genomgång av routrar

Använd en router för att skicka Pokemon kontra superhjältar i paket längs rätt bana och skapa sedan en uppgift för varje tecken.

![En bild av Fusion-scenariot](assets/universal-connectors-and-routing-2.png)

## Genomgång av routrar

Workfront rekommenderar att du tittar på genomgången av videon innan du försöker återskapa övningen i din egen miljö.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12&learn=on&enablevpops=1)

## URL för övning

* Superhero-API-webbplats: `https://www.superheroapi.com/`
* Första URL för övning: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Andra URL för övning: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Om du har problem med att få tillgång till din egen superhjälte-token kan du använda den här delade token: 10110256647253588. Tänk på hur många gånger du anropar superhjälte-API:t så att denna delade token fortsätter att fungera för alla.



## Söka efter objekt på mappningspanelen

Med fältet Sök efter objekt högst upp på mappningspanelerna kan du snabbt hitta fält på panelen, även om de är kapslade i arrayer. Sökningen är skiftlägesokänslig.

![En bild av den första sökpanelen](assets/universal-connectors-and-routing-3.png)

![En bild av den andra sökpanelen](assets/universal-connectors-and-routing-4.png)

## Tips och tricks för att arbeta med API:er

Fram tills nu har du arbetat med ett mycket enkelt API (Application Programming Interface) som inte kräver någon extra autentisering för att hämta information som behövs i scenariot. Här är några tips som hjälper dig att navigera med API:er och universella anslutningar.

## Steg 1: Bestäm typ av API

Workfront och många programvarusystem byggs med en REST-API (Representational State Transfer), som är den enklaste och mest vanliga typen av API idag. Det finns dock några andra, till exempel:

* SOAP (Simple Object Access Protocol) (Workfront Proof API är SOAP-baserat)
* FTP (File Transfer Protocol)
* SFTP (Secure File Transfer Protocol)
* Om du vill veta mer gör du en webbsökning efter API-typer och nyckelord av intresse.

>[!NOTE]
>
>När du ansluter till större plattformar som Salesforce kommer olika delar av dessa plattformar att innehålla olika API:er. Kontrollera att du hittar rätt för den tjänst du vill ansluta till.

## Steg 2: Bestäm vilken typ av autentisering som krävs av API:t

API-autentisering är en form av identifiering som används för att styra åtkomsten till en tjänst, till exempel när du försöker ansluta via Workfront Fusion. Det hjälper dig att bevisa för ett annat system att du har behörighet att komma åt systemet. OAuth 2 är den vanligaste typen av autentisering som används idag. Läs mer i en Internetsökning om API-autentisering.

Autentisering kan vara den svåraste aspekten av att arbeta med ett API. En av de värdefullaste funktionerna i Workfront Fusions universella anslutningar är att Workfront Fusion kan hantera autentisering åt dig med vanliga autentiseringsmetoder som grundläggande autentisering, som OAuth 2, API Key med flera. När du har skapat en anslutning med rätt Workfront Fusion-modul för din autentiseringsmetod (t.ex. OAuth 2) genererar Workfront Fusion kontinuerligt API-nycklar och/eller tokens varje gång du vill köra ditt scenario.

Läs mer om de olika typer av autentisering som Workfront tillhandahåller i artikeln Översikt över utökad autentisering på Experience League.

## Steg 3: Läs API-dokumentationen och hitta de slutpunkter som behövs

När ett API interagerar med ett annat system betraktas kontaktytorna i det här meddelandet som slutpunkter. En slutpunkt är den plats där API:er skickar begäranden och där resursen finns.

När du interagerar med ett API med en universell anslutning måste du förstå vilka slutpunkter API:t stöder och vilka data som krävs för varje begäran. API-dokumentationen bör beskriva en API:s slutpunkter och hur du utför vanliga åtgärder som att skapa, läsa, uppdatera eller ta bort. För att kunna utföra dessa anrop krävs viss övning, särskilt om du inte har gjort några API-anrop eller om du har arbetat med ett nytt API.

Läs mer om Workfront Fusion Universal Connectors och hur du konfigurerar dem för att ansluta till de API:er du behöver på Experience League.

## Slutkommentar

Du kan kontrollera hela listan med våra färdiga appanslutningar i Experience League. Om du vill föreslå en ny appanslutning till Workfront Fusion-produktteamet skickar du din idé till Innovation Lab. Om du inte har lämnat in någon ansökan tidigare, lär dig mer om Innovation Lab, plus hur du kan rösta på idéer och delta i den årliga prioriteringen av Ledarpanelen. Om du redan har tillgång till innovationslabb loggar du in och skickar in dina idéer.

## Din tur

>[!NOTE]
>
>Praktiska övningar och utmaningar är frivilliga och behövs inte för att slutföra Fusion-utbildningen.

Denna övning bygger på vad du lärde dig under genomgången, men lösningen tillhandahålls inte.

Skapa variabeln&quot;Stat (nivå)&quot; i modulen Ange flera variabler för Pokemon-tecken. Mappa namnet på Pokemonstatistik till den här variabeln. Använd funktionen för arrayvärden för att ändra hur arrayen visas, så att varje station blir en ny rad enligt nedan.

**Tips!** Det finns bara sex olika Pokemon-statistik med motsvarande nivå.

![En bild av statistik](assets/universal-connectors-and-routing-5.png)

**Utmaning:** Se om du kan använda matrisformler för att få funktioner att visa på samma sätt som ovan som olika rader i stället för en sträng med värden avgränsade med kommatecken. Skärmbilden nedan ger ett tips.

![En bild av ett arraynamn](assets/universal-connectors-and-routing-6.png)

## Vill du veta mer? Vi rekommenderar följande:

[Workfront Fusion-dokumentation](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
