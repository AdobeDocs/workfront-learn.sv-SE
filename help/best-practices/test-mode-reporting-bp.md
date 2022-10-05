---
title: God praxis - rapportering i textläge
description: Utforska rekommendationer från Adobe Workfront experter om hur man ställer in, hanterar och använder Workfront textlägesrapportering.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# God praxis - rapportering i textläge

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## Bästa praxis för rapportering av textläge

* Använd uttryck för textlägesvärden i stället för beräknade anpassade fält när det är möjligt i kolumnerna i listrapporter.

* Använd beräkningar i en textlägesberäkning i rapportens beskrivning.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Använd uttryck för textlägesvärden i stället för beräknade anpassade fält när det är möjligt i kolumnerna i listrapporter.



**Här är varför**

Värdeuttryck för textläge beräknas när rapporten körs och beräknas om när rapporten uppdateras. Det innebär att ni alltid har aktuella data och korrekta rapporter.



Beräknade anpassade fält (används i anpassade formulär) uppdateras inte automatiskt när data visas i Workfront. I stället visas resultatet av den senaste beräkningen som lagrats i Workfront. Detta innebär att dessa värden kan vara&quot;inaktuella&quot; eller inaktuella vid en given tidpunkt. Beräknade anpassade fält måste uppdateras manuellt, antingen genom att uttrycket beräknas om eller genom att objektet som innehåller beräkningsfältet redigeras och sparas. Det kan vara tidskrävande och lätt att glömma.


</br>
</br>

**Bästa praxis**

Använd beräkningar i en textlägesberäkning i rapportens beskrivning.



**Här är varför**

Om du inkluderar beräkningar av textläge i rapportens beskrivning kan andra förstå hur beräkningen skapades och vilken typ av information den ska visa. Det påminner också systemadministratörerna om hur rapporten skapades ifall det skulle behövas uppdateringar i framtiden.
