---
title: Svar på vanliga frågor om begärandeköer
description: Få svar på vanliga frågor om begärandeköer i [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner, Intermediate
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Svar på vanliga frågor om begärandeköer

**Varför kan jag se en begärandekö, men det går inte för användaren?**

I [!UICONTROL Köinformation] se till att användaren uppfyller villkoren i &quot;Vem kan lägga till begäranden i den här kön?&quot; fält.

**Jag gav användarna åtkomst till kön, men nu kan de även se begärandeköprojektet. Varför?**

Det har att göra med hur du gav dem åtkomst till kön med förfrågningar.

Om du använde [!UICONTROL Delning] på startsidan för projektet i kön för begäranden har du gett dessa användare åtkomst för att se projektet i listan över projekt.

Om du däremot bara vill ge dem åtkomst för att skicka en begäran till kön går du till Köinställningar och väljer lämpligt alternativ under&quot;Vem kan lägga till begäranden till det här projektet&quot;.

**Kan jag omvandla en förfrågan till ett projekt?**

Ja. Du kan konvertera utgåvor till aktiviteter eller projekt beroende på vad som behövs.

Läs den här artikeln för mer information: [Konvertera problem](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**Var hittar jag en begärandekö att redigera?**

Du kan använda [!UICONTROL Sök] i navigeringsfältet eller sök efter det i [!UICONTROL Projekt] område.

Om du öppnar en begäran från begärandekön kan du klicka på projektnamnet i området för vägbeskrivningar.

**Kan jag överföra informationen från ett anpassat formulär till ett anpassat projekt?**

Ja. När du skapar ett anpassat formulär väljer du båda [!UICONTROL Projekt] och [!UICONTROL Problem] som objekttyper. Bifoga det anpassade formuläret till begäran. När du konverterar begäran till ett projekt bifogas det anpassade formuläret automatiskt till det nya projektet och värdena i fälten visas både i det begärda formuläret och i de anpassade projektformulären.

**Jag tittar på ett projekt eller en uppgiftsrapport. Hur tar jag reda på vilken begäran det här objektet kommer från?**

Du har åtkomst till fälten i **[!UICONTROL Konverterat problem]** och **[!UICONTROL Originator för konverterat ärende]** fältkällor för att lägga till den informationen i dina projekt- och uppgiftsrapporter.

**Vilket är det bästa sättet att filtrera efter begärandeköer i en rapport?**

Om projektfiltret innehåller **Kö>>Är offentlig>>Lika>>Ingen** rapporten visar endast projekt som **NOT** begärandeköer.

Om projektfiltret innehåller **Kö>>Är offentlig>>Inte lika med>>Ingen** rapporten visar endast projekt som **ÄR** begärandeköer.
