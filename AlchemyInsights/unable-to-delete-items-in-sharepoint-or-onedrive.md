---
title: Nije moguće izbrisati stavke u SharePoint ili OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558645"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

Imate li problema brisanje stavki SharePoint?

- Uvijek provjerite imate li [odgovarajuće dozvole](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) za brisanje artikla ili ste [administrator zbirke web-mjesta](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) pokušaj ukloniti stavku.

- Provjerite postoji li nije postavljanje [pravila zadržavanja](https://docs.microsoft.com/office365/securitycompliance/retention-policies) na stavku.

- Provjerite je li stavka nije [odjavljen](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.

- Konačno, administratori mogu koristiti [SharePoint uzorke i postupci](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koji sadrži biblioteku PowerShell naredbe koje dopuštaju izvođenje složenih upravljanja akcije kao što su prisilno brisanje stubborn stavki.
- [Uklanjanje PNP datoteke](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Uklanjanje PNP mape](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ukloni stavku PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Uklanjanje PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ukloni PNP polje (stupac)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)