---
title: Förstå det grundläggande textläget för vyer
description: Lär dig vilket textläge som är, vilket kameraläge som är och ett grundläggande textläge för att"spela upp" som du kan använda i dina vyer i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Förstå det grundläggande textläget för vyer


>[!IMPORTANT]
>
>Förutsättningar:
>
>* Förstå rapportelement
>* Förstå rapporteringskomponenter
>* Skapa en grundvy


>[!TIP]
>
>* Vi rekommenderar att du tittar på det inspelade webbinariet för att få en bättre förståelse för textläget [Fråga experten - Introduktion till rapportering i textläge](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), som är en timme lång.
>* Vi rekommenderar att du tittar på [Avancerad rapportering](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) självstudiekurser, som tillsammans är fem och en halv timme långa.


I den här videon får du lära dig:

* Vilket textläge är
* Vad kamelväska är
* Vissa grundläggande textlägen för plug and play som du kan använda i dina vyer

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## Aktivitet - 4 överordnade vyer

Skapa först en kolumn för Uppgiftsnamn och Överordnat namn och använd sedan följande textläge för att skapa de andra tre kolumnerna.

### Aktivitet - överordnad för överordnat namn

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### Aktivitet - överordnad för överordnat namn

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### Aktivitet - överordnad för överordnad för överordnat namn

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![En skärmbild som visar vyn 4 för överordnade](assets/4-parents-view.png)

## Användare - Iterationer som visar listor i användarvyer

### Användare - alla jobbroller

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Användare - Alla jobbroller visar primär

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Användare - alla team

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>Det finns ett Team-fält som är tillgängligt via gränssnittet och som visar alla team, kommaseparerade, men med textläget ovan visas varje team på en separat rad.


### Användare - alla grupper

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Användare - Alla grupper som visar hemgrupp

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Användare - direkta rapporter

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Användare - framtida PTO

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![En skärmbild som visar vyn Användarlistor](assets/user-lists-view-large.png)

## Aktivitet - Så här visar du aktivitetstilldelningar och arbetar med status

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![En skärmbild som visar uppdrags- och statusvyn](assets/assignments-and-status-view.png)


## Aktivitet - Så här visar du roll och allokering för flera aktivitetstilldelningar

### Aktivitet - roll + timmar

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Aktivitet - Tilldelning + procentuell allokering

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![En skärmbild som visar vyn Uppdrag och roller](assets/assignments-roles-and-percent-view.png)

## Aktivitet - Föregående och efterföljande projekt för flera projekt

### Aktivitetsfilter (valfritt)

**Visa alla aktiviteter som har minst en föregångare för korsprojekt**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Aktivitet - Visa föregående namn och föregående projekt finns i

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### Aktivitet - Visa efterträdarnamn och efterföljare för projekt finns i

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### Aktivitet - Visa planerat slutförandedatum för föregående aktiviteter

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### Aktivitet - Visa förloppsstatus för föregående aktiviteter

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### Aktivitet - Visa procent färdigt av föregående projekt

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![En skärmbild som visar vyn för föregående och efterföljande tvärprojekt](assets/cross-project-predecessors-and-successors.png)


## Aktivitet - Iteration som visar alla personer som har tilldelats och som har tilldelat var och en av dem

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![En skärmbild som visar alla personer som har tilldelats och som har tilldelat var och en av dem](assets/all-assignees-and-requesters.png)

## Aktivitet/projekt - Iteration som visar alla anpassade formulär i ett projekt eller en uppgift

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![En skärmbild som visar alla anpassade formulär i ett projekt](assets/all-custom-forms-on-a-project.png)


## Projekt - Iteration som visar alla primära kontakter för lösta objekt i projektvyn

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![En skärmbild som visar primära kontakter för upplösningar](assets/primary-contacts-for-resolvables.png)

## Projekt - iteration som visar alla projektgruppsmedlemmar

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![En skärmbild som visar alla medlemmar i projektteamet](assets/all-project-team-members.png)

## Projekt - iteration som visar postDatum för alla lösta problem för ett projekt

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![En skärmbild som visar entryDate för alla lösta problem i ett projekt](assets/resolvables-entry-date.png)

## Projekt - Visa hemgruppen för den ursprungliga projektbegäraren

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![En skärmbild som visar hemgruppen för projektbegäraren](assets/requestor-home-group.png)

## Projekt - Visa om projektet är en begärandekö

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![En skärmbild som visar om projektet är en begärandekö](assets/project-is-a-request-queue.png)

## Problem - Upprepning som visar alla medlemmar i projektteamet som kan matchas

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![En skärmbild som visar alla medlemmar i projektteamet som kan matchas](assets/all-resolve-project-team-members.png)

## Problem - Upprepning som visar alla team för problemets primära kontakt

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![En skärmbild som visar alla primära kontaktteam](assets/all-primary-contact-teams.png)

## Dokument - iteration som visar mapp i en dokumentrapport

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![En skärmbild som visar en mapp i en dokumentrapport](assets/folder-in-a-document-report.png)

## Dokument - iteration som visar den överordnade mappen i en dokumentrapport

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![En skärmbild som visar den överordnade mappen i en dokumentrapport](assets/parent-folder-in-a-document-report.png)

## Dokument - datum för dokumentgodkännande

```
displayname=Document Approval Dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![En skärmbild som visar vyn Godkännandedatum för dokument](assets/document-approval-dates.png)

## Godkännanden

### Korrektur för godkännande - Visa projektnamn

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Korrektur för godkännande - Visa aktivitetsnamn

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![En skärmbild som visar projektet och uppgiften med ett korrekturgodkännande](assets/proof-approval-project-and-task.png)
