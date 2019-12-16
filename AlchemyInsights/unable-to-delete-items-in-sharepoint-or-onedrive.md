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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049509"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

Imate problema s brisanjem SharePoint stavki?

- Uvijek provjerite imate li [odgovarajuće dozvole](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) za brisanje stavke ili ako [administrator zbirke web-mjesta](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) pokuša ukloniti stavku.

- Osigurajte da na artiklu nema postavljanja [pravila zadržavanja](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

- Osigurajte da artikl nije [odjavljen](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.

- Na kraju, administratori mogu koristiti [SharePoint obrasci i prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koji sadrže biblioteku PowerShell naredbi koje vam omogućuju izvođenje složenih upravljanja akcije kao što su prisilno brisanje tvrdokornih stavki.
- [Ukloni PNP datoteku](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Ukloni PNP mapu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Ukloni stavku PNP popisa](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ukloni PNP popis](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Ukloni PNP polje (stupac)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)