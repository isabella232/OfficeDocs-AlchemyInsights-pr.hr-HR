---
title: Nedostaju poruke e-pošte u karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568964"
---
# <a name="missing-emails-in-quarantine"></a>Nedostaju poruke e-pošte u karanteni"

Administratori mogu [pregledavati, objavljivati ili brisati te poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Da biste otvorili Centar za usklađenost sa sigurnosnim &, idite na [https://protection.office.com](https://protection.office.com/) . Da biste izravno otvorili stranicu Karantena, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete pretraživati prema sljedećim vrijednostima:  

- **ID poruke**: globalno jedinstveni identifikator poruke. Ako odaberete poruku na popisu, vrijednost **ID poruke** pojavljuje se u oknu potpalete **detalji** koje će se pojaviti. Administratori mogu koristiti [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i njihove odgovarajuće vrijednosti ID-a poruka.
- **Adresa e-pošte pošiljatelja**: adresa e-pošte jednog pošiljatelja.
- **Adresa e-pošte primatelja**: E-adresa jednog primatelja.
- **Predmet**: Koristite cijeli predmet poruke. Pretraživanje ne razlikuje velika i mala slova.

Kada unesete kriterije pretraživanja, kliknite ![ Osvježi gumb ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osvježi** da biste filtrirali rezultate.  

Cmdleti koje koristite za prikaz i upravljanje porukama i datotekama u karanteni su:
- [Brisanje karanteneMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz-KarantenaMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ovaj cmdlet namijenjen samo porukama, a ne za datoteke zlonamjernog softvera iz ATP-a za SharePoint Online, OneDrive za tvrtke ili timove.
- [Izdanje-KarantenaMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)