---
title: Grundläggande textläge för filter
description: Lär dig mer om textläge, kamelläge och grundläggande textläge som du kan använda i rapportfilter i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-30T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 092205dbe501521ce2152019d79e3c315e197f4f
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Grundläggande textläge för filter

>[!PREREQUISITES]
>
>* [Förstå rapportelement](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=sv-SE)
>* [Förstå rapportkomponenter](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=sv-SE)
>* [Skapa ett enkelt filter](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=sv-SE)


>[!TIP]
>
>* För att få en mer ingående förståelse för textläget rekommenderar vi att du tittar på den inspelade webbinarihändelsen [Fråga experten - Introduktion till textlägesrapportering](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), som är en timme lång.
>* Om du vill veta mer om textläge rekommenderar vi att du tittar på självstudiekurserna [Avancerad rapportering](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=sv-SE) som tillsammans är fem och en halv timmars långa.
>* Klicka här för att komma åt [[!UICONTROL API-utforskaren]](https://developer.adobe.com/workfront/api-explorer/)


I den här videon får du lära dig mer om:

* Textläge
* Kamerafodral
* Vissa _kodblock för textläge_ som du kan använda i rapportfiltren

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)

## &quot;Förstå grundläggande textläge för filter&quot;-aktiviteter


### Aktivitet - Filtrera bort aktiviteter där jag har markerat &quot;Klar med min del&quot;

I följande textläge exkluderas uppgifter där en användare har markerat &quot;Klar med min del&quot;. Allt du behöver göra är att skapa ett uppgiftsfilter, lägga till eventuella filterregler, växla sedan till textläge och klistra in koden nedan efter det textläge som visas i filtret.


>[!WARNING]
>
> Den är inte avsedd att användas i kalenderfilter.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### Aktivitet - Visa alla uppgifter som väntar på mitt godkännande

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Aktivitet - Visa alla uppgifter som jag har godkänt

Skapa en aktivitetsrapport med de filter du vill ha, gå sedan till fliken Filter och klicka på Växla till textläge. Lägg till den här koden i det som redan finns:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Aktivitet - Visa alla aktiviteter som har minst en föregångare för tvärprojekt

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Aktivitet - Visa alla uppgifter som jag har tilldelat andra

Skapa en aktivitetsrapport med de filter du vill ha, gå sedan till fliken Filter och klicka på Växla till textläge. Lägg till den här koden i det som redan finns:

>[!WARNING]
> 
> Den är inte avsedd att användas i kalenderfilter.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Då visas alla uppgifter där den inloggade användaren har tilldelat minst en av de aktuella tilldelningarna. Om flera personer har tilldelat tilldelningar visas endast namnet på den första personen som tilldelade någon som&quot;Begärd av&quot; på startsidan för uppgiften.

### Aktivitet - Visa alla uppgifter som är slutförda - väntar på godkännande

```
status=CPL:A
status_Mod=in
```


### Problem - Visa alla problem som är slutförda - väntar på godkännande

```
status=CPL:A
status_Mod=in
```


### Projekt - Visa alla projekt som har slutförts - väntar på godkännande

```
status=CPL:A
status_Mod=in
```


### Obs! Visa alla kommentarer som jag är taggad i

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Parameterrapport/rapport för anpassat fält - Visa anpassade fält som inte är kopplade till ett anpassat formulär (mycket användbart vid rensning)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
