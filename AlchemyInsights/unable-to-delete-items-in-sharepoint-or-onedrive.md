---
title: Brisanje stavki u sustavu SharePoint ili na servisu OneDrive nije moguće
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019575"
---
# <a name="unable-to-delete-items"></a>Brisanje stavki nije moguće

- Pravila zadržavanja mogu izazvati to, morate onemogućiti ili isključiti odgovarajuće zadržavanje koje uzrokuje taj problem. Nakon uklanjanja pravilnika o zadržavanju ili zadržavanja, može potrajati i do 24 sata da bi promjena stupila na pamet. Provjerite ne postoji li postavljanje [pravilnika o zadržavanju](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) na stavci.

- Web-mjesto je moglo premašiti ograničenje prostora za pohranu, povećati [kvotu web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisati stavku.

- Provjerite nije li stavka [odjavljena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.

- Na kraju administratori mogu koristiti [obrasce i prakse sustava SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koji sadrže biblioteku programa PowerShell koje omogućuju obavljanje složenih akcija upravljanja, kao što je prisilno brisanje tvrdoglavih stavki.
- [Uklanjanje PNP datoteke](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Uklanjanje mape PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Uklanjanje stavke PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Uklanjanje PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Uklanjanje PNP polja (stupca)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)