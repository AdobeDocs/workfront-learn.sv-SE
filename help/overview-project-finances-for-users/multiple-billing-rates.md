---
title: Förstå flera faktureringsräntor
description: Lär dig hur du åsidosätter systemfaktureringstaxor i ett projekt.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
source-git-commit: d7347d41099e0faf6b47a6fe0e58091105e4e41d
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Förstå flera faktureringsräntor

Inom [!DNL Workfront] kan en projektledare åsidosätta systemfaktureringstariffer inom ett visst projekt. Tidigare påverkades inte bara framtida timmar utan även timmar som redan var inloggade i projektet när den nya faktureringstakten tillämpades på projektet.

Med den nya funktionen för flera faktureringstaxor för [!DNL Workfront] kan projektledaren bestämma vilken tidsperiod en faktureringstaxa ska tillämpas. På så sätt kan projektledaren avgöra när en avgift ska börja gälla om en frekvens har förhandlats fram eller ändrats.

## Ändra faktureringstariff

1. Gå till projektets landningssida. Välj **[!UICONTROL Faktureringstariffer]** i den vänstra panelen.

   ![En bild på hur du väljer [!UICONTROL Faktureringstariffer] i [!DNL Workfront]](assets/project-finances-1.png)

1. Klicka på knappen **[!UICONTROL Lägg till faktureringstakt]** på fliken **[!UICONTROL Faktureringstariffer]** . Välj **[!UICONTROL Ny faktureringstakt]** i listrutan.

   ![En bild på hur du väljer [!UICONTROL Ny faktureringsfrekvens] i [!DNL Workfront]](assets/project-finances-2.png)

1. Dialogrutan [!UICONTROL Ny faktureringshastighet] visas. I listrutan **[!UICONTROL Jobbroll]** väljer du den jobbroll som den nya faktureringssatsen ska tillämpas på.

   ![En bild av hur du väljer jobbroller i en ny faktureringsfrekvens i [!DNL Workfront]](assets/project-finances-3.png)

1. När jobbrollen har valts visas fälten [!UICONTROL Standardfaktureringshastighet] och [!UICONTROL Faktureringshastighet 1]. Ange den nya faktureringstakten i fältet [!UICONTROL Faktureringstakt 1]. Om den faktureringstakten gäller för hela projektet (tidigare, nuvarande och framtida loggade timmar) klickar du på knappen **[!UICONTROL Spara]** .

   ![En bild på hur du sparar en ny faktureringsfrekvens som gäller för hela projektet i [!DNL Workfront]](assets/project-finances-5.png)

1. Om den nya faktureringstariffen endast gäller för en viss tidsperiod klickar du på knappen **[!UICONTROL Lägg till kurs]** . Fälten [!UICONTROL Faktureringshastighet 1 Slutdatum] och [!UICONTROL Faktureringshastighet 2] visas. Ange slutdatum för [!UICONTROL faktureringstakt 1]. Du kan inte ange ett startdatum för [!UICONTROL Faktureringshastighet &#x200B;] eftersom systemet antar att det startade i början av projektet.

   ![En bild på hur du skapar en ny faktureringsfrekvens som gäller för en viss tidsperiod, med början i början av projektet i [!DNL Workfront]](assets/project-finances-6.png)

1. Om så inte är fallet:

   * Ange standardfaktureringstakten för [!UICONTROL faktureringstariff 1].
   * Välj slutdatum för [!UICONTROL faktureringshastighet 1] ([!UICONTROL standardfaktureringshastighet]).
   * Startdatumet för [!UICONTROL Faktureringshastighet &#x200B;] anges automatiskt till dagen efter att [!UICONTROL faktureringshastighet 1] avslutas.
   * Ange önskad faktureringstaxa i avsnittet [!UICONTROL Faktureringstakt 2].
   * Fortsätt att lägga till faktureringstariffer efter behov genom att klicka på knappen **[!UICONTROL Lägg till ränta]**.
   * När du är klar klickar du på **[!UICONTROL Spara]**.
   * Alla faktureringstariffer visas på fliken [!UICONTROL Faktureringstariffer] i projektet.

   ![En bild på hur du skapar nya faktureringsfrekvenser som gäller för olika tidsperioder i [!DNL Workfront]](assets/project-finances-7.png)
