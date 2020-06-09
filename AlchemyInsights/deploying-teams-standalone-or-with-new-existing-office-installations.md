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
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617887"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementacija timova kao samostalnih ili s novim ili postojećim instalacijama sustava Office

Microsoft Teams sada je dio ***novih instalacija*** aplikacija microsoft 365 za tvrtke, Aplikacija microsoft 365 za tvrtke i sustava Office za Mac. Dodatne informacije potražite u odjeljku [Kada će Microsoft Teams početi biti uključen u nove instalacije sustava Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Uz to, počevši od verzije 1906 u trenutnom kanalu , timovi će se ***dodati postojećim instalacijama*** aplikacija microsoft 365 za tvrtke (i Microsoft 365 Aplikacije za tvrtke) na uređajima sa sustavom Windows kada ažurirate postojeću instalaciju na najnoviju verziju. Dodatne informacije potražite u [odjeljku Što o postojećim instalacijama sustava Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ako ne želite čekati ovaj raspored uvođenja, možete implementirati Teams kao samostalne za svoje korisnike [slijedeći ove upute](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ili možete imati svoje korisnike da instaliraju Teams za sebe iz  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) sustava .

Ako vaša tvrtka ili ustanova nije spremna za implementaciju programa Teams, imamo korake koje možete poduzeti da biste ***izmakle aplikacije Teams*** iz [novih](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ili [postojećih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacija sustava Office. Ako želite da teams bude instaliran, ali ne želite da se Teams automatski pokreće za korisnika nakon instalacije, [pročitajte mogućnost Sprječavanje automatskog pokretanja servisa Microsoft Teams nakon instalacije](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Upute ***za deinstalaciju aplikacije Teams*** s uređaja sa sustavom Windows [potražite u odjeljku Deinstalacija programa Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Da biste očistili Microsoft Teams s više ciljnih računala ili korisnika, pogledajte [čišćenje implementacije programa Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ako koristite dijeljena računala, servise udaljene radne površine (RDS) ili infrastrukturu virtualne radne površine (VDI), pročitajte članak [Dijeljeno računalo i VDI okruženja s programom Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ako koristite Office za Mac, pogledajte [instalacije servisa Microsoft Teams na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Nakon instalacije aplikacije Teams automatski se [ažurira](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) otprilike svaka dva tjedna novim značajkama i ažuriranjima kvalitete. 