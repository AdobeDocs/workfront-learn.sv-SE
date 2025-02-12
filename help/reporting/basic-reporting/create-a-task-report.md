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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# Skapa en uppgiftsrapport

I den här videon får du lära dig:

* Skapa en uppgiftsrapport med ett komplext filter
* Hitta de rapporter du skapar

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on&enablevpops)



>[!TIP]
>
>Dela upp dina spatulor och mixa skålar och gör dig redo att prova recepten i vår [Adobe Workfront Customer Reporting Cookbook](/help/assets/workfront-customer-reporting-cookbook.pdf). Inuti finns stegvisa instruktioner för 10 rapporter, klara att användas i din miljö idag.
>Vi har samlat in rapporter från kunderna och sammanställt dem i en lättsmält kokbok som du kan ta tillbaka och testa i ditt eget Workfront-kök.
>Dessa 10 rapporter kommer från kunder som är precis som du. Vi är skyldiga ett stort tack till de fantastiska kunder som delade en av sina favoritrapporter, som sprids ut över olika branscher, avdelningar, team, befattningar och alla i olika företag. Vissa rapporter är enkla (men mycket användbara), och vissa är mer komplexa för att ta dina rapporter till nästa nivå.



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

1. Välj **[!UICONTROL Rapporter]** på **[!UICONTROL Huvudmenyn]**.
1. Klicka på menyn **[!UICONTROL Ny rapport]** och välj **[!UICONTROL Obs!]**.
1. I **[!UICONTROL Kolumner (Visa)]** ställer du in dina kolumner så att de omfattar:

   ![En bild av skärmen för att skapa anteckningsrapportkolumner](assets/note-report-columns.png)

   * [!UICONTROL Obs!] > [!UICONTROL Anteckningstext]
   * [!UICONTROL Obs!] > [!UICONTROL Granska text]
   * [!UICONTROL Obs!] > [!UICONTROL Anmälningsdatum]
   * [!UICONTROL Ägare] > [!UICONTROL Namn]
   * [!UICONTROL Obs!] > [!UICONTROL Granskningstyp]
   * [!UICONTROL Aktivitet] > [!UICONTROL Namn]
   * [!UICONTROL Problem] > [!UICONTROL Namn]

1. Markera kolumnen **[!UICONTROL Postdatum]** och ändra **[!UICONTROL Sortera till fallande]**.
1. På fliken **[!UICONTROL Grupperingar]** anger du att rapporten ska grupperas efter [!UICONTROL Projekt] > [!UICONTROL Namn].

   ![En bild av skärmen för att skapa rapportgrupperingar för anteckningar](assets/note-report-groupings.png)

1. Lämna [!UICONTROL Filter] tomt.
1. Öppna **[!UICONTROL Rapportinställningar]** och ge rapporten namnet&quot;Anteckningssökning&quot;.
1. I fältet [!UICONTROL Beskrivning] skriver du något som: Sök efter system- eller användaranteckningar baserat på granskningstypen och andra uppmaningar. Systemanteckningar visas i kolumnen Granskningstext och Användaranteckningar visas i kolumnen Anteckningstext.&quot;

   ![En bild av skärmen för att skapa inställningar för anteckningsrapport](assets/note-report-report-options.png)

1. Välj fliken **[!UICONTROL Information]** så att den visas när rapporten läses in.
1. Ange att rapporten ska visa 200 objekt när rapporten inkluderas på en kontrollpanel.
1. Klicka på **[!UICONTROL Rapportera frågor]** och lägg till:

   ![En bild av skärmen där uppmaningar om anteckningsrapport skapas](assets/note-report-report-prompts.png)

   * [!UICONTROL Obs!] > [!UICONTROL Granska text]
   * [!UICONTROL Obs!] > [!UICONTROL Anteckningstext]
   * [!UICONTROL Ägare] > [!UICONTROL Namn]
   * [!UICONTROL Obs!] > [!UICONTROL Anmälningsdatum]
   * [!UICONTROL Projekt] > [!UICONTROL Namn]
   * [!UICONTROL Obs!] > [!UICONTROL Granskningstyp]

1. Markera kryssrutan för **[!UICONTROL Visa frågor i instrumentpaneler]**.
1. Spara och stäng rapporten.

## Aktivitet 2: Skapa en feedback från administratörsteamet

Det här är en problemrapport som visar alla problem i en kön för feedback-begäranden som har skapats för systemadministratörer. Du kan se hur du skapar den här begärandekön i självstudiekursen [Skapa en kö för systemadministratörsfeedback](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-system-admin-feedback-request-queue.html).

I den här rapporten används även ett anpassat formulär. Om du vill lära dig hur du skapar ett anpassat formulär kan du läsa självstudiekursen [Skapa och dela ett anpassat formulär](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html).

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

Skapa en problemrapport med namnet **Administratörsteamets feedback-rapport**.

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


![En skärmbild på feedbackrapporten från Admin team](assets/create-a-system-admin-feedback-request-queue.png)



## Aktivitet 2 svar

1. Välj **[!UICONTROL Rapporter]** på **[!UICONTROL Huvudmenyn]**.
1. Klicka på menyn **[!UICONTROL Ny rapport]** och välj **[!UICONTROL Problem]**.
1. I **[!UICONTROL Kolumner (Visa)]** ställer du in dina kolumner så att de omfattar:

   ![En bild av skärmen för att skapa kolumner för problemrapport](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problem] > [!UICONTROL Namn]
   * [!UICONTROL Primär kontakt] > [!UICONTROL Namn]
      * Obs! Detta visas med &quot;Owner:Name&quot; som kolumnetikett. Du kan ändra detta till&quot;Rapporterad av&quot; genom att klicka på Avancerade alternativ och skriva&quot;Rapporterad av&quot; i fältet **Etikett för anpassad kolumn**.
   * [!UICONTROL Problem] > [!UICONTROL Processtyp]
   * [!UICONTROL Problem] > [!UICONTROL Processnamn]
   * [!UICONTROL Problem] > [!UICONTROL Processgrad]
   * [!UICONTROL Problem] > [!UICONTROL Problem eller goda nyheter]
   * [!UICONTROL Utgåva] > [!UICONTROL Införseldatum]
   * [!UICONTROL Problem] > [!UICONTROL Ålder]
   * [!UICONTROL Problem] > [!UICONTROL Uppdrag]
   * [!UICONTROL Problem] > [!UICONTROL Status]

1. Markera kolumnen **[!UICONTROL Postdatum]** och ändra **[!UICONTROL Sortera till fallande]**.
1. På fliken **[!UICONTROL Grupperingar]** ställer du in rapporten på att gruppera efter **[!UICONTROL Problem] > [!UICONTROL Processtyp]**.

   ![En bild av skärmen för att skapa grupper med problemrapporter](assets/task-report-activity-2-2.png)

1. På fliken **[!UICONTROL Filter]** lägger du till ett filter för **[!UICONTROL Utgåva] > [!UICONTROL Projekt-ID]** som är lika med begärandeköprojektet där feedbackproblemen finns.

   ![En bild av skärmen för att skapa filter för problemrapport](assets/task-report-activity-2-3.png)

1. Spara och stäng rapporten.
