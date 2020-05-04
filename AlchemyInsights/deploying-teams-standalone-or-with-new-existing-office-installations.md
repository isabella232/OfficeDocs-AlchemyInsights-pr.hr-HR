---
title: Implementacija timova kao samostalnih ili s novim ili postojećim instalacijama sustava Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010210"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementacija timova kao samostalnih ili s novim ili postojećim instalacijama sustava Office

Microsoft Teams sada je dio ***novih instalacija*** aplikacija sustava Microsoft 365 za tvrtke, aplikacija microsoft 365 za tvrtke i Office za Mac. Dodatne informacije potražite u [odjeljku Kada će Microsoft Teams početi biti obuhvaćen novim instalacijama sustava Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Osim toga, počevši od verzije 1906 u mjesečnom ***kanalu,*** Timovi će se dodati postojećim instalacijama aplikacija Microsoft 365 za tvrtke (i Microsoft 365 Apps za tvrtke) na uređajima sa sustavom Windows kada postojeću instalaciju ažurirate na najnoviju verziju. Dodatne informacije potražite u [odjeljku Što je s postojećim instalacijama sustava Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ako ne želite čekati ovaj raspored uvođenja, možete implementirati Teams kao samostalne za svoje korisnike slijedeći ove [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) [upute](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ili možete postaviti korisnike da instaliraju Teams za sebe iz sustava .

Ako vaša tvrtka ili ustanova nije spremna za implementaciju timova, imamo korake koje možete poduzeti da ***biste izuzeli Teams*** iz [novih](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ili [postojećih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacija sustava Office. Ako želite instalirati Teams, ali ne želite da se Timovi automatski pokreću za korisnika nakon instalacije, pročitajte u [odjeljku Sprječavanje automatskog pokretanja servisa Microsoft Teams nakon instalacije](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Da biste ***instalirali Teams*** s uređaja sa sustavom Windows, [pročitajte članku Deinstalacija servisa Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Da biste očistili Microsoft Teams s više ciljanih računala ili korisnika, pročitajte popis [implementacije programa Microsoft Teams .](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Ako koristite zajednička računala, servise udaljene radne površine (RDS) ili infrastrukturu virtualne radne površine (VDI), [pročitajte članak Zajedničko računalo i VDI okruženja s programom Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ako koristite Office za Mac, pročitajte upute [za Microsoft Teams na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Nakon instalacije aplikacije Teams automatski se [ažuriraju](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) otprilike svaka dva tjedna novim značajkama i ažuriranjima kvalitete. 