---
title: Uvođenje timovima kao samostalni ili uz nove ili postojeće instalacije sustava Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054223"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Uvođenje timovima kao samostalni ili uz nove ili postojeće instalacije sustava Office

Sada je Microsoft Teams uključene kao dio ***nove instalacije*** Office 365 ProPlus, Office 365 Business i Office za Macu Za dodatne informacije pogledajte [će Microsoft Teams početka nove instalacije paketa Office koji se uključene?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Uz to, počevši s 1906 verziju u kanal mjesečno, timovima bit će ***dodan postojeće instalacije*** Office 365 ProPlus (i Office 365 Business) na uređajima sustavom Windows kada ažurirate postojeće instalacije na najnoviju verziju. Za dodatne informacije pogledajte [što o postojeće instalacije paketa Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Ako ne želite čekati za ovaj raspored rollout, možete implementirati timovima kao samostalni za korisnike slijedeći [ove upute](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ili imate korisnici instalirati timovima za same iz [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Ako vaša organizacija nije spremna za uvođenje timovima, imamo korake koje možete poduzeti za ***timova isključivanje*** iz [nove](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) ili [postojeće](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacije paketa Office. Ako želite timovima instaliran, ali ne želite timovima za automatsko pokretanje za korisnika nakon instalacije, pogledajte [Spriječiti Microsoft timovima iz Početni automatski nakon instalacije](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Da biste ***deinstalirali timove*** s uređaja sa sustavom Windows potražite [Deinstalirati Microsoft timovima](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Čišćenje Microsoft Teams s više ciljana računala ili korisnike, pogledajte [Microsoft timovima uvođenja očistiti](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ako koristite zajednička računala, uslugama udaljene radne površine (ZAPISI) ili Infrastruktura virtualne radne površine (VDI), pogledajte [zajedničko računalo i VDI okruženju s Microsoft timovima](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ako koristite Office za Mac pogledajte [Microsoft timovima instalacije na u Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Nakon instalacije timove je [automatski ažurira](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približno svaka dva tjedna novim značajkama i kvalitete ažuriranja. 