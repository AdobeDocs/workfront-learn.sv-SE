---
title: Förstå e-postaviseringar och korrekturmeddelanden
description: Förstå skillnaden mellan e-postaviseringar och korrekturmeddelanden i  [!DNL &#x200B; Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Förstå e-postaviseringar och korrekturmeddelanden

E-postaviseringar skiljer sig från korrekturmeddelanden via e-post. Du får ett e-postmeddelande om korrektur när du har fått ett nytt korrektur att granska, när ett korrektur är sent eller när det finns en ny version av korrekturet att titta på.

![En bild på ett e-postmeddelande om korrektur som anger att det finns ett nytt korrektur att granska.](assets/email-alert-1.png)

Om du inaktiverar meddelandealternativet när du överför ett korrektur får ingen information från [!DNL Workfront] om att det finns ett nytt korrektur att granska.

E-postaviseringar anges per granskare/godkännare, oftast när korrekturet överförs. En standardtyp för e-postavisering kan tilldelas dina korrekturmottagare så att du inte behöver ange den varje gång du överför ett korrektur. Tala med systemadministratören om hur du får dessa standardinställningar.

![En bild på en e-postavisering som anger att ett beslut har fattats om korrekturet och det finns en kommentar att granska.](assets/email-alert-2.png)

Även om e-postaviseringar är inställda på [!UICONTROL Inaktiverad] får korrekturmottagare ändå ett meddelande om ett nytt korrektur eller en ny version.

## Bästa praxis

| Bästa praxis | Här är varför |
|---|---|
| Inaktivera inställningen&quot;Skicka e-post från Workfront när en kommentar görs på ett korrektur&quot; i Workfront-inställningarna | När den här inställningen är aktiverad (vilket den är som standard) kan användare få flera e-postmeddelanden för varje kommentar i ett korrektur - en från korrekturfunktionen och en från Workfront. De här dubblettmeddelandena orsakar e-postmeddelanden som stör och förvirrar, samt en fullständig e-postinkorg, vilket i slutänden kan leda till att användare ignorerar korrekturmeddelanden som de får. Det kan i sin tur betyda missade deadlines. <br> <br>Obs! Den här inställningen finns på Workfront huvudmeny > Inställningar > E-post > Granska och godkänn. |


