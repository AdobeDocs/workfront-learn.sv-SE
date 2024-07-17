---
title: Synlighet i resurshanteringsverktyg
description: Ta reda på vad en primär tilldelad är och hur det påverkar hanteringen av dina resurser.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10184
exl-id: 3818c7fb-b820-4002-bf49-9c79c9f0afb2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Synlighet i resurshanteringsverktyg

Att veta vem som är tillgänglig och när är avgörande för resursplanering och resurshantering. När användare avmarkerar sin personliga tid i kalendern i Workfront kan den informationen också visas i Workfront resursverktyg.

## Resursplanering

En användares lediga tid visas i kolumnen Tillgänglig (AVL) i resursplaneraren. Workfront subtraherar den tid som är markerad i kalendern från den tillgängliga tiden, enligt Workfront beräkning baserat på tilldelat schema, procentvärde för jobbroll osv.

![Tid kvar i tillgänglig kolumn](assets/vis_01.png)

## Utjämning av arbetsbelastning

I Arbetsbelastningsutjämnaren visas ledig tid som grå staplar i kalendern. Denna synlighet hjälper resursansvariga och andra att fatta mer välgrundade beslut när de tilldelar arbete.

Tidsgränsen för indikatorn förhindrar dock inte att arbete tilldelas användaren via Utjämning av arbetsbelastning. Om arbete tilldelas visar Utjämning av arbetsbelastning att personen är övertilldelad under periodens tid.

![Tid för grått fält](assets/vis_02.png)
