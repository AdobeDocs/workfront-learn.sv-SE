---
title: Ställ in metadatamappning
description: Lär dig hur du konfigurerar metadatamappning för [!UICONTROL Workfront DAM].
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

[!DNL Workfront]-relaterad information om en resurs kan överföras från [!DNL Workfront] till [!UICONTROL Workfront DAM] med resursen. Metadatamappningsalternativet i området [!DNL Workfront] [!UICONTROL Inställningar] tillåter den här informationsöverföringen.

Tala med din [!DNL Workfront]-konsult för bästa praxis om hur du konfigurerar metadatamappningen.

Du måste vara administratör för [!DNL Workfront] och administratör för [!UICONTROL Workfront DAM] för att kunna konfigurera metadatamappning. Innan du kan starta måste du ansluta dina [!DNL Workfront]- och [!UICONTROL Workfront DAM]-konton.

## Anslut konton

1. Logga in på [!DNL Workfront].
1. Öppna ett projekt, en uppgift eller ett problem och klicka på fliken **[!UICONTROL Dokument]** .
1. Klicka på knappen **[!UICONTROL Lägg till ny]** och välj **[!UICONTROL Från Workfront DAM]** i listrutan.
1. Ange ditt inloggningsnamn och lösenord i rutan [!UICONTROL Workfront DAM] som visas.
1. Klicka sedan på **[!UICONTROL Yes]** för att ge [!DNL Workfront] åtkomst till [!UICONTROL DAM]-kontot.
1. Uppdatera sidan om det behövs för att uppdatera åtkomsten till [!UICONTROL Workfront DAM].

När den här anslutningen är upprättad kan du börja mappa metadata mellan de två systemen. Kontrollera att du redan har skapat de metadatafält som behövs i [!UICONTROL Workfront DAM] innan du börjar mappningen.

## Konfigurera mappningen

1. Logga in på [!DNL Workfront].
1. Välj **[!UICONTROL Konfigurera]** på [!UICONTROL huvudmenyn].
1. Expandera avsnittet **[!UICONTROL Dokument]** på den vänstra panelmenyn.
1. Klicka sedan på **[!UICONTROL Metadatamappning]**.
1. I fältet Workfront anger du fältkällan för fältet [!DNL Workfront] som ska mappas.
1. Markera sedan metadatafältet **[!UICONTROL Workfront DAM]** eller motsvarande.
1. Klicka på knappen **[!UICONTROL Lägg till mappning]**.
1. [!UICONTROL Workfront Field Source] och [!UICONTROL Workfront DAM Target Field] visas i diagrammet längst ned i fönstret.
1. Upprepa för alla metadatafält du vill använda.

![En skärmbild av skärmen [!UICONTROL Metadatamappning] i [!DNL Workfront]](assets/01-metadata-mapping.png)
