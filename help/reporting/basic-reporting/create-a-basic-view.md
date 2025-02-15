---
title: Skapa en grundvy
description: Lär dig vad en vy är, hur du skapar en vy och hur du delar en vy med andra användare i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2023-06-20T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: 6afb57b983b094f9bc0c082a160453ecb394ca8e
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Skapa en grundvy

I den här videon får du lära dig:

* Vilken vy har Workfront?
* Så här skapar och ändrar du en vy
* Dela en vy med andra Workfront-användare

>[!VIDEO](https://video.tv.adobe.com/v/335148/?quality=12&learn=on)

## Skapa grundläggande vyaktiviteter

[Klicka här](/help/assets/create-basic-view-activities.pdf) om du vill hämta en PDF av den här sidan.

### Aktivitet 1: Skapa en aktivitetsstatusvy

Som projektledare, gruppledare eller resurshanterare vill du hålla reda på hur arbetet fortskrider. I den här vyn visas flera statusindikatorer för en aktivitet på en rad i listan eller rapporten.

Skapa en uppgiftsvy med namnet &quot;Aktivitetsstatusvy&quot; med följande kolumner:

* [!UICONTROL Aktivitetsnamn]
* [!UICONTROL Uppdrag]
* [!UICONTROL Varaktighet]
* [!UICONTROL Procent färdigt]
* [!UICONTROL Status]
* [!UICONTROL Förloppsstatus]
* [!UICONTROL Statusikoner]

### Svar 1

![En bild av skärmen för att skapa en aktivitetsstatusvy](assets/view-exercise.png)

1. I en uppgiftslistrapport går du till listrutan **[!UICONTROL Visa]** och väljer **[!UICONTROL Ny vy]**.
1. Ge vyn namnet&quot;Aktivitetsstatusvy&quot;.
1. Ta bort de här kolumnerna: [!UICONTROL Planera timmar], [!UICONTROL Föregående], [!UICONTROL Starta den] och [!UICONTROL Förfaller den].
1. Klicka på **[!UICONTROL Lägg till kolumn]**.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du&quot;status&quot; och väljer sedan&quot;Status&quot; under fältkällan [!UICONTROL Aktivitet].
1. Klicka på **[!UICONTROL Lägg till kolumn]** igen.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du &quot;status&quot; och väljer sedan &quot;Status&quot; under fältkällan [!UICONTROL Aktivitet].
1. Klicka på **[!UICONTROL Lägg till kolumn]** igen.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du &quot;status&quot; och väljer sedan &quot;Status Icons&quot; under aktivitetsfältets källa.
1. Klicka på **[!UICONTROL Spara]**.

Håll pekaren över ikonerna i kolumnen [!UICONTROL Statusikoner] för att se vad de representerar. Om de är nedtonade innebär det att uppgiften inte har några anteckningar, dokument, godkännandeprocesser osv. Om en ikon visas i färg är minst ett av objekten kopplat till uppgiften. Du kan klicka på antecknings- eller dokumentikonerna för att gå till det objektet.

### Aktivitet 2: Skapa en milstolpe-vy

Om du använder milstolpar är den här vyn det enklaste sättet att se milstolpar efter namn och lägga till eller redigera dem med hjälp av redigering i rad.

Skapa en uppgiftsvy med namnet&quot;Milstolpevy&quot; med följande kolumner:

* [!UICONTROL Aktivitetsnamn]
* [!UICONTROL Uppdrag]
* [!UICONTROL Varaktighet]
* [!UICONTROL Planera timmar]
* [!UICONTROL Milstolpe: Namn]
* [!UICONTROL Starta den]
* [!UICONTROL Förfaller den]
* [!UICONTROL Procent färdigt]


### Svar 2

![En bild av skärmen för att skapa en milstolpevy](assets/view-milestone-exercise-1.png)

1. Gå till listrutan **[!UICONTROL Visa]** i en projektuppgiftslista och välj **[!UICONTROL Ny vy]**.
1. Ge din vy namnet&quot;Milstolpevy&quot;.
1. Klicka på kolumnen [!UICONTROL Föregående] för att markera den.
1. I fältet [!UICONTROL Visa i den här kolumnen] klickar du på X-ikonen i fältet [!UICONTROL Aktivitet >> Föregående], skriver [!UICONTROL milstolpe-namn] och klickar på [!UICONTROL Namn] i listan.
1. Klicka på **[!UICONTROL Spara]**.

![En bild av en uppgiftslista med hjälp av en milstolpevy](assets/view-milestone-exercise-2.png)

### Aktivitet 3: Skapa en vy för varaktighetstyper och uppgiftsbegränsningar

I den här vyn kan du granska och redigera alla varaktighetstyper och aktivitetsbegränsningar i ditt projekt.

Skapa en uppgiftsvy med namnet&quot;Varaktighetstyper och vyn över uppgiftsbegränsningar&quot; med följande kolumner:

* [!UICONTROL Aktivitetsnamn]
* [!UICONTROL Uppdrag]
* [!UICONTROL Varaktighet]
* [!UICONTROL Planerad varaktighet]
* [!UICONTROL Planera timmar]
* [!UICONTROL Föregående]
* [!UICONTROL Starta den]
* [!UICONTROL Förfaller den]
* [!UICONTROL Varaktighetstyp]
* [!UICONTROL Aktivitetsbegränsning]
* [!UICONTROL Begränsningsdatum]

Ändra [!UICONTROL fältformatet ] i kolumnerna [!UICONTROL Starta den] och [!UICONTROL Förfaller den ] så att både datum och tid visas.

### Svar 3

![En bild av skärmen som visar varaktighetstyperna och vyn för aktivitetsbegränsningar](assets/view-activity-3.png)

1. Gå till listrutan **[!UICONTROL Visa]** i en projektuppgiftslista och välj **[!UICONTROL Ny vy]**.
1. Ge din vy namnet&quot;Varaktighetstyper och vyn Begränsade uppgifter&quot;.
1. Ta bort kolumnen [!UICONTROL  % färdigt].
1. Klicka på **[!UICONTROL Lägg till kolumn]**.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du [!UICONTROL &quot;duration&quot;] och väljer sedan [!UICONTROL &quot;Planerad varaktighet&quot;] under fältkällan [!UICONTROL Aktivitet].
1. Flytta den här kolumnen mellan kolumnerna [!UICONTROL Varaktighet] och [!UICONTROL Planera timmar].
1. Klicka på **[!UICONTROL Lägg till kolumn]** igen.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du [!UICONTROL &quot;varaktighetstyp&quot;] och väljer sedan [!UICONTROL &quot;Varaktighetstyp&quot;] under fältkällan [!UICONTROL Aktivitet].
1. Klicka på **[!UICONTROL Lägg till kolumn]** igen.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du [!UICONTROL &quot;begränsning&quot;] och väljer sedan [!UICONTROL &quot;Aktivitetsbegränsning&quot;] under aktivitetsfältets källa.
1. Klicka på **[!UICONTROL Lägg till kolumn]** igen.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du [!UICONTROL &quot;begränsning&quot;] och väljer sedan [!UICONTROL &quot;Begränsningsdatum&quot;] under aktivitetsfältets källa.
1. Markera kolumnen [!UICONTROL Starta den] och klicka sedan på [!UICONTROL Avancerade alternativ].
1. Under listrutan [!UICONTROL Fältformat] väljer du [!UICONTROL &quot;10/17/60 3:00 AM&quot;].
1. Markera kolumnen [!UICONTROL Förfaller den] och klicka sedan på [!UICONTROL Avancerade alternativ].
1. Under listrutan [!UICONTROL Fältformat] väljer du [!UICONTROL &quot;10/17/60 3:00 AM&quot;].
1. Klicka på **[!UICONTROL Spara]**.

### Aktivitet 4: Skapa en aktiv statusvy för projektmall

Alla som hanterar projektmallar kommer att uppskatta om de kan se den aktiva statusen (Sant eller Falskt) för varje mall i en lista. Ännu bättre - fältet kan redigeras direkt!

Skapa en projektmallsvy med namnet&quot;Standard+active status&quot; med följande kolumner:

* [!UICONTROL Namn]
* [!UICONTROL Ägare]
* [!UICONTROL Varaktighet]
* [!UICONTROL Planerade timmar]
* [!UICONTROL Planerad kostnad]
* [!UICONTROL Flaggor]
* [!UICONTROL Gruppnamn]
* [!UICONTROL Är aktiv]


### Svar 4

![En bild av skärmen som visar en aktiv statusvy för en projektmall](assets/view-activity-4.png)

1. Gå till listrutan **[!UICONTROL Visa]** i en projektmallslista och välj **[!UICONTROL Ny vy]**.
1. Ge vyn namnet&quot;Standard+active status&quot;.
1. Klicka på **[!UICONTROL Lägg till kolumn]**.
1. I fältet [!UICONTROL Visa i den här kolumnen] skriver du&quot;is&quot; och väljer&quot;Is Active&quot; under fältkällan [!UICONTROL Template].
1. Klicka på **[!UICONTROL Spara vy]**.
