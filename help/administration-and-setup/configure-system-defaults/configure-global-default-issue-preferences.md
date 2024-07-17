---
title: Konfigurera inställningar för globala standardproblem
description: Lär dig hur du anger inställningar för problem med konverterade utgåvor, faktiska datum och åtkomst till utgåvor.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Konfigurera inställningar för globala standardutgåvor

Flera systemomfattande inställningar fastställer standardinställningar för hur problem fungerar under vissa omständigheter i [!DNL Workfront].

Bästa sättet är att lämna de globala standardvärdena som de är och låta projektledarna göra de justeringar de behöver på projektnivå eller i projektmallar.

De globala inställningarna för utgåvor kan justeras, men du och din [!DNL Workfront]-konsult bör diskutera vilka inställningar som behövs för din organisations arbetsflöden, processer och rapporteringsbehov. Din konsult kan också hjälpa dig att förstå vad som kommer att hända om vissa inställningar ändras.

Med inställningar för problem kan systemadministratörer styra alternativen när utgåvor konverteras till aktiviteter eller projekt, hur faktiska datum beräknas och vem som får projektåtkomst när utgåvor tilldelas. Låt oss titta på var dessa inställningar finns i [!DNL Workfront].

## Inställningar för konverterat problem

De här inställningarna styr vad som händer med ett problem när det konverteras till en aktivitet eller ett projekt i [!DNL Workfront].

Inställningsfönstret ![[!UICONTROL Åtgärder och problem] med avsnittet [!UICONTROL Problem] markerat](assets/admin-fund-issue-prefs-converting.png)

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Expandera avsnittet **[!UICONTROL Projektinställningar]** på den vänstra menypanelen.
1. Välj **[!UICONTROL Åtgärder och problem]**.
1. Bläddra till avsnittet **[!UICONTROL Problem]**.
1. Klicka på önskade alternativ.
1. Spara när du är klar.

Låt oss titta på alternativen i det här avsnittet så att du kan välja rätt alternativ för din organisation.

* **[!UICONTROL Uppdatera automatiskt status för lösta problem när statusen för det lösta objektet ändras]**

  Med den här inställningen kan du korrelera upplösningen för den ursprungliga utgåvan med upplösningen för det nya objektet (uppgift eller projekt).

  När den här inställningen är aktiverad (markerad) kan du skapa anpassade utgivningsstatusar som har samma statusnyckel som en aktivitet eller projektstatus. När aktiviteten eller projektet (det lösta objektet) är inställt på anpassad status visas ändringen även på problemstatusen.

  När det här alternativet är inaktiverat anges objektets status automatiskt till standardstatus i stället för anpassade.

  För att den här inställningen ska ha någon effekt måste alternativet [!UICONTROL Behåll det ursprungliga problemet och koppla dess upplösning till aktiviteten] vara markerat.

* **[!UICONTROL Behåll det ursprungliga problemet och knyt tid till aktiviteten/projektet]**

  När utgåvan konverteras visas information om att de ursprungliga utgåvorna ska behållas av [!DNL Workfront]. Status för utleverans ändras när status för aktiviteten eller projektet ändras. När aktiviteten eller projektet har markerats som slutfört markeras problemet som löst.

  Om det här alternativet inte är markerat tas den ursprungliga utgåvan bort och endast den konverterade uppgiften eller det konverterade projektet återstår.

  Den här inställningen påverkar rapportering om problem som ursprungligen loggades i ett projekt eller som kom via en [!DNL Workfront]-begärandekö.

* **[!UICONTROL Tillåt att primär kontakt har åtkomst till aktiviteten/projektet]**

  Detta ger den person som skapade den ursprungliga utgåvan åtkomst till uppgiften eller projektet som skapades under konverteringen. De kan granska materialet, göra uppdateringar och hålla sig informerade om hur det utvecklas.

* **[!UICONTROL Tillåt att de här inställningarna ändras under konverteringen]**

  När det här alternativet är markerat innebär det att standardinställningarna för [!UICONTROL Behåll ursprungligt problem] och [!UICONTROL Tillåt primär kontakt] kan ändras av användaren som konverterar problemet. Om du vill att standardinställningarna ska vara oförändrade avmarkerar du det här alternativet.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Inställningar för faktiska datum

Flera typer av datum används i hela [!DNL Workfront]. Faktiska datum är en&quot;tidsstämpel&quot; som [!DNL Workfront] genererar när vissa statusändringar inträffar.

Tidsstämpeln [!UICONTROL Faktiskt startdatum] skapas när utgivningsstatusen ändras från Nytt till en annan status. Tidsstämpeln [!UICONTROL Faktiskt slutförandedatum] är när utgivningsstatusen ändras till en status som anger att den är stängd.

Det är viktigt att komma ihåg att den här inställningen styr de faktiska datuminställningarna för både uppgifter och ärenden.

Inställningsfönstret ![[!UICONTROL Uppgifter och problem] med avsnittet [!UICONTROL Faktiska datum] markerat](assets/admin-fund-issue-prefs-actual-dates.png)

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Expandera avsnittet **[!UICONTROL Projektinställningar]** på den vänstra menypanelen.
1. Välj **[!UICONTROL Åtgärder och problem]**.
1. Bläddra till avsnittet **[!UICONTROL Faktiska datum]**.
1. Välj önskat alternativ för **[!UICONTROL Faktiskt startdatum]** — [!UICONTROL Nu] (aktuellt datum och tid) eller [!UICONTROL Planerat startdatum] (det [!UICONTROL faktiska startdatumet] matchar startdatumet som angetts i probleminformationen).
1. Välj nu alternativet för **[!UICONTROL Faktiskt slutförandedatum]** — [!UICONTROL Nu] (aktuellt datum och tid) eller [!UICONTROL Planerat slutförandedatum] (det [!UICONTROL faktiska startdatumet] matchar det datum som angetts i probleminformationen).
1. Spara när du är klar.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Utfärda åtkomst

[!UICONTROL Åtkomst]-inställningarna för problem styr vilken åtkomst en användare får när de tilldelas ett problem i Workfront. Dessa inställningar styr åtkomsten till själva problemet, förutom åtkomsten till det projekt som problemet är kopplat till.

Innan du ändrar de här inställningarna ska du diskutera eventuella arbetsflödes- eller processbehov med dina [!DNL Workfront]-konsulter och ditt interna ledningsgrupp.

Inställningsfönstret ![[!UICONTROL Uppgifter och problem] med inställningsfönstret [!UICONTROL När någon tilldelas till ett UTGÅVA] markerat](assets/admin-fund-issue-prefs-access-1.png)

1. Klicka på **[!UICONTROL Konfigurera]** på **[!UICONTROL Huvudmenyn]**.
1. Expandera avsnittet **[!UICONTROL Projektinställningar]** på den vänstra menypanelen.
1. Välj **[!UICONTROL Åtgärder och problem]**.
1. Bläddra till avsnittet **[!UICONTROL Åtkomst]** och hitta alternativet [!UICONTROL När någon har tilldelats till ett UTGÅVA].
1. Ange delningsåtkomst för själva utgåvan - [!UICONTROL Visa], [!UICONTROL Contribute] eller [!UICONTROL Hantera]. [!DNL Workfront] rekommenderar att du låter de avancerade alternativen vara som de är.
1. Markera kryssrutan om den som tilldelats utgåvan även ska ha tillgång till projektet
1. Välj sedan delningsåtkomst för projektet: [!UICONTROL Visa], [!UICONTROL Contribute] eller [!UICONTROL Hantera]. När du anger [!UICONTROL Avancerade alternativ] bör du tänka på organisationens arbetsflöden och åtkomstbehov.
1. Spara när du är klar.

Fönstret ![[!UICONTROL Åtkomst] med [!UICONTROL Contribute]-alternativ](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
