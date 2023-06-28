---
title: Bästa praxis - Förhandsgranska sandlåda
description: Utforska rekommendationer om god praxis från Adobe Workfront experter om hur du konfigurerar, hanterar och använder sandlådemiljön Preview för Workfront.
feature: Strategic Planning
role: Admin, Leader, User
level: Beginner
jira: KT-10917
exl-id: 5e172ad5-7e75-41cd-bce0-858095d13c6c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Bästa praxis - Förhandsgranska sandlåda

## Vad är Adobe Workfront&quot;best practice&quot;?

Bästa metoder är riktlinjer som representerar ett effektivt och verkningsfullt tillvägagångssätt. är lätta att ta till sig av dig och användarna på ditt företag, och kan replikeras i hela organisationen.

När du granskar dessa rekommendationer bör du tänka på att vissa av Workfront bästa metoder är universella medan andra kan vara mer specifika för ämnet. Använd dessa metodtips som ett ramverk för att vägleda installation och användning av Workfront-system.

## Navigera på den här sidan

När du bläddrar igenom den här sidan hittar du först en högnivålista med alla de bästa metoderna för ämnet. På så sätt kan du granska rekommendationerna utan att behöva gå in på detaljerna om varför.

&quot;Varför är de här bästa metoderna?&quot; som finns efter högnivålistan ger mer information om några av de bästa metoderna och varför de anses vara en process, ett verktyg osv., bör du överväga att implementera med din Workfront-instans.

</br>
</br>

## God praxis för förhandsvisning av sandlåda

* Definiera, diagram och testa ändringar av befintliga Workfront-processer eller inställningar i förhandsgranskningssandlådemiljön innan du gör uppdateringar i Production-instansen.

</br>
</br>

## Varför är detta de bästa sätten?

**Bästa praxis**

Definiera, diagram och testa ändringar av befintliga Workfront-processer eller inställningar i förhandsgranskningssandlådemiljön innan du gör uppdateringar i Production-instansen.

**Här är varför**

Sandlådemiljön för förhandsgranskning fungerar som en kopia av din livemiljö. Även om det inte rekommenderas att skapa en hel ny miljö i sandlådan innan du skapar den i Production-instansen, eftersom detta skapar extra arbete, är det bra att använda den som testmiljö för ändringar som du vill implementera.

Genom att utföra UAT-tester (User accept testing) och involvera utvalda användare under testfasen av en ändring kan du få en bättre förståelse för användarnas behov och arbetsflöden. Detta är ett bra sätt att förbättra Workfront arbetsflöden och få bättre acceptans inom er organisation.


**Anteckning**: Alla ändringar som du vill implementera i Workfront behöver inte skapas i förhandsvisningssandlådemiljön först. Många Workfront-ändringar, som att skapa en ny begärandekö eller projektmall, kan göras i produktionsmiljön. En bra tumregel när du testar i ProductionInstance är att styra synligheten för dina objekt tills du är redo att publicera till en större publik. Se till att du tar bort allt som du inte tänker använda så att systemet förblir rent och hanterbart.
