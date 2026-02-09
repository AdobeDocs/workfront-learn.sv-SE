---
title: Skapa EXISTS-filter för komplexa rapporter
description: Lär dig vad ett EXISTS-filter är, vad det kan göra för dig och hur du kan skapa ett från grunden. Dessutom finns det många användbara exempel på EXISTS-filter.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Skapa EXISTS-filter för komplexa rapporter

EXISTS-filter är avancerade textlägesfilter, som gör att vi kan kringgå 2 tabell-/fälthoppsbegränsning i en standardrapportbyggare. De kan också användas för att identifiera objekt i systemet som saknar ett visst relationsvillkor via NOTEXISTS.

I den här videon får du lära dig hur du skapar ett EXISTS-filter för att se&quot;Korrekturgodkännanden för aktuella projekt&quot; i en rapport om korrekturgodkännanden.

En mer ingående genomgång av hur funktionen EXISTS fungerar finns i [Skapa komplexa textlägesfilter med hjälp av EXISTS-programsatser](https://experienceleague.adobe.com/sv/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements) .

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops=1)

## EXISTS-filterexempel

### Projektrapport finns

Detta använder aktiviteten som det länkade objektet genom att jämföra det projekt-ID som finns på aktivitetsnivån och matcha det med ID-fältet på projektnivå. Detta gör att vi sedan kan jämföra tilldelningsanvändarna för aktiviteten med jokertecknet $$USER.ID. Detta resulterar endast i projekt där användaren som visar är tilldelad en
uppgift, oavsett om de är den primära tilldelaren eller inte.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


Detta använder utgåvan (optask) som det länkade objektet, genom att även jämföra projekt-ID:t som finns på utgåvnivå (optask) och matcha det med ID-fältet på projektnivå. Detta kontrollerar sedan om något av problemen (optasks) har ett anmälningsdatum inom det angivna intervallet. I det här fallet returneras alla projekt som
inte har haft ett problem (optask) som loggats in under de senaste 30 dagarna på grund av NOTEXISTS.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### Mallrapport finns

Det här filtret visar alla mallar som inte har använts för att skapa ett projekt eller som har kopplats till ett projekt det senaste året. En sak är att för att ta reda på om en mall användes som en bifogad fil eller inte, så är den beroende av att mallen innehåller uppgifter.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### Aktivitetsrapport finns

Det här använder användartabellen som det länkade objektet, som ansluts av tilldelningens aktivitets-ID och aktivitets-ID. Detta kontrollerar sedan teamsamlingen med ID:n till användarens Team ID:n och returnerar uppgiften om någon av de tilldelade finns i samma team som den som tittar.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### Användarrapport finns

Detta returnerar alla användare som inte har publicerat en uppdatering de senaste tre veckorna. Anteckningsobjektet används för att överbrygga mellanrummet och jämför ownerID:t med ett användar-ID. Returnerar sedan användaren om inga anteckningar som ägs av användaren har ett anmälningsdatum som är större än 3 veckor sedan.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Detta returnerar alla användare som inte har loggat timmar den senaste veckan. Detta använder en metod som är mycket lik den i exemplet ovan, men i stället används timägarinformationen och timanmälningsdatumet för att basera på vilka användare som returneras.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

Visa en lista med användare som matchar ett projekts flik Personer i en användarrapport.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### Kategorirapport (anpassat formulär) finns

Den här texten innehåller en lista över alla projektformulär som aldrig har använts i ett projekt. Detta bör användas tillsammans med att ange objekttypen för det formulär som vi fokuserar på. I det här fallet är fokus PROJ, så vi bör inkludera bildtexterna i objTypes-raderna. Detta kan användas
för andra objekttyper genom att ändra objektkodrelaterade delar. Detta kontrollerar samlingen av projekt som bifogats formulär, till de listade formulären och returnerar om det inte finns någon matchning.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### Parameterrapport (anpassat fält) finns

Detta returnerar alla anpassade fält som inte är kopplade till ett anpassat formulär i systemet.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### Rapport finns

Då returneras alla rapporter med ett specifikt värde i filtren.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

Då returneras alla rapporter som är bifogade till en kontrollpanel.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### Godkännanderapport finns

Detta returnerar endast korrekturgodkännanden för projekt med statusen Aktuell. Detta använder Document-objektet för att överbrygga gapet från korrekturgodkännande till projekt genom att kontrollera currentVersionID till documentVersionID, därifrån går vi till projektstatus.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
