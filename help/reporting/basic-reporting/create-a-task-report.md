---
title: Skapa en uppgiftsrapport
description: Lär dig hur du skapar en uppgiftsrapport med ett komplext filter och hittar de rapporter du skapar i Workfront. Aktivitet – skapa en anteckningsrapport med uppmaningar.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: 2134c921e39a549808bb11235b32e25903f77df4
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 3%

---

# Skapa en uppgiftsrapport

I den här videon får du lära dig:

* Skapa en uppgiftsrapport med ett komplext filter
* Hitta de rapporter du skapar

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Aktivitet 1: Skapa en anteckningsrapport med uppmaningar

Skapa en anteckningsrapport som du kan använda för att söka efter användaranteckningar (d.v.s. kommentarer eller uppdateringar) eller systemanteckningar baserat på anteckningsinnehållet, författaren, anmälningsdatumet, projektnamnet eller granskningstypen. Ge rapporten namnet&quot;Anteckningssökning&quot;.

När du använder kommandotolken Anteckningstext söker den här rapporten i uppdateringstrådar för att snabbt extrahera alla som uppfyller villkoren som anges i uppmaningarna. När du kör rapporten behöver du inte fylla i varenda dialogruta, bara de som du bryr dig om. De tomma ignoreras automatiskt.

Vyn ska innehålla kolumner för:

* Anteckningstext
* Granskningstext
* Anmälningsdatum
* Ägare: Namn
* Granskningstyp
* Aktivitetsnamn
* Ärendenamn

Lämna filterfliken tom.

Gruppera efter projektnamn.

Ta med uppmaningar om följande:

* Granskningstext
* Anteckningstext
* Ägarnamn
* Anmälningsdatum
* Projektnamn
* Granskningstyp

## Aktivitet 1 svar

1. Välj **[!UICONTROL Rapporter]** från **[!UICONTROL Huvudmeny]**.
1. Klicka på **[!UICONTROL Ny rapport]** meny och välj **[!UICONTROL Anteckning]**.
1. I **[!UICONTROL Kolumner (vy)]** konfigurera kolumnerna så att de omfattar:

   ![En bild av skärmen för att skapa anteckningsrapportkolumner](assets/note-report-columns.png)

   * [!UICONTROL Anteckning] > [!UICONTROL Anteckningstext]
   * [!UICONTROL Anteckning] > [!UICONTROL Granskningstext]
   * [!UICONTROL Anteckning] > [!UICONTROL Anmälningsdatum]
   * [!UICONTROL Ägare] > [!UICONTROL Namn]
   * [!UICONTROL Anteckning] > [!UICONTROL Granskningstyp]
   * [!UICONTROL Uppgift] > [!UICONTROL Namn]
   * [!UICONTROL Problem] > [!UICONTROL Namn]

1. Välj **[!UICONTROL Anmälningsdatum]** kolumn och ändra **[!UICONTROL Sortera till fallande]**.
1. I **[!UICONTROL Grupperingar]** ställer du in rapporten på att gruppera efter [!UICONTROL Projekt] > [!UICONTROL Namn].

   ![En bild av skärmen för att skapa rapportgrupperingar för anteckningar](assets/note-report-groupings.png)

1. Lämna [!UICONTROL Filter] tom.
1. Öppna **[!UICONTROL Rapportinställningar]** och ge rapporten namnet&quot;Anteckningssökning&quot;.
1. I [!UICONTROL Beskrivning] -fält, skriv något som &quot;Sök efter system- eller användaranteckningar baserat på vald granskningstyp och andra uppmaningar. Systemanteckningar visas i kolumnen Granskningstext och Användaranteckningar visas i kolumnen Anteckningstext.&quot;

   ![En bild av skärmen för att skapa inställningar för anteckningsrapporter](assets/note-report-report-options.png)

1. Välj **[!UICONTROL Fliken Detaljer]** så att den visas när rapporten läses in.
1. Ange att rapporten ska visa 200 objekt när rapporten inkluderas på en kontrollpanel.
1. Klicka **[!UICONTROL Rapportera uppmaningar]** och lägg till:

   ![En bild av skärmen för att skapa anteckningsrapportmeddelanden](assets/note-report-report-prompts.png)

   * [!UICONTROL Anteckning] > [!UICONTROL Granskningstext]
   * [!UICONTROL Anteckning] > [!UICONTROL Anteckningstext]
   * [!UICONTROL Ägare] > [!UICONTROL Namn]
   * [!UICONTROL Anteckning] > [!UICONTROL Anmälningsdatum]
   * [!UICONTROL Projekt] > [!UICONTROL Namn]
   * [!UICONTROL Anteckning] > [!UICONTROL Granskningstyp]

1. Markera kryssrutan för **[!UICONTROL Visa frågor i instrumentpaneler]**.
1. Spara och stäng rapporten.

## Aktivitet 2: Skapa en feedback från administratörsteamet

Det här är en problemrapport som visar alla problem i en kön för feedback-begäranden som har skapats för systemadministratörer. Du kan se hur du skapar den här begärandekön i **Skapa en kö för feedback från systemadministratörer** självstudie.

I den här rapporten används även ett anpassat formulär. Mer information om hur du skapar ett anpassat formulär finns i [Skapa och dela ett anpassat formulär](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html) självstudie.

Det anpassade formuläret ska skapas på följande sätt:

Namn: Administratörsprocessfeedback

1. Processtyp (nedrullningsbart fält)
   * åtkomstnivåer
   * godkännandeprocess (endast globalt)
   * e-postmeddelanden
   * layoutmall
   * milstolpbana
   * projektmall
   * påminnelsemeddelanden
   * begärandekö
1. Processnamn (textfält med en rad)
1. Processklass (listrutefält)
   * 1 - helt värdelös
   * 2 - inte särskilt användbar
   * 3 - bra men kunde vara bättre
   * 4 - utmärkt
1. Problem eller goda nyheter (textfält för stycke)

Skapa en problemrapport med namnet **Återrapportering från administratörsteamet**.

Vyn ska ha följande kolumner:

* Problem: Namn
* Primär kontakt: Namn
* Problem: Processtyp
* Problem: Processnamn
* Problem: Processkvalitet
* Problem: Problem eller goda nyheter
* Utgåva: Anmälningsdatum
* Problem: Ålder
* Problem: Uppdrag
* Problem: Status

Grupp på processtyp.

Filtrera på ID:t för begärandeköprojektet där feedbackproblemen finns.


![En skärmbild med feedback från administratörsteamet](assets/create-a-system-admin-feedback-request-queue.png)



## Aktivitet 2 svar

1. Välj **[!UICONTROL Rapporter]** från **[!UICONTROL Huvudmeny]**.
1. Klicka på **[!UICONTROL Ny rapport]** meny och välj **[!UICONTROL Problem]**.
1. I **[!UICONTROL Kolumner (vy)]** konfigurera kolumnerna så att de omfattar:

   ![En bild av skärmen för att skapa kolumner för problemrapporter](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problem] > [!UICONTROL Namn]
   * [!UICONTROL Primär kontakt] > [!UICONTROL Namn] Obs! Detta visas med &quot;Owner:Name&quot; som kolumnetikett. Du kan ändra detta till&quot;Rapporterad av&quot; genom att klicka på Avancerade alternativ och skriva&quot;Rapporterad av&quot; i dialogrutan **Etikett för anpassad kolumn** fält.
   * [!UICONTROL Problem] > [!UICONTROL Processtyp]
   * [!UICONTROL Problem] > [!UICONTROL Processnamn]
   * [!UICONTROL Problem] > [!UICONTROL Processkvalitet]
   * [!UICONTROL Problem] > [!UICONTROL Problem eller goda nyheter]
   * [!UICONTROL Problem] > [!UICONTROL Anmälningsdatum]
   * [!UICONTROL Problem] > [!UICONTROL Ålder]
   * [!UICONTROL Problem] > [!UICONTROL Uppdrag]
   * [!UICONTROL Problem] > [!UICONTROL Status]

1. Välj **[!UICONTROL Anmälningsdatum]** kolumn och ändra **[!UICONTROL Sortera till fallande]**.
1. I **[!UICONTROL Grupperingar]** ställer du in rapporten på att gruppera efter **[!UICONTROL Problem] > [!UICONTROL Processtyp]**.

   ![En bild av skärmen för att skapa grupper med problemrapporter](assets/task-report-activity-2-2.png)

1. I **[!UICONTROL Filter]** lägga till ett filter för **[!UICONTROL Problem] > [!UICONTROL Projekt-ID]** för att motsvara det begärandeköprojekt där feedbackproblemen finns.

   ![En bild av skärmen för att skapa filter för problemrapporter](assets/task-report-activity-2-3.png)

1. Spara och stäng rapporten.
