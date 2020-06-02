---
title: Nije moguće izbrisati stavke u sustavu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511968"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

Pravila zadržavanja mogu uzrokovati to, morate onemogućiti ili isključiti odgovarajuće zadržavanje koje uzrokuje taj problem. Nakon uklanjanja pravila zadržavanja ili zadržavanja može biti potrebno do 24 sata da promjena stupi na snagu. Provjerite ne postoji postavljanje [pravila zadržavanja](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) na stavci.

Web-mjesto je možda premašilo ograničenje pohrane, povećalo [kvotu web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisalo stavku.

Provjerite nije li stavka [odjavljena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.

Naposljetku, administratori mogu koristiti [obrasce i prakse sustava SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koja sadrži biblioteku powershell naredbi koje vam omogućuju izvođenje složenih akcija upravljanja kao što je prisilno brisanje tvrdoglavih stavki.
- [Ukloni PNP datoteku](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ukloni PNP mapu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ukloni stavku PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ukloni PNP popis](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ukloni PNP polje (stupac)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)