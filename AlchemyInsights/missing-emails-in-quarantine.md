---
title: Propuštate poruke e-pošte u karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673706"
---
# <a name="missing-emails-in-quarantine"></a>Propuštate poruke e-pošte u karanteni "

Administratori mogu [pregledavati, objaviti ili brisati te poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Da biste otvorili centar za sigurnost & usklađenosti, otvorite [https://protection.office.com](https://protection.office.com/) . Da biste izravno otvorili stranicu karantene, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Možete pretraživati po sljedećim vrijednostima:  

- **ID poruke**: globalno jedinstveni identifikator poruke. Ako odaberete poruku na popisu, prikazat će se vrijednost  **ID**  -a poruke u oknu s  **detaljima**  koje će se prikazati. Administratori mogu koristiti [Praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i odgovarajuće ID-ove poruka.
- **Adresa e-pošte pošiljatelja**: adresa e-pošte jednog pošiljatelja.
- **Adresa e-pošte primatelja**: adresa e-pošte jednog primatelja.
- **Predmet**: koristite cijeli predmet poruke. Pretraživanje ne razlikuje velika i mala slova.

Nakon što unesete kriterij pretraživanja, kliknite Osvježi ![ gumb Osvježi ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** da biste filtrirali rezultate.  

Cmdleti koje koristite za prikaz i upravljanje porukama i datotekama u karanteni su:
- [Brisanje-poruka u karanteni](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz-poruka u karanteni](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Poruka o karanteni](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Pretpregled – poruka karantene](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na čemu da je ovaj cmdlet namijenjen samo porukama, a ne i zlonamjernim datotekama sa servisa ATP za SharePoint Online, OneDrive za tvrtke ili timove.
- [Release-poruka u karanteni](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)