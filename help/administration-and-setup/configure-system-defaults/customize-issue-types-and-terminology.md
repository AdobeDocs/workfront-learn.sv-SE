---
title: Anpassa problemtyper och terminologi
description: Lär dig hur du anpassar och byter namn på de fyra standardutgåvorna så att de passar din organisations behov.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10021
exl-id: d1e5c2d6-b001-4e9e-b72d-c792c70d09e8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Anpassa problemtyper och terminologi

## Byt namn på standardutgåvorna

[!DNL Workfront] innehåller fyra typer av problem som hjälper dina användare att kategorisera den typ av problem som skapas. Standardvärdena är:

* [!UICONTROL Felrapport]
* [!UICONTROL Ändra ordning]
* [!UICONTROL Utgåva]
* [!UICONTROL Begäran]

Vad händer om de befintliga problemtyperna inte matchar organisationens behov av problemhantering? Eller så använder din organisation en annan terminologi?

Det finns t.ex. ett team som vill spåra projektrisker med hjälp av problem. Som systemadministratör vet du att din organisation inte spårar felrapporter. Så du kan ändra namnet på en oanvänd utgåva, som [!UICONTROL Felrapporter], till Projektrisker.

Ärendetyperna har bytt namn på hela systemet, så ändringen gäller alla användare.

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Expandera avsnittet **[!UICONTROL Projektinställningar]** på den vänstra menypanelen.
1. Välj **[!UICONTROL Status]**.
1. Välj fliken **[!UICONTROL Problem]**.
1. Kontrollera att menyn i det övre högra hörnet är inställd på [!UICONTROL Systemstatus].
1. Håll markören bredvid en problemtyp högst upp i listan. Klicka på pennikonen för att aktivera fältredigering.
1. Byt namn på problemtypen.
1. Klicka utanför fältet som du vill spara.

![[!UICONTROL Problem] på fliken [!UICONTROL Status] på sidan [!UICONTROL Inställningar]](assets/admin-fund-issue-types.png)

>[!NOTE]
>
>Du kan inte skapa fler typer av utgåvor eller ta bort en utgåva.

<!---
learn more URLs
Customize default issue types
--->

## Ändra termen&quot;problem&quot; i Workfront

Vissa organisationer använder en annan term än&quot;issue&quot; för att hänvisa till oplanerade arbetsuppgifter. Problemet är standardtermen och visas i alla program - menyer, rapporter, fältnamn osv.
Workfront-administratörer kan använda layoutmallsfunktionen för att byta namn på problemobjektet så att det matchar organisationens terminologi. Den nya termen visas sedan i hela [!DNL Workfront] för dem som är tilldelade layoutmallen.

![[!UICONTROL Terminologi] fönster med [!UICONTROL Problem] markerat](assets/admin-fund-issue-custom-terminology.png)

<!---
paragraph below needs a hyperlink
--->

Lär dig hur system- och gruppadministratörer kan skapa layoutmallar i utbildningsvägen, Grundläggande om administratörer i den nya [!DNL Workfront]-upplevelsen: Del 3 Kontroll- och gränssnittsupplevelse.

<!---
learn more URLs
Create and manage layout templates
--->
