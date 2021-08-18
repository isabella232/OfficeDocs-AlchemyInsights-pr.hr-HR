---
title: Nedostaje poruka e-pošte u karanteni
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329654"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaje poruka e-pošte u karanteni

Administratori mogu [pregledavati, objavu i brisati te poruke](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Na portalu Microsoft 365 Defender u <https://security.microsoft.com> idite na **Pregled** \> **karantene**. Možete i izravno otići na stranicu **Karantena** pomoću <https://security.microsoft.com/quarantine> .  

Dodatne informacije o vrijednostima pretraživanja/filtriranja koje možete koristiti potražite u članku Upravljanje porukama i datotekama u karanteni [kao administratora u programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Cmdleti koje koristite za prikaz poruka i datoteka u karanteni te upravljanje njima:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet samo za poruke, a ne i datoteke iz Sef privitaka za SharePoint, OneDrive ili Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
