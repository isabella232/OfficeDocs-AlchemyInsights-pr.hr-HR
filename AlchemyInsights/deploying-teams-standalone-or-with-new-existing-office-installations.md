---
title: Implementacija Teams kao samostalna ili s novim ili postojećim Office instalacijama
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320114"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Implementacija Teams kao samostalna ili s novim ili postojećim Office instalacijama

Microsoft Teams sada je dio novih ***instalacija*** sustava Microsoft 365 Apps za velike tvrtke, Microsoft 365 Apps za male tvrtke i Office za Mac. Dodatne informacije potražite u članku [Kada Microsoft Teams biti obuhvaćena novim instalacijama sustava Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Uz ***to,*** počevši od verzije 1906 u trenutnom kanalu , Teams će se dodati u postojeće instalacije sustava Microsoft 365 Apps za velike tvrtke (i Microsoft 365 Apps za male tvrtke) na uređajima sa sustavom Windows kada postojeću instalaciju ažurirate na najnoviju verziju. Dodatne informacije potražite u članku [Što je s postojećim instalacijama sustava Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Napomena**: ako ne želite čekati ovaj raspored uvođenja, možete implementirati Teams kao samostalnu [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) implementaciju za korisnike slijedeći ove upute ili korisnici mogu sami instalirati Teams za [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) sebe.

Ako vaša tvrtka ili ustanova nije spremna za implementaciju Teams, imamo korake koje [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) možete poduzeti ***da Teams*** iz novih ili [postojećih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacija Office. Ako želite Teams instalaciju, ali ne želite da se Teams automatski pokreće za korisnika nakon instalacije, pogledajte Microsoft Teams onemogućivanje automatskog pokretanja [nakon instalacije.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Da ***biste Teams s*** uređaja sa sustavom Windows, pogledajte [deinstalaciju Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Da biste očistili Microsoft Teams više ciljnih računala ili korisnika, pogledajte [Microsoft Teams čišćenje implementacije](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ako koristite zajednička računala, servise udaljene radne površine (RDS) ili infrastrukturu virtualne radne površine (VDI), pogledajte zajedničko računalo i [VDI okruženja s Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ako koristite e-Office za Mac, pogledajte [Microsoft Teams instalacije na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**Napomena:** nakon Teams instalacije automatski se [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ažurira otprilike svaka dva tjedna novim značajkama i ažuriranjima kvalitete. 