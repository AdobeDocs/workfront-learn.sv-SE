---
title: Skapa instrumentpaneler
description: Videon syftar till att hjälpa användare att effektivt skapa, anpassa och hantera kontrollpaneler i Workfront för att övervaka och dela projektrelaterade data.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
exl-id: 7adc2aeb-6618-4894-acc3-298e35175854
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Skapa instrumentpaneler

Videon innehåller följande huvudpunkter:

* **Introduktion till instrumentpaneler:** Beskriver vad en instrumentpanel är i Workfront och dess syfte som en samling relaterade rapporter. &#x200B;
* **Skapa en instrumentpanel:** Guider för hur du skapar en ny instrumentpanel genom att navigera till instrumentpanelsområdet, välja Ny instrumentpanel, namnge den och välja en layout. &#x200B;
* **Lägga till rapporter:** Visar hur du lägger till olika rapporter på kontrollpanelen, till exempel projektrapporter, aktivitetsrapporter och problemrapporter, och hur du ordnar dem i den valda layouten. &#x200B;
* **Anpassa vyer:** Visar hur du anpassar vilka kolumner som visas i instrumentpanelsvyn genom att redigera rapporten och välja vilka kolumner som ska visas. &#x200B;
* **Lägger till ytterligare element:** Beskriver hur du lägger till en anpassad kalender och en extern sida (t.ex. ett onlinedokument) i instrumentpanelen. &#x200B;
* **Spara och fästa:** Instruktioner för hur du sparar instrumentpanelen och fäster den så att den blir enkel att komma åt. &#x200B;
* **Visning och redigering:** Visar tips om hur du visar och redigerar instrumentpanelen, inklusive hur du justerar kolumnsynlighet för bättre visning. &#x200B;
* **Söka efter och dela instrumentpaneler:** Beskriver hur du hittar instrumentpaneler via huvudmenyn, lägger till dem i favoriter och delar dem med andra användare. &#x200B;
* **Skriver ut instrumentpaneler:** Beskriver processen att skriva ut en instrumentpanel. &#x200B;


>[!VIDEO](https://video.tv.adobe.com/v/335157/?quality=12&learn=on)


## Aktiviteter för att skapa kontrollpanel

### Aktivitet 1: Skapa en kontrollpanel

Skapa en [!UICONTROL kontrollpanel] med endast en rapport i den:&quot;Sökanteckningar i det här projektet&quot;. Detta är användbart om du snabbt vill hitta uppdateringar som gjorts i ett projekt, även om det finns tusentals uppdateringar att söka igenom. Detta söker efter uppdateringstrådar för att snabbt extrahera uppdateringar som uppfyller villkoren som du anger i uppmaningarna.

Skapa den här rapporten genom att skapa en kopia av rapporten&quot;Sökanteckningar&quot; som du skapade i aktiviteten&quot;Skapa en anteckningsrapport&quot; (eller använd en annan rapport om du inte gjorde den aktiviteten).

* Ta bort uppmaningen om projektnamn från kopian och byt namn på rapporten&quot;Sök anteckningar i det här projektet&quot;.
* Namnge [!UICONTROL instrumentpanelen] &quot;Sökanteckningar&quot;.
* Gå till en projektstartsida och skapa en anpassad sektion för en [!UICONTROL instrumentpanel].
* Observera, att när du söker efter anteckningar i ditt anpassade avsnitt visas endast anteckningar i det projekt som du just nu befinner dig i.

### Svar 1

1. Kör rapporten som du skapade i aktiviteten Skapa en anteckningsrapport.
1. Klicka på **[!UICONTROL Rapportera åtgärder]** och välj **[!UICONTROL Kopiera]**. [!DNL Workfront] skapar en ny rapport med namnet&quot;Anteckningssökning (kopia)&quot;.
1. Gå till **[!UICONTROL Rapportåtgärder]** och välj **[!UICONTROL Redigera]**. Klicka på **[!UICONTROL Rapportinställningar]** och ändra namnet till &quot;Sök anteckningar i det här projektet&quot;.
1. Klicka på [!UICONTROL Rapportera frågor] och ta bort uppmaningen [!UICONTROL Projekt] > [!UICONTROL Namn] från listan.

   ![En bild av skärmen för att skapa en ny instrumentpanel](assets/edit-report-prompts.png)

1. Markera rutan **[!UICONTROL Visa frågor i instrumentpanelen]**.
1. Klicka på **[!UICONTROL Klar]** och sedan på **[!UICONTROL Spara + stäng]**. Du tittar nu på skärmen [!UICONTROL Fråga] i rapporten.

   Därefter ska du använda en genväg för att skapa en ny instrumentpanel och lägga till den här rapporten i den.

1. Klicka på **[!UICONTROL Rapportera åtgärder]** och välj **[!UICONTROL Lägg till i instrumentpanelen]** > **[!UICONTROL Ny instrumentpanel]**.
1. Dra rapporten &quot;Sök anteckningar i det här projektet&quot; till panelen **[!UICONTROL Layout]** .
1. Observera att rapportens namn blir kontrollpanelens namn. Redigera namnet så att det bara är &quot;Sök anteckningar&quot;.

   ![En bild av skärmen för att skapa en ny instrumentpanel](assets/create-dashboard.png)

1. Klicka på **[!UICONTROL Spara + Stäng]**.

   Lägg nu till kontrollpanelen på en projektsida.

   ![En bild av skärmen för att skapa en ny instrumentpanel](assets/add-custom-section.png)

1. Gå till vilket projekt som helst. Klicka på ikonen **[!UICONTROL Lägg till anpassat avsnitt]** på den vänstra panelmenyn.
1. I fältet **[!UICONTROL Lägg till en instrumentpanel]** skriver du&quot;Sökanteckningar&quot; och väljer [!UICONTROL instrumentpanelen] i listan.
1. I fältet **[!UICONTROL Anpassad avsnittstitel]** skriver du &quot;Search Notes&quot;.
1. Klicka på **[!UICONTROL Lägg till nytt avsnitt]**.
1. På den vänstra panelmenyn hittar du Sök anteckningar. Klicka på punkterna till vänster om avsnittsnamnet och dra det till höger under Uppdateringar.
