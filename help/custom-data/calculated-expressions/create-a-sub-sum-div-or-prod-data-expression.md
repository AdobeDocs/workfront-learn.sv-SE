---
title: Skapa ett datauttryck för SUB, SUM, DIV eller PROD
description: Lär dig hur du använder och skapar de grundläggande matematiska uttrycken i ett beräkningsfält i Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Skapa ett datauttryck för SUB, SUM, DIV eller PROD

I den här videon får du lära dig:

* Vad uttrycken SUB, SUM, DIV och PROD gör
* Så här skapar du ett SUB-datauttryck i ett beräkningsfält

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12)

## Ytterligare information: ROUND-uttryck

### Skapa ett ROUND-uttryck

ROUND-uttrycket tar valfritt tal och avrundar det till ett visst antal decimaler.

Oftast används ROUND-datautdraget tillsammans med ett annat datautdrag och när formatfältet lämnas som antingen Text eller Number.

Låt oss skapa ett beräkningsfält för att avgöra skillnaden mellan antalet timmar som planerats och som faktiskt loggats in i en uppgift, vilket kräver SUB-uttrycket och ser ut så här:

**SUB (Planerade timmar, Faktiska timmar)**

Och eftersom tiden spåras i minuter och det primära formatet är att visa informationen i timmar, måste uttrycket också delas med 60 och se ut så här:

**DIV (SUB (Planerade timmar, Faktiska timmar), 60)**

Om formatet ändras till Number när du skapar beräkningsfältet i det anpassade formuläret kan du ändra talformatet när du lägger till fältet i en vy.

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/round01.png)

Om fältformatet däremot lämnas som Text när du skapar ett anpassat fält kan du inte enkelt ändra formatet i vyn. ROUND-uttrycket måste användas för att undvika att siffror som detta visas i ditt projekt:

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/round02.png)

Använd ROUND-datauttrycket i ett beräkningsfält ROUND-uttrycket innehåller namnet på uttrycket (ROUND) och vanligtvis två datapunkter. Dessa datapunkter kan vara ett uttryck eller ett fält i [!DNL Workfront], följt av en siffra som anger hur många decimaler du vill gå.

Ett uttryck skulle struktureras så här: ROUND(datapunkt, #)

Använd det här uttrycket - DIV(SUB(Planerade timmar, Faktiska timmar),60) - som första datapunkt i uttrycket som beräknar skillnaden mellan planerad och faktisk tid. Kontrollera sedan att det tal som kommer från det uttrycket inte är längre än två decimaler till höger om decimaltalet.

![Arbetsbelastningsutjämnare med utnyttjanderapport](assets/round03.png)

Uttrycket kan skrivas så här: ROUND(DIV(SUB(Planerade timmar, Faktiska timmar),60),2).
