---
title: Svar på vanliga frågor om begärandeköer
description: Få svar på vanliga frågor om begärandeköer i  [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Svar på vanliga frågor om begärandeköer

**Varför kan jag se en begärandekö, men min användare kan inte det?**

På fliken [!UICONTROL Köinformation] i kön/projektet för din begäran kontrollerar du att användaren uppfyller villkoren för &quot;Vem kan lägga till begäranden i den här kön?&quot; fält.

**Jag gav användarna åtkomst till kön, men nu kan de även se begärandeköprojektet. Varför?**

Det har att göra med hur du gav dem åtkomst till kön med förfrågningar.

Om du har använt [!UICONTROL delningsverktyget] från startsidan för projektet i kön för begäranden har du gett dessa användare åtkomst för att se projektet i listan över projekt.

Om du däremot bara vill ge dem åtkomst för att skicka en begäran till kön går du till Köinställningar och väljer lämpligt alternativ under&quot;Vem kan lägga till begäranden till det här projektet&quot;.

**Kan jag omvandla en begäran till ett projekt?**

Ja. Du kan konvertera utgåvor till aktiviteter eller projekt beroende på vad som behövs.

Mer information finns i den här artikeln: [Konvertera problem](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**Var hittar jag en begärandekö att redigera?**

Du kan använda fältet [!UICONTROL Sök] i navigeringsfältet eller söka efter det i området [!UICONTROL Projekt] .

Om du öppnar en begäran från begärandekön kan du klicka på projektnamnet i området för vägbeskrivningar.

**Kan jag överföra informationen från ett anpassat begärandeformulär till ett anpassat projektformulär?**

Ja. När du skapar ett anpassat formulär väljer du både [!UICONTROL Projekt] och [!UICONTROL Problem] som objekttyper. Bifoga det anpassade formuläret till begäran. När du konverterar begäran till ett projekt bifogas det anpassade formuläret automatiskt till det nya projektet och värdena i fälten visas både i det begärda formuläret och i de anpassade projektformulären.

**Jag tittar på ett projekt eller en aktivitetsrapport. Hur kan jag ta reda på vilken begäran det här objektet kommer från?**

Du kan komma åt fält i fälten **[!UICONTROL Konverterat problem]** och **[!UICONTROL Konverterat ärende-original]** för att lägga till den informationen i projekt- och aktivitetsrapporter.

**Vilket är det bästa sättet att filtrera efter begärandeköer i en rapport?**

Om ditt projektfilter innehåller **Kö>>Är offentlig>>Lika>>Inget** visas endast projekt som är **NOT**-begärandeköer i rapporten.

Om ditt projektfilter innehåller **Kö>>Är offentlig>>Inte lika med>>Ingen** visas endast projekt som **ARE**-frågeköer för.
