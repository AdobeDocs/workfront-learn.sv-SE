---
title: Skapa ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-uttryck
description: Lär dig hur du använder och skapar ADD-uttryck i ett beräkningsfält i Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Skapa ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS-uttryck

I den här videon får du lära dig:

* Hur ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-uttrycken beräknas
* Så här skapar du ett ADDWEEKDAYS-datauttryck i ett beräkningsfält

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops)

## Ytterligare exempel

Nedan finns några ytterligare ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR-uttryck som Adobe Workfront-kunder har skapat.

**borde ha gjorts av**

Kunden ville veta när uppgiften skulle ha slutförts baserat på det faktiska startdatumet och den planerade varaktigheten. Det planerade slutförandedatumet fungerar inte i det här fallet eftersom det kan flyttas om aktiviteten är sen, och det planerade slutförandedatumet hjälper inte om det uppstår förseningar i tidigare aktiviteter.

Det skapade uttrycket var ADDDAYS({actualStartDate},{durationMinutes}/480)

Tid i fältet Varaktighet sparas i minuter. I det här uttrycket kan fältet Varaktighet inte vara fristående om tiden ska visas i dagar. För att detta ska ske måste varaktigheten divideras med 480 minuter (480 minuter = 8 timmar = 1 dag)

Det är därför den andra värdeplatsen innehåller (Duration/480).


**Fakturaavslutsdatum**

I det här exemplet används inte bara ADDDAYS-uttrycket utan även ett anpassat fält som skapats och sparats i det anpassade formuläret.

Kunden registrerar datumet då en faktura skickas via ett anpassat datumfält med namnet&quot;Inlämningsdatum för faktura&quot;.

När fakturan har skickats måste den fyllas i och arkiveras inom 30 dagar. För att automatiskt skapa detta slutförings- och arkiveringsdatum används ett ADDDAYS-beräkningsfält tillsammans med det anpassade fältet &quot;Inlämningsdatum för faktura&quot;. Uttrycket ser ut så här:

ADDDAYS({DE:Inlämningsdatum för faktura},30)
