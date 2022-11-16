---
title: Skapa en uppgiftsrapport
description: Lär dig hur du skapar en uppgiftsrapport med ett komplext filter och hittar de rapporter du skapar i Workfront. Aktivitet - skapa en anteckningsrapport med uppmaningar.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
kt: 8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Skapa en uppgiftsrapport

I den här videon får du lära dig:

* Skapa en uppgiftsrapport med ett komplext filter
* Hitta de rapporter du skapar

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12)

## Aktivitet: Skapa en anteckningsrapport med uppmaningar

Skapa en anteckningsrapport som du kan använda för att söka efter användaranteckningar (d.v.s. kommentarer eller uppdateringar) eller systemanteckningar baserat på anteckningsinnehållet, författaren, anmälningsdatumet, projektnamnet eller granskningstypen. Ge rapporten namnet&quot;Anteckningssökning&quot;.

När du använder textrutan Anteckning söker den här rapporten i uppdateringstrådar för att snabbt extrahera alla som uppfyller villkoren som anges i uppmaningarna. När du kör rapporten behöver du inte fylla i alla uppmaningar, bara de du bryr dig om. De tomma ignoreras automatiskt.

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

## Svar

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
1. I [!UICONTROL Beskrivning] -fält, skriv &quot;Sök efter system- eller användaranteckningar baserat på vald granskningstyp och andra uppmaningar. Systemanteckningar visas i kolumnen Granskningstext och Användaranteckningar visas i kolumnen Anteckningstext.&quot;

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
