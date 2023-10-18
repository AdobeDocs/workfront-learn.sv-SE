---
title: Ställ in metadatamappning
description: Lär dig hur du ställer in metadatamappning för [!UICONTROL WORKFRONT DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Ställ in metadatamappning

[!DNL Workfront]-relaterad information om en tillgång kan överföras från [!DNL Workfront] till [!UICONTROL WORKFRONT DAM] med tillgången. Alternativet för metadatamappning i [!DNL Workfront] [!UICONTROL Inställningar] utrymme som möjliggör denna överföring av information.

Tala med [!DNL Workfront] konsult om du vill ha rekommendationer om hur du skapar metadatamappningen.

Du måste vara en [!DNL Workfront] administratör och en [!UICONTROL WORKFRONT DAM] administratör för att konfigurera metadatamappning. Innan du kan börja måste du ansluta [!DNL Workfront] och [!UICONTROL WORKFRONT DAM] konton.

## Anslut konton

1. Logga in på [!DNL Workfront].
1. Öppna ett projekt, en uppgift eller ett ärende och klicka på **[!UICONTROL Dokument]** -fliken.
1. Klicka på **[!UICONTROL Lägg till ny]** knapp och markera **[!UICONTROL Från Workfront DAM]** i listrutan.
1. Ange ditt inloggningsnamn och lösenord i dialogrutan [!UICONTROL WORKFRONT DAM] ruta som visas.
1. Klicka på Nästa **[!UICONTROL Ja]** att ge [!DNL Workfront] åtkomst till [!UICONTROL DAM] konto.
1. Uppdatera sidan om det behövs för att uppdatera åtkomsten till [!UICONTROL WORKFRONT DAM].

När den här anslutningen är upprättad kan du börja mappa metadata mellan de två systemen. Kontrollera att du redan har skapat de metadatafält som behövs i [!UICONTROL WORKFRONT DAM] innan du börjar mappa.

## Konfigurera mappningen

1. Logga in på [!DNL Workfront].
1. Välj **[!UICONTROL Inställningar]** från [!UICONTROL Huvudmeny].
1. Expandera **[!UICONTROL Dokument]** i den vänstra panelmenyn.
1. Klicka sedan på **[!UICONTROL Metadatamappning]**.
1. I fältet Workfront anger du fältkällan för [!DNL Workfront] fält att mappa.
1. Välj sedan motsvarande mål eller mål **[!UICONTROL WORKFRONT DAM]** metadatafält.
1. Klicka på **[!UICONTROL Lägg till mappning]** -knappen.
1. Du kommer att se [!UICONTROL Workfront Field Source] och [!UICONTROL Workfront DAM-målfält] i diagrammet längst ned i fönstret.
1. Upprepa för alla metadatafält du vill använda.

![En skärmbild av [!UICONTROL Metadatamappning] skärm in [!DNL Workfront]](assets/01-metadata-mapping.png)
