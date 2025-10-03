---
title: Skapa grundläggande filteraktiviteter
description: I den här aktiviteten skapar du ett projektfilter med namnet"Alla projekt i marknadsföringsportföljen" och ett annat projektfilter med namnet"Projekt jag äger som stänger den här månaden".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
last-substantial-update: 2025-05-15T00:00:00Z
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Skapa grundläggande filteraktiviteter


## Aktivitet 1 - Alla projekt i marknadsföringsportföljen

I den här aktiviteten skapar du ett projektfilter med namnet&quot;Alla projekt i marknadsföringsportföljen&quot; i [!UICONTROL Äldre filter] -upplevelsen. Här visas alla projekt i portföljen med namnet&quot;Marketing Portfolio&quot;, oavsett status.

Stegvisa instruktioner finns nedan.

## Svar på aktivitet 1

![En bild av skärmen för att skapa ett nytt filter](assets/basic-filter-activity-1.png)

1. Navigera till området [!UICONTROL Projekt] från [!UICONTROL Huvudmenyn]. Här visas en lista med projekt.
1. Klicka på menyn **[!UICONTROL Filter]** och välj [!UICONTROL Äldre filter] om det inte redan är markerat.
1. Välj **[!UICONTROL Nytt filter]**.
1. Ge filtret namnet&quot;Alla projekt i marknadsföringsportföljen&quot;.
1. Klicka på **[!UICONTROL Lägg till filterregel]**.
1. Klicka på fältet **Välj ett fält** och börja skriva &quot;[!UICONTROL portföljnamn]&quot;. Välj sedan [!UICONTROL Namn] under fältkällan [!UICONTROL Portfolio].
1. Låt operatorn [!UICONTROL Lika med] vara kvar.
1. Skriv [!UICONTROL marketing] i sökfältet.
1. Välj [!UICONTROL Marketing Portfolio] om du har en portfölj med det namnet som du vill filtrera på. Om du inte bara använder funktionen för att skriva framför för att hitta den portfölj du vill ha.
1. Klicka på **[!UICONTROL Spara filter]**.

## Aktivitet 2 - projekt som jag äger stänger den här månaden

I den här videon skapar du ett projektfilter med namnet&quot;Projekt jag stänger den här månaden&quot; i [!UICONTROL Äldre filter] . Om du håller ett öga på många projekt kan det här filtret hjälpa dig att zooma in på de som ska stängas snart.

Stegvisa instruktioner finns nedan.

>[!VIDEO](https://video.tv.adobe.com/v/3443383/?quality=12&learn=on&enablevpops=1&captions=swe)

## Svar på aktivitet 2

![En bild av skärmen för att skapa ett nytt filter](assets/basic-filter-activity-2.png)

1. Navigera till området [!UICONTROL Projekt] från [!UICONTROL Huvudmenyn]. Här visas en lista med projekt.
1. Klicka på menyn **[!UICONTROL Filter]** och välj [!UICONTROL Äldre filter] om det inte redan är markerat.
1. Välj **[!UICONTROL Nytt filter]**.
1. Ge filtret namnet&quot;Projekt jag äger stänger den här månaden&quot;.
1. Klicka på **[!UICONTROL Lägg till filterregel]**.
1. Klicka på fältet **Markera ett fält** och börja skriva ordet &quot;Ägare&quot;. Klicka nu på ägar-ID under fältkällan [!UICONTROL Projekt].
1. Låt operatorn [!UICONTROL Lika med] vara kvar.
1. Skriv $$ i sökfältet.
1. Välj [!UICONTROL $$USER.ID]. Detta är jokertecknet för den inloggade användaren.
1. Klicka på Lägg till en annan filterregel.
1. Klicka på fältet **Markera ett fält** och börja skriva ordet&quot;Är slutfört&quot;. Klicka nu på&quot;Är slutförd&quot; under fältkällan [!UICONTROL Projekt].
1. Låt operatorn [!UICONTROL Lika med] vara kvar.
1. Välj &quot;Falskt&quot;.
1. Klicka på Lägg till en annan filterregel igen.
1. Klicka på fältet **Markera ett fält** och börja skriva ordet &quot;Planerad&quot;. Klicka nu på &quot;Planerat slutförandedatum&quot; under fältkällan [!UICONTROL Projekt].
1. Ändra operatorn [!UICONTROL Lika med] till [!UICONTROL Den här månaden].
1. Klicka på **[!UICONTROL Spara filter]**.
