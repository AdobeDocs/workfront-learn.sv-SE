---
title: God praxis - filter, vyer och grupperingar
description: Utforska rekommendationer från Adobe Workfront experter om hur du konfigurerar, hanterar och använder Workfront-filter, -vyer och -grupperingar.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0c822b5be5272c5b638039d83294b00d25c32141
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# God praxis - filter, vyer och grupperingar

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa praxis är riktlinjer som utgör ett effektivt och effektivt sätt att agera, som enkelt används av dig och användarna på ditt företag och som kan återges framgångsrikt i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa tillvägagångssätt för filter, vyer och grupperingar

* Minska antalet anpassade rapporter du skapar genom att utnyttja filter, vyer och grupperingar i en objektlista för att få de data du behöver.

* Använd listkontrollerna i layoutmallar för att dölja onödiga filter, vyer och grupperingar för vanliga objekt (projekt, uppgifter, program osv.).

* Utbyt egna filter, vyer och grupperingar som är relevanta för organisationens arbetsflöden och processer med listkontrollerna för layoutmallar.

* När du skapar filter för projektstatus, aktivitetsstatus eller utgivningsstatus ska du använda (objekt)>>Status är lika med fältets käll-/fältnamn med modifieraren Lika, i stället för Project>>Statusfältets källa/fältnamn.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Minska antalet anpassade rapporter du skapar genom att utnyttja filter, vyer och grupperingar i en objektlista för att få de data du behöver.

**Här är varför**

Att skapa engångsrapporter för varje datasegment som du vill se är tidskrävande och klumpar ihop Workfront-systemet.

Instruktioner om hur du skapar rapporter med uppmaningar finns i kapitlet&quot;Hur du konfigurerar och använder rapportmeddelanden&quot; i [Förstå rapportinställningar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html).

Instruktioner om hur du skapar rapporter med anpassade uppmaningar finns i [Skapa egna uppmaningar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html).

</br>
</br>

**Bästa praxis**

Använd listkontrollerna i layoutmallar för att dölja onödiga filter, vyer och grupperingar för vanliga objekt (projekt, uppgifter, program osv.).

**Här är varför**

Mindre är mer. Alternativen för att dölja filter, visa och gruppera listor som inte är relevanta för dina användares dagliga arbetsflöden minskar listorna, vilket gör det enklare för användarna att hitta det de behöver snabbare.

Instruktioner om hur du döljer filter, vyer och grupperingar med layoutmallar finns i [Anpassa rapportlistor med layoutmallar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html).

</br>
</br>

**Bästa praxis**

Utbyt egna filter, vyer och grupperingar som är relevanta för organisationens arbetsflöden och processer med listkontrollerna för layoutmallar.

**Här är varför**

Om du har skapat filter, vyer och grupperingar som visar information som är specifik för användarnas dagliga processer är det enkelt att dela dessa via layoutmallarna. Detta garanterar att alla som är tilldelade layoutmallen har alternativ för filtrering, visning och gruppering som är relevanta för deras arbetsflöden.

Att anpassa den information som du vill visa för användarna via layoutmallarna är också tidsbesparande för system- och gruppadministratörer eftersom de inte behöver dela varje filter, vy eller grupperingsalternativ individuellt.

Instruktioner om hur du delar filter, vyer och grupperingar med layoutmallar finns i [Anpassa rapportlistor med layoutmallar](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html).

</br>
</br>

**Bästa praxis**

När du skapar filter för projektstatus, aktivitetsstatus eller utgivningsstatus ska du använda (objekt)>>Status är lika med fältets käll-/fältnamn med modifieraren Lika, i stället för Project>>Statusfältets källa/fältnamn.

**Här är varför**

Genom att använda (objekt)>>Liknar med, inkluderas alla anpassade statusvärden som har den specifika statusen tilldelad i fältet Likater med i statusinställningarna. Om du ställer in filtret som (objekt)>>Status > Likhet måste du välja specifika lägen för filtret. Detta kan utgöra en underhållsutmaning om du behöver ta hänsyn till de nya statusvärdena i olika filter. Varje filter måste öppnas och uppdateras med den nya statusen.

Om du till exempel vill se alla aktuella projekt kan du konfigurera filtret så att det läser Projekt > Status > Lika > Aktuell. Men om någon lägger till en anpassad status med namnet Aktiv och jämför den med Aktuell, kommer det filtret inte att hitta projekt med statusen Aktiv. Om du däremot använder Project>>Status Equates With > Equal > Current hittar filtret objekt med antingen aktuell eller aktiv status eftersom de båda har Current i fältet Equates With.
