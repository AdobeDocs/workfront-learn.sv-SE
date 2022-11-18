---
title: Ange/hämta variabler
description: Lär dig hur du använder modulerna Ange och Hämta variabel för att använda fälten som finns i en sökväg i en annan sökväg.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11045
thumbnail: KT11045.png
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Ange/hämta variabler

Lär dig hur du använder modulerna Ange och Hämta variabel för att använda fälten som finns i en sökväg i en annan sökväg.

## Översikt över övningar

Hitta information om ett projekt i Workfront och skicka ett e-postmeddelande med relaterad information.

![Ange Hämta variabler, bild 1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Steg som ska följas

1. Skapa ett nytt scenario och ge det namnet&quot;Dela variabler mellan routningssökvägar&quot;.
1. För utlösaren väljer du modulen Sök i Workfront-appen.

   + Ange Posttyp till Projekt.
   + Välj Alla matchande poster i resultatuppsättningen.
   + För sökvillkor ställer du in det på Status lika med CUR.
   + För Utdata väljer du ID, Namn, Beskrivning och Sponsorn-ID.

   ![Ange Hämta variabler, bild 2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Ange variabler för bild 3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Klicka på OK och byt namn på den här modulen till&quot;Sök efter aktuella projekt&quot;.
1. Lägg till en annan modul och välj Workfront Läs en post-modulen.

   + Välj Användare som posttyp.
   + Välj Namn för Utdata.
   + Mappa sponsor-ID från sökmodulen till ID-fältet.

1. Klicka på OK.
1. Byt namn på modulen&quot;Hitta sponsernamn&quot;.

   ![Ange Get variables Image 4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Spara scenariot och klicka på Kör en gång.

   Om du får ett fel i modulen Läs en post beror det troligen på att sökmodulen har hittat ett projekt utan någon sponsor.

   **Du kan undvika det här felet genom att skapa två sökvägar: en för projekt som har ett sponsor-ID och en för projekt som inte gör det.**

1. Lägg till en router mellan de två modulerna genom att klicka på skiftnyckelsikonen mellan routern och modulen Läs en post. Ställ in ett filter med namnet&quot;Sponsorn finns&quot; och ställ in villkoret till Sponsorns ID finns.

   ![Ange Get variables Image 5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Klicka på routern för att skapa en annan sökväg. Lägg till en Skicka ett e-postmodul från e-postappen.

   + Placera din egen e-postadress i fältet Till.
   + Skriv&quot;Aktuell projektinformation&quot; i fältet Ämne.
   + Ange projektnamnet, beskrivningen och sponsorn i fältet Innehåll.
   + Du kan inte hämta sponsorns namnutdata från modulen Läs en post. Du kan bara få åtkomst till ditt sponsor-ID från sökmodulen före routern. Du måste hitta ett sätt att komma åt sponsorns namn från den andra routerns sökväg.

   ![Ange Get variables Image 6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Klicka på OK för tillfället och byt namn på modulen&quot;Skicka projektinformation&quot;

   **Använd Ange/Hämta variabler för att dela data mellan olika sökvägar.**

1. Efter Sök efter sponsorns namnmodul lägger du till modulen Ange variabelverktyg.

   + Ange&quot;Sponsornamn&quot; som variabelnamn.
   + Låt livstiden för variabeln vara en cykel.
   + Mappa fältet till namnutdata från modulen Sök sponsornamn.

1. Klicka på OK och byt sedan namn på modulen&quot;Ange sponsernamn&quot;.

   ![Ange Get variables Image 7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. Högerklicka sedan mellan routern och modulen Skicka ett e-postmeddelande för att lägga till en Get-variabelverktygsmodul. Ange&quot;Sponsornamn&quot; i fältet Variabelnamn.
1. Klicka på OK. Byt namn på modulen &quot;Hämta sponsernamn&quot;.

   ![Ange Get variables Image 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Gå tillbaka till modulen Skicka ett e-postmeddelande och mappa värdet från modulen Hämta sponsernamn till innehållsfältet. Klicka på OK.

   ![Ange Get variables Image 8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Innan du testar scenariot rekommenderar vi att du begränsar antalet projekt som du bearbetar för att undvika en översvämning av e-postmeddelanden.

1. Gå till testkörningen i Workfront och leta upp projektet Northstar Fashion Exhibitors Booth. Detta är ett aktuellt projekt som har en sponsor. Kopiera projekt-ID från URL:en.

   ![Ange Hämta variabler Bild 10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. I ditt scenario klickar du på modulen Sök aktuella projekt. Lägg till ytterligare ett villkor i sökvillkoren genom att klicka på den gröna knappen &quot;Lägg till OCH regel&quot;. Ange att ID:t måste vara samma som det projekt-ID du kopierade. Klicka på OK.
1. Spara ditt scenario och klicka på Kör en gång.
1. Granska körningskontrollerna och det e-postmeddelande du får.

   ![Ange Hämta variabler Bild 11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
