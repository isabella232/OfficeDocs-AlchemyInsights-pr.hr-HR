---
title: MC210173 – obustava značajke za stvaranje novog prilagođenog obrasca u programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: a53b8885a877cb688cfb42bb4f9108cb2cef2418
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743745"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – obustava značajke za stvaranje novog prilagođenog obrasca u programu SharePoint Designer

Otkrili smo problem koji utječe na funkcionalnost programa SharePoint Designer za [stvaranje prilagođenih obrazaca](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) u usluzi SharePoint Online. Nakon pažljivog razmatranja, utvrdili smo da ne postoji nijedno poznato rješenje tog problema te smo stoga odlučili da onemogućimo značajku za stvaranje prilagođenih obrazaca. Značajka je prestala biti dostupna u 3:00 (UTC) u subotu, 25. travnja 2020. Ta promjena ne utječe na mogućnost uređivanja prethodno stvorenih obrazaca ili drugih postojećih značajki u programu SharePoint Online Designer.

Nakon što je promjena stupila na snagu, korisnici su mogli dobiti pogrešku: „Spremanje promjena popisa na poslužitelju nije uspjelo“ prilikom stvaranja novih obrazaca.

Korisnici koji su prethodno iskoristili mogućnost programa SharePoint Designer za stvaranje prilagođenih obrazaca od sada u tu svrhu mogu koristiti [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).

PowerApps je jednostavan i moćan alat koji korisnicima modernog sučelja usluge SharePoint Online omogućuje stvaranje i uređivanje prilagođenih obrazaca za popise programa SharePoint i biblioteke dokumenata izravno u prozoru preglednika. PowerApps ne zahtijeva tradicionalno znanje kodiranja ni dodatna preuzimanja aplikacija, kao što je InfoPath.

**Napomena**: korisnici klasičnog sučelja usluge SharePoint Online moraju privremeno prijeći na moderno sučelje kako bi pristupali aplikacijama PowerApps i koristili ih. Međutim, svi prilagođeni obrasci stvoreni u aplikaciji PowerApps dostupni su korisnicima klasičnog sučelja usluge SharePoint Online.
