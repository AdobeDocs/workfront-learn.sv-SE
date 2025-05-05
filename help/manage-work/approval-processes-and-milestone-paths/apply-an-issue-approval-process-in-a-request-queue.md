---
title: Använda en godkännandeprocess i en begärandekö
description: Implementera en standardprocess för godkännande för att effektivisera arbetsflödena för begäran och säkerställa att godkända begäranden ändrar sin status till"Nytt". Åtgärda förvirring för avvisade begäranden genom att välja en statusändring till "Won't Resolve".
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: 3fc3a58c829769ca06ffb93971ac75516dfbd5f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Använda en godkännandeprocess i en begärandekö

>[!PREREQUISITES]
>
>* [Skapa ett begärandeflöde](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Skapa en global godkännandeprocess och en godkännandeprocess för enstaka användning](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


I videon förklaras hur du tillämpar en standardprocess för godkännande när du skapar en begärandekö. &#x200B; När en begäran skapas börjar den med statusen&quot;Nytt - Väntar på godkännande&quot; och ett meddelande om godkännande skickas till den utsedda godkännaren. &#x200B; Om det godkänns ändras statusen till&quot;Nytt&quot;, vilket innebär att tilldelade personer kan börja arbeta. &#x200B; Om statusen avvisas kan den felaktigt återställas till&quot;Nytt&quot; på grund av ett vanligt fel i konfigurationen av godkännandeprocessen. &#x200B;
I videon visas att godkännandeprocessen aktiveras när statusen är&quot;Nytt&quot;, som är standard för nya begäranden. &#x200B; Om det avvisas ändras statusen till den tidigare statusen som standard, vilket inte är idealiskt för nya begäranden. &#x200B; Du bör istället välja en annan status, till exempel &quot;Won&#39;t Resolve&quot;. &#x200B; I videon visas även att det inte finns någon&quot;Avvisad&quot;-status som standard, men en systemadministratör kan skapa en om det behövs. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops)

## Viktiga uppgifter

* **Standardgodkännandeprocess:** När du skapar en begärandekö kan du använda en standardgodkännandeprocess som automatiskt tilldelar ett godkännandearbetsflöde till varje begäran.
* **Statusändringar vid godkännande:** Godkända begäranden ändrar status från Nytt - väntar på godkännande till Nytt, så att tilldelade personer kan börja arbeta med dem.
* **Allmänt fel i avvisningshantering:** Om en begäran avslås återställs statusen till Nytt på grund av en standardsysteminställning i godkännandeprocessen.
* **Rekommenderad status för nekade begäranden:** I stället för att återgå till den tidigare statusen (&quot;Nytt&quot;) är det bättre att välja en annan status, till exempel&quot;Lös inte&quot;, för att undvika förvirring.
* **Alternativ för anpassad status:** Statusen Avvisad har inte angetts som standard, men en systemadministratör kan skapa en om det behövs för att godkännandeprocessen ska bli tydligare.


## Rekommenderade självstudiekurser i detta ämne

* [Delegera uppgifter, ärenden och godkännanden](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Förstå gruppspecifika godkännandeprocesser](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Skapa ett begärandeflöde](/help/manage-work/request-queues/create-a-request-flow.md)
* [Skapa en global godkännandeprocess och en godkännandeprocess för enstaka användning](https://experienceleague.adobe.com/sv/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
