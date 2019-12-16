---
title: E-pošta tijeka rada se ne šalje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049365"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta tijeka rada ne šalje se za SharePointov popis ili biblioteku

1. E-pošta iz tijekova rada ne šalju se svim korisnicima ili samo određenim korisnicima ili vidite pogrešku **koju poruka e-pošte ne može poslati. Provjerite ima li e-pošta valjanog primatelja**.

    Provjerite postoji li korisnik u grupi dozvola za **sve osobe** (popis korisničkih informacija) za tu zbirku web-mjesta.  Primjer Direct URL: https://<tenant>. sharepoint.com/sites/<sitename>/_layouts/15/. aspx? MembershipGroupId = 0

    - Ako korisnik ne postoji, provjerite je li korisnik potpisan na stranicu. 
    - Ako je to vanjski korisnik, provjerite je li njihova pozivnica prihvaćena.
    - Ako korisnik postoji u grupi dozvola, provjerite je li adresa e-pošte točna.
    - Ako adresa e-pošte korisnika nije postavljena ovdje, zatim stvorite upozorenje uzorka za tog korisnika koji tjera sinkronizaciju tog korisničkog računa iz korisničkih profila sustava SharePoint u ovu zbirku web-mjesta.
 
2. E-pošta iz tijekova rada šalju se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i vidjeti pogrešku **http zabranjeno <span>https:</span>, url/_vti_bin/Client.XVC.SP.Utilities.Utility.sendemail**.
 

    Pogledajte [pristup odbijen prilikom slanja e-pošte u SharePoint grupu](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Također provjerite nije li aktivna značajka prikupljanja **dopuštenja za korisnike ograničenog pristupa** .


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvori tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


