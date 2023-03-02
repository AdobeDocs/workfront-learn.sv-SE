---
title: Redigera en automatiserad arbetsflödesmall
description: Lär dig hur du ändrar en befintlig arbetsflödesmall för automatisk korrekturläsning i [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
kt: 8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Redigera en automatiserad arbetsflödesmall

I takt med att gransknings- och godkännandeprocesserna förfinas eller organisatoriska förändringar görs bör automatiserade arbetsflödesmallar uppdateras för att återspegla den aktuella verksamheten för era team med Workfront.

Genom att hålla mallarna uppdaterade får du en konsekvent gransknings- och godkännandeprocess, och dessutom sparar du tid för dem som laddar upp korrektur eftersom de inte behöver ändra något arbetsflöde hela tiden.

1. Välj **[!UICONTROL Korrektur]** från **[!UICONTROL Huvudmeny]** in [!DNL Workfront].
1. Välj **[!UICONTROL Arbetsflöden]** i den vänstra panelmenyn.
1. Klicka på menyn med tre punkter längst till höger om mallnamnet och välj **[!UICONTROL Visa mallinformation]**.

Alternativ för att dela, kopiera och ta bort mallen finns längst upp i mallinformationsfönstret för varje mall. Om du tar bort en mall påverkas inte korrektur som använder mallen, men det betyder att mallen inte längre är tillgänglig.

![Mallinformationsfönster](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Klicka på pilen för att utöka [!UICONTROL Detaljer] för att ändra saker som mallnamnet eller mallens tidszon.

## Gör ändringar i stadier och mottagare

Ändringar kan behövas i [!UICONTROL Arbetsflöde] när en smidig process innebär en tidigare deadline eller när någon går med i teamet och kommer att granska korrektur.

Varje steg i ett automatiserat arbetsflöde har ett eget avsnitt där du kan ändra deadlines, sekretess, korrekturmottagare och annan information oberoende av varandra.

I den här videon visas några av de ändringar du kan göra i [!UICONTROL Arbetsflöde] område. Se punktlistan under den här videon som visar dessa inställningar. Det finns inget ljud i den här videon.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12)

Här är korrekturmallsändringarna som du kan göra i [!UICONTROL Arbetsflöde] avsnitt:

* Klicka på [!UICONTROL scennamn] fält eller [!UICONTROL deadline] fält för att uppdatera informationen.
* Markera pilen bredvid [!UICONTROL deadline] för att låsa scenen, avgöra när scenen aktiveras eller endast kräva ett beslut.
* Klicka på i listan över mottagare [!UICONTROL Roll] eller [!UICONTROL E-postaviseringar] fält för att välja ett annat alternativ.
* Gå till menyn med tre punkter längst till höger om namnet på en mottagare om du vill ta bort dem från listan, göra dem till den primära beslutsfattaren för arbetsflödessteget eller redigera korrekturrollen och e-postaviseringsinformationen.
* Du har två alternativ för att lägga till mottagare i listan. När du har öppnat [!UICONTROL Lägg till personer på scenen] klickar du på den scen du vill lägga till dem i. Ange sedan deras namn eller e-postadress i mottagarlistan och tilldela en korrekturroll och en e-postavisering. Klicka på [!UICONTROL Lägg till personer] när du är klar.
   1. I det övre högra hörnet av varje scenavsnitt går du till [!UICONTROL Mer] meny och välj [!UICONTROL Lägg till personer på scenen].
   1. Överst på [!UICONTROL Arbetsflöde] område, markera [!UICONTROL Lägg till personer på scenen].

## Malldelning

The [!UICONTROL Delas med] -området visar de korrekturanvändare som kan använda mallen. Ta bort personer som inte längre behöver använda mallen genom att klicka på menyn med tre punkter längst till höger om namnet och välja [!UICONTROL Ta bort].

![[!UICONTROL Delas med] list](assets/proof-system-setups-edit-template-shared-with.png)

Du kan dock inte lägga till personer i delningslistan från det här avsnittet. Det gör du genom att gå tillbaka till mallinformationsfönstrets överkant och klicka på [!UICONTROL Dela mall] -knappen.

## Aktivitetsavsnittet

[!DNL Workfront] sparar en granskningshistorik över när ändringar gjordes i mallen. Du kan se datumet, vem som gjorde ändringen och en del kortfattad information om vilka ändringar som gjordes.

I det här avsnittet registreras ingen information om när mallen användes på korrektur.

![Lista över korrekturaktiviteter](assets/proof-system-setups-edit-template-activity.png)
