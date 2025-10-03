---
title: Anpassa utseendet på [!UICONTROL varumärkesanslutningen]
description: Lär dig hur du anpassar navigeringsfältet och sidfoten och anpassar hemsidan och inloggningssidan i [!UICONTROL Brand Connect] för [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Anpassa utseendet på [!UICONTROL varumärkesanslutningen]

I den här videon får du lära dig att:

* Anpassa navigeringsfältet och sidfoten
* Anpassa startsidan och inloggningssidan

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on&enablevpops=1)

## Ytterligare inställning för [!UICONTROL Utseende]

Alternativet [!UICONTROL Teckensnitt] under menyn [!UICONTROL Utseende] formaterar all text i hela [!UICONTROL Brand Portal] i det valda teckensnittet. Mer än 800 Google-teckensnitt stöds.

![Alternativet [!UICONTROL Teckensnitt] under menyformatet [!UICONTROL Utseende] för [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## Widgetar för hemsida

Anpassa utseendet på din [!UICONTROL Brand Connect]-hemsida så att den matchar din organisation. Med widgetar kan du lägga till element som mappar och bildreglage. Om din organisation har flera [!UICONTROL varumärkesanslutningar] har alla en egen hemsida, som du kan ge olika utseenden.

![En skärmbild av de tillgängliga widgetarna för din [!UICONTROL Brand Connect]-hemsida](assets/03-brand-connect-home-page-widgets.png)

Dessa widgetar är tillgängliga:

**A. Carousel** - Visa flera resurser i ett bildreglage. Du kan lägga till beskrivningar för varje resurs. Klicka på ikonen Lägg till för att välja bilder som ska visas i karusellen.

**B. Mapp** - Visa en mapp som innehåller markerade resurser. Klicka på ikonen Lägg till för att öppna [!UICONTROL resursväljaren] så att du kan välja en mapp. Assets i mappen är synligt för [!UICONTROL Brand Connect]-användare, men kan bara hämtas av dem som har behörighet.

**C. Ljuslåda** - Visa en befintlig [!UICONTROL Ljuslåda ] . Resurserna i [!UICONTROL ljuslådan] visas för [!UICONTROL Brand Connect] -användare, men kan bara hämtas av dem som har behörighet.

**D. Varumärkesriktlinjer** - Visa Varumärkesriktlinjerna på hemsidan i stället för/utöver i det övre navigeringsfältet.

**E. Beskrivning** - Används för att visa korta textbitar.

**F. Fylld beskrivning** - Ange ett textkopieringsblock som ska visas på en grå bakgrund.

**G. HTML** - Använd HTML och CSS för att skapa anpassat innehåll. Du kan till exempel bädda in en länk till en video. Det finns några [HTML-taggar som kan undvikas](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html).

## Lägg till ett sökfält

Om du utformar en anpassad hemsida för din organisations [!UICONTROL varumärkesanslutning] måste användarna klicka i [!UICONTROL Assets] för att kunna göra en sökning.

Men systemadministratörer kan skapa ett sökfält med hjälp av HTML-widgeten och den här HTML-taggen:

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
