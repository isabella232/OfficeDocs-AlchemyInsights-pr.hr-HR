---
title: Tijek rada e-pošta se šalje
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270664"
---
# <a name="workflow-email-is-not-being-sent"></a>Tijek rada e-pošta se šalje

1. E-pošta s tijekovima rada se šalju sve korisnike ili samo određenim korisnicima ili vidjeti pogreške **poruku e-pošte nije moguće poslati. Provjerite je li e-pošta ima valjan primatelj**.

    Provjerite je li korisnik postoji u grupi dozvole **Sve osobe** (Popis korisničkih informacija) za tu zbirku web-mjesta.  Ogledni direktni URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Ako korisnik ne postoji, provjerite je li korisnik potpisano u stranicu. 
    - Ako je vanjskog korisnika, provjerite njihove poziv je prihvaćen.
    - Ako korisnik ne postoji u grupi dozvole, provjerite je li adresa e-pošte točna.
    - Ako adresa e-pošte korisnicima ne Ovdje postavite, stvoriti primjerak upozorenja za tog korisnika koje navodi sinkronizaciju taj korisnički račun iz korisnički profili SharePoint zbirke web-mjesta.
 
2. E-pošta iz tijekova rada se šalju administratori zbirke web-mjesta, ali ne i drugim korisnicima i vidjeti pogrešku **HTTP zabranjeno za <spam> <spam> ** <spam> <spam>.
 

    Pogledajte [Pristup odbijen kada grupira poslane e-pošte](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Također, provjerite je li značajka zbirke web-mjesta **način rada lockdown dozvole Ograničeni pristup korisnika** nije aktivan.


## <a name="related-topics"></a>Povezane teme
Želite li pokušajte Microsoft Flow u SharePoint Online?
- [Stvaranje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i tijek](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


