---
title: Skapa instrumentpaneler
description: Organisera och visa projektdata med Workfront-instrumentpaneler som kan anpassas, öppnas enkelt, delas och skrivas ut för smidig projekthandledning och smidigt samarbete.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
last-substantial-update: 2025-05-28T00:00:00Z
exl-id: 7adc2aeb-6618-4894-acc3-298e35175854
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 4%

---

# Skapa instrumentpaneler

Videon innehåller en omfattande guide till hur du lär dig mer om och använder kontrollpaneler i Workfront.
&#x200B;Det förklarar att en kontrollpanel är en samling rapporter som gör att användarna kan ordna och visa relaterade data på ett och samma ställe.

>[!VIDEO](https://video.tv.adobe.com/v/335157/?quality=12&learn=on)

## Viktiga uppgifter

* **Kontrollpaneler i Workfront:** En kontrollpanel är en samling rapporter som gör att användare kan ordna och visa relaterade data, till exempel projekt, uppgifter och problem, i en central vy. &#x200B;
* **Skapa instrumentpaneler:** Du kan anpassa instrumentpaneler genom att välja en layout, lägga till rapporter, anpassade kalendrar eller externa sidor och ordna dem för optimal visning. &#x200B; Användare kan också anpassa vilka kolumner som ska visas i rapporter sida vid sida på kontrollpanelen. &#x200B;
* **Åtkomst till instrumentpaneler:** Instrumentpaneler finns under Mina instrumentpaneler, Delade instrumentpaneler eller Alla instrumentpaneler i instrumentpanelsområdet. &#x200B; Kontrollpaneler som används ofta kan fästas eller läggas till i favoriter för snabb åtkomst. &#x200B;
* **Kontrollpaneler för delning:** Instrumentpaneler kan delas med andra Workfront-användare, inklusive alla rapporter på kontrollpanelen, via menyn Instrumentpanelsåtgärder. &#x200B;
* **Kontrollpaneler för utskrift:** Kontrollpaneler kan skrivas ut direkt från menyn Instrumentpanelsåtgärder, vilket gör det enkelt att dela fysiska kopior av data. &#x200B;


## Aktiviteter för att skapa kontrollpanel

### Aktivitet 1: Skapa en kontrollpanel

Skapa en [!UICONTROL kontrollpanel] med endast en rapport i den:&quot;Sökanteckningar i det här projektet&quot;. Detta är användbart om du snabbt vill hitta uppdateringar som gjorts i ett projekt, även om det finns tusentals uppdateringar att söka igenom. Detta söker efter uppdateringstrådar för att snabbt extrahera uppdateringar som uppfyller villkoren som du anger i uppmaningarna.

Skapa den här rapporten genom att skapa en kopia av rapporten&quot;Sökanteckningar&quot; som du skapade i aktiviteten&quot;Skapa en anteckningsrapport&quot;. Har du inte skapat den än? Klicka här om du vill se aktiviteten i självstudiekursen [Skapa en aktivitetsrapport](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-task-report#activity-1-create-a-note-report-with-prompts).

* Ta bort uppmaningen om projektnamn från kopian och byt namn på rapporten&quot;Sök anteckningar i det här projektet&quot;.
* Namnge [!UICONTROL instrumentpanelen] &quot;Sökanteckningar&quot;.
* Gå till en projektstartsida och skapa en anpassad sektion för en [!UICONTROL instrumentpanel].
* Observera, att när du söker efter anteckningar i ditt anpassade avsnitt visas endast anteckningar i det projekt som du just nu befinner dig i.

### Svar 1

1. Kör rapporten som du skapade i aktiviteten Skapa en anteckningsrapport. Har du inte skapat den än? Klicka här om du vill se aktiviteten i självstudiekursen [Skapa en aktivitetsrapport](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-task-report#activity-1-create-a-note-report-with-prompts).
1. Klicka på **[!UICONTROL Rapportera åtgärder]** och välj **[!UICONTROL Kopiera]**. [!DNL Workfront] skapar en ny rapport med namnet&quot;Anteckningssökning (kopia)&quot;.
1. Gå till **[!UICONTROL Rapportåtgärder]** och välj **[!UICONTROL Redigera]**. Klicka på **[!UICONTROL Rapportinställningar]** och ändra namnet till &quot;Sök anteckningar i det här projektet&quot;.
1. Klicka på [!UICONTROL Rapportera frågor] och ta bort uppmaningen [!UICONTROL Projekt] > [!UICONTROL Namn] från listan.

   ![En bild av skärmen för att skapa en ny instrumentpanel](assets/edit-report-prompts.png)

1. Markera rutan **[!UICONTROL Visa frågor i instrumentpanelen]**.
1. Klicka på **[!UICONTROL Klar]** och sedan på **[!UICONTROL Spara + stäng]**. Du tittar nu på skärmen [!UICONTROL Fråga] i rapporten.

   Därefter ska du använda en genväg för att skapa en ny instrumentpanel och lägga till den här rapporten i den.

1. Klicka på **[!UICONTROL Rapportera åtgärder]** och välj **[!UICONTROL Lägg till i klassisk kontrollpanel]** > **[!UICONTROL Ny kontrollpanel]**.
1. Dra rapporten &quot;Sök anteckningar i det här projektet&quot; till panelen **[!UICONTROL Layout]** .
1. Observera att rapportens namn blir kontrollpanelens namn. Redigera namnet så att det bara är &quot;Sök anteckningar&quot;.

   ![En bild av skärmen för att skapa en ny instrumentpanel](assets/create-dashboard.png)

1. Klicka på **[!UICONTROL Spara + Stäng]**.

   Lägg nu till kontrollpanelen på en projektsida.

   ![En bild av skärmen för att skapa en ny instrumentpanel](assets/add-custom-section.png)

1. Gå till vilket projekt som helst. Klicka på knappen **[!UICONTROL Lägg till en instrumentpanel]** på den vänstra panelmenyn.
1. I fältet **[!UICONTROL Välj en instrumentpanel]** skriver du&quot;Sökanteckningar&quot; och väljer [!UICONTROL instrumentpanelen] i listan.
1. I fältet **[!UICONTROL Namn på snabblänk]** skriver du&quot;Sök anteckningar&quot;.
1. Klicka på **[!UICONTROL Lägg till]**.
1. På den vänstra panelmenyn hittar du Sök anteckningar längst ned. Klicka på punkterna till vänster om namnet och dra det uppåt till höger nedanför Uppdateringar.
