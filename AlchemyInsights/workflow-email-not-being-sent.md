---
title: E-pošta tijeka rada nije poslana
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766125"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta tijeka rada ne šalje se na popis ili biblioteku sustava SharePoint

1. E-pošta iz tijekova rada ne šalje se svim korisnicima ili samo određenim korisnicima ili vidite pogrešku **Poruka e-pošte ne može se poslati. Provjerite ima li e-pošta valjanog primatelja**.

    Provjerite postoji li korisnik u grupi **Dozvole za sve osobe** (popis korisničkih informacija) za tu zbirku web-mjesta.  Uzorak izravnog URL-a: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0

    - Ako korisnik ne postoji, provjerite je li korisnik prijavljen na stranicu. 
    - Ako je to vanjski korisnik, provjerite je li prihvaćena njihova pozivnica.
    - Ako korisnik postoji u grupi dozvola, provjerite je li adresa e-pošte ispravna.
    - Ako adresa e-pošte korisnika nije postavljena ovdje, stvorite ogledno upozorenje za tog korisnika koje prisiljava sinkronizaciju tog korisničkog računa iz korisničkih profila sustava SharePoint s ovom zbirkom web-mjesta.
 
2. E-pošta iz tijekova rada šalje se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i vidjeti **pogrešku HTTP Zabranjeno <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Pogledajte [Pristup odbijen prilikom slanja e-pošte sharepoint grupi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Provjerite i nije li aktivna značajka prikupljanja dozvola **za zaključavanje korisničkih dozvola s ograničenim pristupom.**


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvori tijek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


