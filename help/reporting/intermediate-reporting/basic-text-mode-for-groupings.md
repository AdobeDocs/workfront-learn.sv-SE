---
title: Grundläggande textläge för grupperingar
description: Lär dig mer om textläge, kamelläge och grundläggande textläge som du kan använda i rapportgrupperingar i Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Grundläggande textläge för grupperingar

>[!PREREQUISITES]
>
>* [Förstå rapportelement](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=sv-SE)
>* [Förstå rapportkomponenter](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=sv-SE)
>* [Skapa en grundläggande gruppering](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-grouping.html?lang=sv-SE)


>[!TIP]
>
>* För att få en mer ingående förståelse för textläget rekommenderar vi att du tittar på den inspelade webbinarihändelsen [Fråga experten - Introduktion till textlägesrapportering](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), som är en timme lång.
>* Om du vill veta mer om textläge rekommenderar vi att du tittar på självstudiekurserna [Avancerad rapportering](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=sv-SE) som tillsammans är fem och en halv timmars långa.
>* Klicka här för att komma åt [[!UICONTROL API-utforskaren]](https://developer.adobe.com/workfront/api-explorer/)

I den här videon får du lära dig:

* Vilket textläge är
* Vad kamelfodral är
* Vissa _textlägeskodblock_ som du kan använda i rapportgrupperingarna

>[!VIDEO](https://video.tv.adobe.com/v/3428983/?quality=12&learn=on&captions=swe)

## Förstå grundläggande textläge för grupperingar

### Aktivitet - 4 överordnade grupperingar

I följande textläge grupperas uppgifter baserat på upp till fyra nivåer med överordnade och överordnade som inte finns tomma lämnas.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![En skärmbild som visar projektaktiviteter grupperade av 4 överordnade](assets/4-parents-grouping.png)


### Aktivitet - Procent slutförd gruppering

I följande textläge grupperas uppgifter baserat på hur många procent de har slutförts. Aktiviteter hamnar i någon av följande kategorier när de grupperas:

* 0 %
* 1 till 25 %
* 26 till 50 %
* 51 till 75 %
* 76 % till 99 %
* 100 %

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![En skärmbild som visar projektaktiviteter grupperade efter procent färdigt](assets/percent-complete-grouping.png)

### Aktivitet - statusEquatesWith, sedan status

I följande textläge grupperas uppgifter efter statusEquatesWith och sedan efter status.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![En skärmbild som visar projektaktiviteter grupperade efter statusEquatesWith](assets/status-equates-with.png)


### Godkännandebevis - gruppera efter projektnamn

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![En skärmbild som visar korrekturgodkännanden grupperade efter projektnamn](assets/proof-approvals-grouped-by-project-name.png)


### Godkännandebevis - gruppera efter dokumentnamn

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![En skärmbild som visar korrekturgodkännanden grupperade efter projektnamn](assets/proof-approvals-grouped-by-doc-name.png)

