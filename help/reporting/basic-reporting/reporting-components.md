---
title: Förstå rapporteringskomponenter
description: Workfront rapportkomponenter förbättrar datavisualiseringen med objektbaserade filter, dynamiska vyer, strukturerade grupperingar och jokerfunktioner för skräddarsydda insikter.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
last-substantial-update: 2025-04-28T00:00:00Z
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# Förstå rapporteringskomponenter

I videon förklaras begreppet att rapportera komponenter i Workfront, vilket är nödvändigt för att skapa filter, vyer och grupperingar. Nyckelkomponenterna är:

* **Objekttyp:** Anger det Workfront-objekt som behandlas, till exempel ett projekt, en aktivitet eller en timingpost. &#x200B; Filter, vyer och grupperingar är specifika för objekttypen. &#x200B;
* **Fält-Source och fältnamn:** Fältkällan är det objekt i Workfront där information bifogas och fältnamnet är den specifika informationen (t.ex. &quot;description&quot; för ett projekt). &#x200B;
* **Värdefält:** Representerar innehållet i ett fält, till exempel &quot;low&quot;, &quot;normal&quot;, &quot;high&quot; eller &quot;urgent&quot; för prioritetsfältet. &#x200B;
* **Filterkvalificerare:** Definierar vilka värden som ska inkluderas eller exkluderas i en rapport, till exempel att aktiviteter med prioriteten &quot;high&quot; &#x200B; visas.


>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&learn=on&enablevpops=0)

## Viktiga uppgifter

* **Rapporteringskomponenter:** Workfront rapportkomponenter innehåller objekttyp, fältkälla, fältnamn, filterkvalificerare och värdefält, vilket är nödvändigt för att skapa filter, vyer och grupperingar. &#x200B;
* **Objekttypsspecifikation:** Filter, vyer och grupperingar är kopplade till specifika objekttyper, till exempel projekt, uppgifter eller timposter, vilket säkerställer att rapporterna är anpassade till relevanta data. &#x200B;
* **Filterregler:** Filtren använder fältkälla, fältnamn, kvalificerare och värden för att definiera villkor. &#x200B; Filtret&quot;Mina projekt&quot; visar till exempel bara aktuella projekt där den inloggade användaren är en del av projektteamet. &#x200B;
* **Vyer och grupperingar:** Vyer visar kombinationer av fältkälla och fältnamn i kolumner (t.ex. &quot;ägarnamn&quot;), medan grupperingar organiserar data baserat på specifika villkor (t.ex. &quot;företagsnamn&quot;). &#x200B;
* **Användning med jokertecken:** Jokertecken i filter tillåter dynamisk matchning, t.ex. identifiering av inloggade användare i ett projektteam, vilket förbättrar personaliseringen vid rapportering. &#x200B;

## Snabbreferens för rapportkomponenter

![En bild av skärmen för att skapa ett filter](assets/reporting-components-1.png)

**A - Fältkälla**

Alternativen för fältkälla beror på den valda objekttypen. Fältkällan är ofta det objekt i Workfront som en viss del av informationen (kallas fältnamn) tillhör. Ibland är fältkällan densamma som objekttypen.
Fältkällan avgör vilka fältnamn som är tillgängliga.

Exempel: [!UICONTROL Projekt], [!UICONTROL Aktivitet], [!UICONTROL Problem], [!UICONTROL Tilldelad]

**B - Fältnamn**

Fältnamn är information som är tillgänglig om det du har valt som fältkälla.

De kan vara Workfront-fält som du har fyllt i, fält från ett anpassat formulär eller information som Workfront automatiskt hämtar.

Fältnamn styr värdefältalternativen.

Exempel: [!UICONTROL Förloppsstatus], [!UICONTROL Beskrivning], [!UICONTROL Planerat slutförandedatum], anpassade formulärfält

**C - Filterkvalificerare**

Filterkvalificerare minskar antalet möjliga resultat som kan visas under den valda fältkällan och det valda fältnamnet.

De anger hur fältkällan och fältnamnet relaterar till värdefältet.

Exempel: Equal, Contains, Null, Less than

**D - värde**

Värdet är den information som anges i fältet som anges av fältnamnet.

Alternativen för värden bestäms av fältkällan och fältnamnet.

Jokertecken för användare och datum kan användas både i värdet och i friformstext.

Exempel: Nytt, Aktuellt, $$TODAYbw, Beskrivning

>[!TIP]
>
>Mer information om fältnamn i Workfront finns i [ordlistan för Adobe Workfront-terminologi](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=sv-SE).

