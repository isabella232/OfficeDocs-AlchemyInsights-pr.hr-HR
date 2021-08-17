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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892039"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaje poruka e-pošte u karanteni

Administratori mogu [pregledavati, objavu i brisati te poruke](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Na portalu Microsoft 365 Defender , <https://security.microsoft.com> idite na **Pregled** \> **karantene**. Možete i izravno otići na stranicu **Karantena** pomoću <https://security.microsoft.com/quarantine> .  

Dodatne informacije o vrijednostima pretraživanja/filtriranja koje možete koristiti potražite u članku Upravljanje porukama i datotekama u karanteni [kao administratora u programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Cmdleti koje koristite za prikaz poruka i datoteka u karanteni te upravljanje njima:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet samo za poruke, a ne i datoteke iz Sef privitaka za SharePoint, OneDrive ili Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
