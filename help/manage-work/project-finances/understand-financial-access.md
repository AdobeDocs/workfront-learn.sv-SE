---
title: Förstå finansiell åtkomst
description: Se hur administratörer kan styra vilka som får se och redigera den ekonomiska informationen i Workfront.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Förstå finansiell åtkomst

Om din organisation samlar in ekonomiska data med [!DNL Workfront] är det din skyldighet att skydda och hantera vem som har åtkomst att visa och redigera informationen.

Två saker är nödvändiga för att en användare ska kunna visa eller redigera ekonomisk information:

1. Åtkomstbehörighet måste aktiveras på [!UICONTROL åtkomstnivå].
2. Tillstånd att använda dessa åtkomsträttigheter måste beviljas objekt för objekt.

En användare kan till exempel få behörighet att visa ekonomiska data på åtkomstnivå, men kan bara visa ekonomiska data för en uppgift som både delas med användaren och finansiell visning aktiveras när uppgiften delas.

Det är därför möjligt för en användare med [!UICONTROL åtkomstnivå] att visa ekonomiska resurser för att kunna visa ekonomiska resurser på vissa objekt och inte andra, beroende på de enskilda delningsalternativen för dessa objekt. Ingen användare kan dock visa ekonomiska data för något objekt om de inte har behörighet för dem i sin [!UICONTROL åtkomstnivå].

## [!UICONTROL Åtkomstnivå]-inställningar

Allmän åtkomst till ekonomiska data beviljas först av licenstypen [!DNL Workfront].

**[!UICONTROL Planera] licenser kan:**

* Hantera faktureringsposter
* Hantera och visa rollfakturering och kostnadstariffer
* Hantera och visa fakturering och kostnadstariffer för användare
* Hantera utgifter
* Visa och redigera ekonomi

**[!UICONTROL Licenser för arbete] kan:**

* Hantera utgifter
* Visa finanser

**[!UICONTROL Granska] licenser kan:**

* Visa finanser

**Behörigheter kan ändras av [!UICONTROL åtkomstnivån]. De tre alternativen för åtkomst av ekonomiska data är:**

* [!UICONTROL Ingen åtkomst] - Användaren kan inte se ekonomisk information.
* [!UICONTROL Visa] - Användaren kan granska och dela informationen.
* [!UICONTROL Redigera] - Användaren kan skapa, redigera, ta bort och dela informationen. (Endast tillgängligt för en planlicens.)

![En bild som visar allmänna alternativ för ekonomiska data på en åtkomstnivå](assets/setting-up-finances-8.png)

Observera att alternativen [!UICONTROL Visa] och [!UICONTROL Redigera] har ytterligare inställningar för en [!UICONTROL plan]-licens. Klicka på kugghjulet på knappen [!UICONTROL Visa] för följande alternativ:

**[!UICONTROL Visa]**

* Visa fakturering och kostnadstariffer för roller
* Visa fakturering och kostnadstariffer för användare

![En bild som visar visningsalternativ för ekonomiska data på en åtkomstnivå](assets/setting-up-finances-9.png)

**[!UICONTROL Redigera]**

Dessa två alternativ är tillgängliga under alternativet [!UICONTROL Redigera], tillsammans med:

* Redigera rollfakturering och kostnadstariffer
* Redigera fakturering och kostnadstariffer

![En bild som visar redigeringsalternativ för finansiella data på en åtkomstnivå](assets/setting-up-finances-10.png)

>[!NOTE]
>
>En användare som har tillgång till att lägga till utgifter kan även visa de utgifter de lägger till samt de utgifter som läggs till i deras direktrapporter.
