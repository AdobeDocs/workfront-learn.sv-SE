---
title: Skapa ett datauttryck för SUB, SUM, DIV eller PROD
description: Lär dig hur du använder och skapar de grundläggande matematiska uttrycken i ett beräkningsfält i Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Skapa ett datauttryck för SUB, SUM, DIV eller PROD

I den här videon får du lära dig:

* Vad uttrycken SUB, SUM, DIV och PROD gör
* Så här skapar du ett SUB-datauttryck i ett beräkningsfält

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on)

## Ytterligare information: ROUND-uttryck

### Skapa ett ROUND-uttryck

ROUND-uttrycket tar valfritt tal och avrundar det till ett visst antal decimaler.

Oftast används ROUND-datautdraget tillsammans med ett annat datautdrag och när formatfältet lämnas som antingen Text eller Number.

Låt oss skapa ett beräkningsfält för att avgöra skillnaden mellan antalet timmar som planerats och som faktiskt loggats in i en aktivitet, vilket kräver SUB-uttrycket och ser ut så här:

**SUB({workRequired},{actualWorkRequired})**

Och eftersom tiden spåras i minuter och det primära formatet är att visa informationen i timmar, måste uttrycket också delas med 60 och se ut så här:

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

Om formatet ändras till Number när du skapar beräkningsfältet i det anpassade formuläret kan du ändra talformatet när du lägger till fältet i en vy.

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/round01.png)

Men om fältformatet lämnas som Text när du skapar ett anpassat fält kan du inte enkelt ändra formatet i vyn. ROUND-uttrycket måste användas för att undvika att siffror som detta visas i ditt projekt:

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/round02.png)

<b>Använda ROUND-dataututtrycket i ett beräkningsfält</b>

ROUND-uttrycket innehåller namnet på uttrycket (ROUND) och vanligtvis två datapunkter. Dessa datapunkter kan vara ett uttryck eller ett fält i Workfront, följt av ett tal som anger hur många decimaler du vill gå.

Ett uttryck skulle struktureras så här: ROUND(datapunkt, #)

Använd det här uttrycket för att beräkna skillnaden mellan planerade och faktiska timmar —DIV(SUB({workRequired},{actualWorkRequired}),60) - som första datapunkt. Kontrollera sedan att det tal som kommer från det uttrycket inte är mer än två decimaler till höger om decimaltalet.

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/round03.png)

Uttrycket kan skrivas så här: ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2).
