---
title: Förstå det grundläggande textläget för vyer
description: Lär dig mer om textläge, kamelläge och grundläggande textläge som du kan använda i rapportvyer i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Förstå det grundläggande textläget för vyer


>[!PREREQUISITES]
>
>* [Förstå rapportelement](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=en)
>* [Förstå rapportkomponenter](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=en)
>* [Skapa en grundvy](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-view.html?lang=en)


>[!TIP]
>
>* För att få en mer ingående förståelse för textläget rekommenderar vi att du tittar på den inspelade webbinarihändelsen [Fråga experten - Introduktion till textlägesrapportering](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), som är en timme lång.
>* Om du vill veta mer om textläge rekommenderar vi att du tittar på självstudiekurserna [Avancerad rapportering](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) som tillsammans är fem och en halv timmars långa.
>* Klicka här för att komma åt [[!UICONTROL API-utforskaren]](https://developer.adobe.com/workfront/api-explorer/)

I den här videon får du lära dig:

* Vilket textläge är
* Vad kamelfodral är
* Vissa _kodblock för textläge_ som du kan använda i dina rapportvyer

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12&learn=on)

## Förstå grundläggande textläge för vyer

### Aktivitet - 4 överordnade vyer

Skapa först en kolumn för Uppgiftsnamn och Överordnat namn och använd sedan följande textläge för att skapa de andra tre kolumnerna.

#### Aktivitet - överordnad för överordnat namn

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

#### Aktivitet - överordnad för överordnat namn

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

#### Aktivitet - överordnad för överordnad för överordnat namn

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

![En skärmbild som visar vyn 4 överordnade](assets/4-parents-view.png)

### Användare - Iterationer som visar listor i användarvyer

#### Användare - alla jobbroller

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

#### Användare - Alla jobbroller visar primär

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

#### Användare - alla team

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


#### Användare - alla grupper

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

#### Användare - Alla grupper som visar hemgrupp

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


#### Användare - direkta rapporter

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

#### Användare - framtida PTO

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

### Aktivitet - Så här visar du aktivitetstilldelningar och arbetar med status

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


### Aktivitet - Så här visar du roll och allokering för flera aktivitetstilldelningar

#### Aktivitet - roll + timmar

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

#### Aktivitet - Tilldelning + procentuell allokering

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

### Aktivitet - Föregångare och efterföljare mellan projekt

#### Aktivitetsfilter (valfritt)

**Visa alla aktiviteter som har minst en föregångare mellan projekt eller minst en efterföljande tvärprojekt i aktuella projekt**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
project:statusEquatesWith=CUR
project:statusEquatesWith_Mod=in
OR:1:project:statusEquatesWith=CUR
OR:1:project:statusEquatesWith_Mod=in
OR:1:successorsMM:ID_Mod=notblank
OR:1:successorsMM:projectID=FIELD:projectID
OR:1:successorsMM:projectID_Mod=ne
```

#### Aktivitet - Visa föregående namn och föregående projekt finns i

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

#### Aktivitet - Visa efterträdarnamn och efterföljare för projekt finns i

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

#### Aktivitet - Visa planerat slutförandedatum för föregående aktiviteter

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

#### Aktivitet - Visa förloppsstatus för föregående aktiviteter

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

#### Aktivitet - Visa procent färdigt av föregående projekt

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

![En skärmbild som visar vyn för föregående och efterföljande aktiviteter mellan projekt](assets/cross-project-predecessors-and-successors.png)


### Aktivitet - Iteration som visar alla personer som har tilldelats och som har tilldelat var och en av dem

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![En skärmbild som visar alla personer som tilldelats och som tilldelat var och en av dem](assets/all-assignees-and-requesters.png)

### Aktivitet/projekt - Iteration som visar alla anpassade formulär i ett projekt eller en uppgift

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


### Projekt - Iteration som visar alla primära kontakter för lösta objekt i projektvyn

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

### Projekt - iteration som visar alla projektgruppsmedlemmar

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

![En skärmbild som visar alla projektgruppsmedlemmar](assets/all-project-team-members.png)

### Projekt - iteration som visar postDatum för alla lösta problem för ett projekt

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

### Projekt - Visa hemgruppen för den ursprungliga projektbegäraren

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

### Projekt - Visa om projektet är en begärandekö

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

### Problem - Upprepning som visar alla medlemmar i projektgruppen som kan matchas

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

![En skärmbild som visar alla medlemmar i projektgruppen ](assets/all-resolve-project-team-members.png)

### Problem - Upprepning som visar alla team för problemets primära kontakt

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

### Dokument - iteration som visar mapp i en dokumentrapport

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![En skärmbild som visar mappen i en dokumentrapport](assets/folder-in-a-document-report.png)

### Dokument - iteration som visar den överordnade mappen i en dokumentrapport

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

### Dokument - datum för dokumentgodkännande

```
displayname=Document approval dates
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

![En skärmbild som visar datumvyn för dokumentgodkännande](assets/document-approval-dates.png)

### Bevis på godkännande

#### Korrektur för godkännande - Visa projektnamn

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

#### Korrektur för godkännande - Visa aktivitetsnamn

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![En skärmbild som visar projektet och aktiviteten för ett korrekturgodkännande](assets/proof-approval-project-and-task.png)
