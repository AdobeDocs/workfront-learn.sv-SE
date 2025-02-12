---
title: Skapa grundläggande filteraktiviteter
description: I den här aktiviteten skapar du ett projektfilter med namnet"Projekt jag själv stänger den här månaden".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Skapa grundläggande filteraktiviteter

## Aktivitet 1 - Alla projekt i marknadsföringsportföljen

I den här aktiviteten skapar du ett projektfilter med namnet&quot;Alla projekt i marknadsföringsportföljen&quot; i [!UICONTROL Äldre filter] -upplevelsen. Här visas alla projekt i portföljen med namnet&quot;Marketing Portfolio&quot;, oavsett status.

Stegvisa instruktioner finns nedan.

### Svar på aktivitet 1

![En bild av skärmen för att skapa ett nytt filter](assets/basic-filter-activity-1.png)

1. Navigera till området [!UICONTROL Projekt] från [!UICONTROL Huvudmenyn]. Här visas en lista med projekt.
1. Klicka på menyn **[!UICONTROL Filter]** och välj [!UICONTROL Äldre filter].
1. Välj **[!UICONTROL Nytt filter]**.
1. Ge filtret namnet&quot;Alla projekt i marknadsföringsportföljen&quot;.
1. Klicka på **[!UICONTROL Lägg till filterregel]**.
1. I fältet [!UICONTROL Börja skriva fältnamn] skriver du [!UICONTROL portföljnamn]. Välj sedan [!UICONTROL Namn] under fältkällan [!UICONTROL Portfolio].
1. Låt operatorn [!UICONTROL Lika med] vara kvar.
1. Skriv [!UICONTROL marketing] i fältet [!UICONTROL Börja skriva namn].
1. Välj [!UICONTROL Marketing Portfolio] om du har en portfölj med det namnet som du vill filtrera på. Om du inte bara använder funktionen för att skriva framför för att hitta den portfölj du vill ha.
1. Klicka på **[!UICONTROL Spara filter]**.

## Aktivitet 2 - projekt som jag äger stänger den här månaden

I den här videon skapar du ett projektfilter med namnet&quot;Projekt jag stänger den här månaden&quot; i [!UICONTROL Äldre filter] . Om du håller ett öga på många projekt kan det här filtret hjälpa dig att zooma in på de som ska stängas snart.

Stegvisa instruktioner finns nedan.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on&enablevpops)

### Svar på aktivitet 2

![En bild av skärmen för att skapa ett nytt filter](assets/basic-filter-activity-updated-6-15-21.png)

1. Navigera till området [!UICONTROL Projekt] från [!UICONTROL Huvudmenyn]. Här visas en lista med projekt.
1. Klicka på menyn **[!UICONTROL Filter]** och välj [!UICONTROL Äldre filter].
1. Välj **[!UICONTROL Nytt filter]**.
1. Ge filtret namnet&quot;Projekt jag äger stänger den här månaden&quot;.
1. Klicka på **[!UICONTROL Lägg till filterregel]**.
1. Skriv &quot;owner&quot; i fältet [!UICONTROL Börja skriva fältnamn]. Välj sedan [!UICONTROL Ägar-ID] under fältkällan [!UICONTROL Projekt].
1. Låt operatorn [!UICONTROL Lika med] vara kvar.
1. Skriv &quot;$$&quot; i fältet [!UICONTROL Börja skriva namn].
1. Välj [!UICONTROL $$USER.ID]. Detta är jokertecknet för den inloggade användaren.
1. Klicka på [!UICONTROL Lägg till filterregel] igen.
1. I fältet [!UICONTROL Börja skriva fältnamn] börjar du skriva &quot;Är klar&quot;. Välj sedan [!UICONTROL Är slutförd] under Projektfältets källa.
1. Låt operatorn [!UICONTROL Lika med] vara kvar.
1. Välj &quot;Falskt&quot;.
1. Klicka på [!UICONTROL Lägg till filterregel] igen.
1. I fältet [!UICONTROL Start typing field name] skriver du &quot;planerad&quot; och väljer sedan [!UICONTROL Planerad slutförandetid] under fältkällan [!UICONTROL Project].
1. Ändra operatorn [!UICONTROL Lika med] till [!UICONTROL Den här månaden].
1. Klicka på **[!UICONTROL Spara filter]**.
