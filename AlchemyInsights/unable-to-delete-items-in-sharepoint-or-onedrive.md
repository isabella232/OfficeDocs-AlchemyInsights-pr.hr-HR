---
title: Nije moguće izbrisati stavke u SharePoint ili OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038509"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

- Pravila zadržavanja mogu uzrokovati taj problem, morate onemogućiti ili isključiti odgovarajuće čuvanje koje uzrokuje taj problem. Nakon što se pravilnik o zadržavanju ili čuvanje ukloni, promjena može potrajati do 24 sata. Provjerite ne postoji li postavljanje [pravilnika o zadržavanju](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) na stavci.

- Web-mjesto je možda prekoračilo ograničenje prostora za pohranu, povećalo [kvotu web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisalo stavku.

- Provjerite nije li stavka [odjavljena drugom](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) korisniku.

- Naposljetku, administratori [mogu koristiti SharePoint obrasce](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) i prakse (PnP) koji sadrži biblioteku naredbi komponente PowerShell koje omogućuju izvođenje složenih akcija upravljanja, kao što je prisilno brisanje tvrdokornih stavki.
- [Uklanjanje PNP datoteke](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Uklanjanje PNP mape](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ukloni stavku PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ukloni PNP popis](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Uklanjanje PNP polja (stupca)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)