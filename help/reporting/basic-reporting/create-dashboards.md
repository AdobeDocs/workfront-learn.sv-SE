---
title: Skapa instrumentpaneler
description: Lär dig hur du kombinerar olika typer av listrapporter, diagram, kalendrar och externa webbsidor till en kontrollpanel i Workfront.
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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 4%

---

# Skapa instrumentpaneler

I den här videon får du lära dig:

* Vad en kontrollpanel är i Workfront
* Så här skapar du en kontrollpanel
* Hitta och använda kontrollpaneler
* Dela en kontrollpanel med andra Workfront-användare
* Skriva ut en kontrollpanel

>[!VIDEO](https://video.tv.adobe.com/v/335157/?quality=12&learn=on&enablevpops)

## Aktivitet: Skapa en kontrollpanel

Skapa en [!UICONTROL kontrollpanel] med endast en rapport i den:&quot;Sökanteckningar i det här projektet&quot;. Detta är användbart om du snabbt vill hitta uppdateringar som gjorts i ett projekt, även om det finns tusentals uppdateringar att söka igenom. Detta söker efter uppdateringstrådar för att snabbt extrahera uppdateringar som uppfyller villkoren som du anger i uppmaningarna.

Skapa den här rapporten genom att skapa en kopia av rapporten&quot;Anteckningar&quot; som du skapade i aktiviteten&quot;Skapa en anteckningsrapport&quot; (eller använd en annan rapport om du inte gjorde den aktiviteten).

* Ta bort uppmaningen om projektnamn från kopian och byt namn på rapporten&quot;Sök anteckningar i det här projektet&quot;.
* Namnge [!UICONTROL instrumentpanelen] &quot;Sökanteckningar&quot;.
* Gå till en projektstartsida och skapa en anpassad sektion för en [!UICONTROL instrumentpanel].
* Observera, att när du söker efter anteckningar i ditt anpassade avsnitt visas endast anteckningar i det projekt du just nu befinner dig i.

## Svar

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
