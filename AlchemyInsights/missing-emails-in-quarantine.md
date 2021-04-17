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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831726"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaje poruka e-pošte u karanteni"

Administratori mogu [pregledavati, objavu i brisati te poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Da biste otvorili centar za & usklađenosti, idite na [https://protection.office.com](https://protection.office.com/) . Da biste izravno otvorili stranicu Karantena, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete pretraživati prema sljedećim vrijednostima:  

- **ID poruke:** globalno jedinstveni identifikator poruke. Ako na popisu odaberete poruku, u oknu  s detaljima koja će se prikazati prikazat će se vrijednost **ID** poruke. Administratori mogu koristiti [praćenje poruka da bi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pronašli poruke i njihove odgovarajuće vrijednosti ID-a poruke.
- **Adresa e-pošte** pošiljatelja: adresa e-pošte jednog pošiljatelja.
- **Adresa e-pošte** primatelja: adresa e-pošte jednog primatelja.
- **Predmet:** koristite cijeli predmet poruke. Pretraživanje ne može umašati velika i mala slova.

Kada unesete kriterije pretraživanja, kliknite Osvježi gumb ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osvježi da** biste filtrirali rezultate.  

Cmdleti koje koristite za prikaz poruka i datoteka u karanteni i upravljanje njima:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet samo za poruke, a ne i za datoteke zlonamjernog softvera iz sustava ATP za SharePoint Online, OneDrive za tvrtke ili Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)