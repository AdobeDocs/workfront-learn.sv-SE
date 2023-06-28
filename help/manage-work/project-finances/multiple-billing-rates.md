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
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Förstå flera faktureringsräntor

Inom [!DNL Workfront], kan projektledaren åsidosätta systemfaktureringstariffer inom ett specifikt projekt. Tidigare påverkades inte bara framtida timmar utan även timmar som redan var inloggade i projektet när den nya faktureringstakten tillämpades på projektet.

Med [!DNL Workfront]Med sin nya funktion för flera faktureringstaxor kan projektledaren bestämma vilken tidsperiod en faktureringstaxa ska tillämpas. På så sätt kan projektledaren avgöra när en avgift ska börja gälla om en frekvens har förhandlats fram eller ändrats.

## Ändra faktureringstariff

1. Gå till projektets landningssida. Välj **[!UICONTROL Faktureringstaxor]** från den vänstra panelen.

   ![En bild av markering [!UICONTROL Faktureringstaxor] in [!DNL Workfront]](assets/project-finances-1.png)

1. Från **[!UICONTROL Faktureringstaxor]** klickar du på **[!UICONTROL Lägg till faktureringsränta]** -knappen. Välj **[!UICONTROL Ny faktureringstakt]** i listrutan.

   ![En bild av markering [!UICONTROL Ny faktureringstakt] in [!DNL Workfront]](assets/project-finances-2.png)

1. The [!UICONTROL Ny faktureringstakt] visas. Från **[!UICONTROL Jobbroll]** väljer du den jobbroll som den nya faktureringstakten ska tillämpas på.

   ![En bild av hur du väljer jobbroller med en ny faktureringsfrekvens i [!DNL Workfront]](assets/project-finances-3.png)

1. När jobbrollen har valts [!UICONTROL Standardfaktureringshastighet] och [!UICONTROL Faktureringsränta 1] visas. Ange den nya faktureringstakten i dialogrutan [!UICONTROL Faktureringsränta 1] fält. Om den faktureringstariffen gäller för hela projektet (tidigare, nuvarande och framtida loggade timmar) klickar du på **[!UICONTROL Spara]** -knappen.

   ![En bild på hur du sparar en ny faktureringsränta som gäller för hela projektet i [!DNL Workfront]](assets/project-finances-5.png)

1. Om den nya faktureringstariffen endast gäller för en viss tidsperiod klickar du på **[!UICONTROL Lägg till frekvens]** -knappen. The [!UICONTROL Faktureringstakt 1 slutdatum] och [!UICONTROL Faktureringsränta 2] visas. Ange slutdatum för [!UICONTROL Faktureringsränta 1]. Du kan inte ange ett startdatum för [!UICONTROL Faktureringsränta 1] eftersom systemet utgår ifrån att det börjar i början av projektet.

   ![En bild på hur du skapar en ny faktureringsränta som gäller för en viss tidsperiod, med början i början av projektet i [!DNL Workfront]](assets/project-finances-6.png)

1. Om så inte är fallet:

   * Ange standardfaktureringssatsen för [!UICONTROL Faktureringsränta 1].
   * Välj slutdatum för [!UICONTROL Faktureringsränta 1] ([!UICONTROL Standardfaktureringshastighet]).
   * Startdatum för [!UICONTROL Faktureringsränta 2] ställs in automatiskt på dagen efter [!UICONTROL Faktureringsränta 1] slutar.
   * Ange önskad faktureringstaxa i dialogrutan [!UICONTROL Faktureringsränta 2] -avsnitt.
   * Fortsätt lägga till faktureringstariffer efter behov genom att klicka på **[!UICONTROL Lägg till frekvens]** -knappen.
   * När du är klar klickar du på **[!UICONTROL Spara]**.
   * Alla faktureringspriser visas i [!UICONTROL Faktureringstaxor] -fliken i projektet.

   ![En bild av hur du skapar nya faktureringstariffer som gäller för de olika tidsperioderna i [!DNL Workfront]](assets/project-finances-7.png)
