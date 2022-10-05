---
title: Skapa filter med datumbaserade jokertecken
description: Lär dig hur och när datumbaserade jokertecken ska användas och skapa ett filter med ett datumbaserat jokertecken i [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Skapa filter med datumbaserade jokertecken

I den här videon får du lära dig att:

* Ta reda på när datumbaserade jokertecken ska användas
* Förstå skillnaden mellan Workfront två datumbaserade jokertecken
* Lägga till ett datumbaserat jokertecken i ett filter
* Skapa ett anpassat datum med jokertecken, attribut, operatorer och modifierare
* Skapa ett anpassat datumintervall med jokertecken

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12)

## Aktivitetsfrågor

1. Hur skapar du filterregeln om du vill ha problem som har förfallodatumet i går eller idag?
1. Hur skapar du filterregeln för att hitta projekt som förföll förra veckan?
1. Följande filterregler ingår i en uppgiftsrapport som du använder regelbundet. Vilken typ av resultat får du av den här rapporten?

![En bild av skärmen för att skapa ett uppgiftsfilter med ett datumbaserat jokertecken](assets/date-wildcard-answer-1.png)

## Svar

1. Filtrera på planerat slutdatum för utleverans mellan [!UICONTROL $$TODAY-1d] och [!UICONTROL $$IDAG].
1. Filtrera på projektets planerade slutdatum mellan [!UICONTROL $$TODAYb-1w] och [!UICONTROL $$TODAYe-1w].
1. I den här rapporten hittas uppgifter som tilldelats dig och som ännu inte är färdiga (med andra ord har ett procenttal som är mindre än 100) och som är försenade eller förfaller idag. Filterregeln för det planerade slutförandedatumet för aktiviteterna anger att du ska titta på aktiviteter som har ett förfallodatum som är lika med eller före dagens datum.
