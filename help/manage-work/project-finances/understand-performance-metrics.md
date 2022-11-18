---
title: Förstå prestandamått
description: Lär dig använda prestandamätningar - [!UICONTROL Resultatindexmetod] ([!UICONTROL PIM]) och [!UICONTROL Uppskattning vid slutförande] ([!UICONTROL EAC]).
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Förstå prestandamått

Två prestandamått som används av projektledare är [!UICONTROL Resultatindexmetod] ([!UICONTROL PIM]) och [!UICONTROL Uppskattning vid slutförande] ([!UICONTROL EAC]). Standardvärden för hela systemet kan anges i [!DNL Workfront] och tillämpas på nya projekt. [!UICONTROL PIM] kan sedan ändras i enskilda projekt.

**[!UICONTROL PIM]**

Inställningarna för [!UICONTROL PIM] styra hur [!DNL Workfront] beräknar andra projektresultatvärden, som [!UICONTROL Kostnadsprestandaindex] ([!UICONTROL CPI]), [!UICONTROL Resultatindex för kostnadsschema] ([!UICONTROL CSI]), [!UICONTROL Schemalägg prestandaindex] ([!UICONTROL SPI]), och [!UICONTROL Uppskattning vid slutförande] ([!UICONTROL EAC]).

Alternativ för [!UICONTROL PIM] är timbaserade och kostnadsbaserade.

* **Timbaserad** — Workfront använder de planerade timmarna för att beräkna projektets CPI och EAC. Projektets EAC visas i antal timmar.
* **Kostnadsbaserad** — Workfront använder den planerade arbetskostnaden vid beräkning av projektets CPI och EAC. EAC visas som ett valutavärde. När du använder det här alternativet måste du se till att uppgiftstilldelningar (användare och/eller jobbroller) är kopplade till kostnadstariffer.

**[!UICONTROL EAC]**

[!UICONTROL EAC] representerar den beräknade totala kostnaden för uppgiften eller projektet när den är slutförd. Alternativen beräknas på projektnivå och summeras från aktiviteter/underaktiviteter.

* **Beräkna på projektnivå** — [!UICONTROL EAC] för huvuduppgiften och huvudprojektet fastställs med hjälp av de faktiska timmarna/de faktiska arbetskostnaderna i [!UICONTROL EAC] formler. Beräkningen inkluderar faktiska timmar/kostnader och utgifter som lagts till direkt i den överordnade uppgiften eller projektet.
* R **hämta från uppgifter/underaktiviteter** — [!UICONTROL EAC] för den överordnade uppgiften och projektet bestäms genom att lägga till [!UICONTROL EAC] för varje underordnad uppgift. Den här beräkningen exkluderar faktiska timmar/kostnader som lagts till direkt i en överordnad uppgift eller ett överordnat projekt.

The [!UICONTROL EAC] i tabellen&quot;Beräkna uppskattning vid slutförande&quot; <!-- link to article -->artikel om [!UICONTROL [!DNL Workfront] Ett].

**Prestandamätningar: Inställningar**

Till [!UICONTROL PIM] och [!UICONTROL EAC] standardinställningar:

1. Välj **[!UICONTROL Inställningar]** på huvudmenyn.
1. Klicka **[!UICONTROL Projektinställningar]** på den vänstra panelmenyn och sedan klicka **[!UICONTROL Projekt]**
1. I [!UICONTROL Projektstatus] avsnitt, hitta [!UICONTROL Resultatindexmetod]. Välj Timbaserad eller Kostnadsbaserad.
1. För [!UICONTROL Uppskattning vid slutförande]väljer du Beräkna på projektnivå eller Samla in uppgifter/underaktiviteter.
1. Klicka **[!UICONTROL Spara]** längst ned i fönstret.

![En bild av [!UICONTROL Projektinställningar] screen](assets/setting-up-finances-1.png)

**Ange [!UICONTROL PIM] om enskilda projekt**

1. Gå till startsidan för ett projekt.
1. Klicka **[!UICONTROL Projektinformation]** från den vänstra panelen.
1. Öppna **[!UICONTROL Ekonomi]** -avsnitt.
1. Dubbelklicka på texten nedan **[!UICONTROL Resultatindexmetod]** för att redigera den.
1. Välj Timbaserad eller Kostnadsbaserad.
1. Klicka **[!UICONTROL Spara]** Ändringar som ska slutföras.

![En bild av [!UICONTROL Projektinformation] screen](assets/setting-up-finances-2.png)

[!UICONTROL PIM] kan ställas in på en projektmall i [!UICONTROL Ekonomi] i mallinformationen.
