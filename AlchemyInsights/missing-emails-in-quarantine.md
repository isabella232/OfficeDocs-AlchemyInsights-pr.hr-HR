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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026214"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaje poruka e-pošte u karanteni"

Administratori mogu [pregledavati, objavu i brisati te poruke.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Da biste otvorili centar za & usklađenosti, idite na [https://protection.office.com](https://protection.office.com/) . Da biste izravno otvorili stranicu Karantena, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete pretraživati prema sljedećim vrijednostima:  

- **ID poruke:** globalno jedinstveni identifikator poruke. Ako na popisu odaberete poruku, u oknu  s detaljima koja će se prikazati prikazat će se vrijednost **ID** poruke. Administratori mogu koristiti [praćenje poruka da bi](/microsoft-365/security/office-365-security/message-trace-scc) pronašli poruke i njihove odgovarajuće vrijednosti ID-a poruke.
- **Adresa e-pošte** pošiljatelja: adresa e-pošte jednog pošiljatelja.
- **Adresa e-pošte** primatelja: adresa e-pošte jednog primatelja.
- **Predmet:** koristite cijeli predmet poruke. Pretraživanje ne može umašati velika i mala slova.

Kada unesete kriterije pretraživanja, kliknite Osvježi gumb ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osvježi da** biste filtrirali rezultate.

Cmdleti koje koristite za prikaz poruka i datoteka u karanteni i upravljanje njima:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet samo za poruke, a ne i za datoteke zlonamjernog softvera programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive za tvrtke ili Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)