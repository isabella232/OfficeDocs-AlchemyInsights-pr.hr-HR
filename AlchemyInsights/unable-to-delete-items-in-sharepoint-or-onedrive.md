---
title: Nije moguće izbrisati stavke u sustavu SharePoint ili servisu OneDrive
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571232"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

Pravila zadržavanja mogu to uzrokovati, morate onemogućiti ili isključiti odgovarajuće zadržavanje koje uzrokuje taj problem. Nakon što se pravila zadržavanja ili zadržavanje uklone, može trajati do 24 sata kako bi promjena stupila na snagu. Osigurajte da na artiklu nema postavljanja [pravila zadržavanja](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

Web-mjesto je možda prekoračilo ograničenje pohrane, povećala [kvotu web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisala stavku.

Osigurajte da artikl nije [odjavljen](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.

Na kraju, administratori mogu koristiti [SharePoint obrasci i prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koji sadrže biblioteku PowerShell naredbi koje vam omogućuju izvođenje složenih upravljanja akcije kao što su prisilno brisanje tvrdokornih stavki.
- [Ukloni PNP datoteku](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ukloni PNP mapu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ukloni stavku PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ukloni PNP popis](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ukloni PNP polje (stupac)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)