---
title: Konfigurera metadatamappning för [!UICONTROL Workfront DAM]
description: Lär dig hur du ställer in metadatamappning för [!UICONTROL Workfront DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
kt: 10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Mappning av metadata

[!DNL Workfront]-relaterad information om en tillgång kan överföras från [!DNL Workfront] till [!UICONTROL Workfront DAM] med tillgången. Alternativet för metadatamappning i [!DNL Workfront] [!UICONTROL Inställningar] kan överföras.

Tala med [!DNL Workfront] konsult om du vill ha rekommendationer om hur du skapar metadatamappningen.

Du måste vara en [!DNL Workfront] administratör och en [!UICONTROL Workfront DAM] administratör för att konfigurera metadatamappning. Innan du kan börja måste du ansluta [!DNL Workfront] och [!UICONTROL Workfront DAM] konton.

## Anslut konton

1. Logga in på [!DNL Workfront].
1. Öppna ett projekt, en uppgift eller ett ärende och klicka på **[!UICONTROL Dokument]** -fliken.
1. Klicka på **[!UICONTROL Lägg till ny]** och markera **[!UICONTROL Från Workfront DAM]** i listrutan.
1. Ange ditt inloggningsnamn och lösenord i dialogrutan [!UICONTROL Workfront DAM] ruta som visas.
1. Klicka på **[!UICONTROL Ja]** att ge [!DNL Workfront] åtkomst till [!UICONTROL DAM] konto.
1. Uppdatera sidan om det behövs för att uppdatera åtkomsten till [!UICONTROL Workfront DAM].

När den här anslutningen är upprättad kan du börja mappa metadata mellan de två systemen. Kontrollera att du redan har skapat de metadatafält som behövs i [!UICONTROL Workfront DAM] innan du börjar mappa.

## Konfigurera mappningen

1. Logga in på [!DNL Workfront].
1. Välj **[!UICONTROL Inställningar]** från [!UICONTROL Huvudmeny].
1. Expandera **[!UICONTROL Dokument]** i den vänstra panelmenyn.
1. Klicka sedan på **[!UICONTROL Metadatamappning]**.
1. I fältet Workfront anger du fältkällan för [!DNL Workfront] fält att mappa.
1. Välj sedan motsvarande mål eller mål **[!UICONTROL Workfront DAM]** metadatafält.
1. Klicka på **[!UICONTROL Lägg till mappning]** -knappen.
1. Du kommer att se [!UICONTROL Workfront Field Source] och [!UICONTROL Workfront DAM-målfält] i diagrammet längst ned i fönstret.
1. Upprepa för alla metadatafält du vill använda.

![En skärmbild av [!UICONTROL Metadatamappning] skärm in [!DNL Workfront]](assets/01-metadata-mapping.png)
