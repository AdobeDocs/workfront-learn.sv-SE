---
title: Skapa ADDDAYS-, ADDWEEKDAY-, ADDMONTHS-, ADDYEARS-uttryck
description: Lär dig hur du använder och skapar ADD-uttryck i ett beräkningsfält i Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Skapa ADDDAYS-, ADDWEEKDAY-, ADDMONTHS-, ADDYEARS-uttryck

I den här videon får du lära dig:

* Hur ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-uttrycken beräknas
* Så här skapar du ett ADDWEEKDAYS-datauttryck i ett beräkningsfält

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Ytterligare exempel

Nedan finns några ytterligare ADDDAYS-/ADDWEEKDAY-/ADDMONTHS-/ADDYEAR-uttryck Adobe [!DNL Workfront] kunderna har skapat.

**Bör ha gjorts av**

Kunden ville veta när uppgiften skulle ha slutförts baserat på det faktiska startdatumet och den planerade varaktigheten. Det planerade slutförandedatumet fungerar inte i det här fallet eftersom det kan flyttas om aktiviteten är sen, och det planerade slutförandedatumet hjälper inte om det uppstår förseningar i tidigare aktiviteter.

Uttrycket som skapades var ADDDAYS (faktiskt startdatum, (Varaktighet/480))

Tid i fältet Varaktighet sparas i minuter. I det här uttrycket kan fältet Varaktighet inte vara fristående om tiden ska visas i dagar. För att detta ska ske måste varaktigheten divideras med 480 minuter (480 minuter = 8 timmar = 1 dag)

Det är därför den andra värdeplatsen innehåller (Duration/480).


**Fakturaavslutsdatum**

Det här exemplet innehåller ett annat beräkningsfält, som redan har skapats och sparats i systemet, i uttrycket.

Kunden registrerade datumet då fakturan skickades via ett anpassat datumfält med namnet&quot;Inlämningsdatum för faktura&quot; i det anpassade formuläret. Efter att ha skickats har de 30 dagar på sig att fylla i och arkivera fakturan. För att automatiskt skapa detta slutförings- och arkiveringsdatum skapade de ett beräkningsfält med hjälp av ADDDDAYS och fältet Inlämningsdatum för faktura. Uttrycket såg ut så här:

ADDDAYS (fakturadeklarationsdatum,30)
