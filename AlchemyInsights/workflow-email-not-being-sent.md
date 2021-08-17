---
title: E-pošta tijeka rada ne šalje se
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072512"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta tijeka rada ne šalje se za SharePoint ili biblioteku

1. E-pošta iz tijekova rada ne šalje se svim korisnicima ili samo određenim korisnicima ili se prikazuje pogreška Poruka e-pošte nije moguće poslati. Provjerite ima li **poruka e-pošte valjanog primatelja**.

    Provjerite postoji li korisnik u grupi dozvola **Sve osobe** (popis korisničkih podataka) za tu zbirku web-mjesta.  Ogledni izravni URL: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Ako korisnik ne postoji, provjerite je li korisnik prijavljen na stranicu. 
    - Ako je vanjski korisnik, provjerite je li pozivnica prihvaćena.
    - Ako korisnik postoji u grupi dozvola, provjerite je li adresa e-pošte točna.
    - Ako adresa e-pošte korisnika nije ovdje postavljena, stvorite ogledno upozorenje za tog korisnika koje prisiljava sinkronizaciju tog korisničkog računa iz korisničkih profila SharePoint ovoj zbirci web-mjesta.
 
2. E-pošta iz tijekova rada šalje se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i prikazuje se pogreška **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Pogledajte [access denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Provjerite i nije li značajka **zaključavanja web-mjesta s korisničkim** dozvolama s ograničenim pristupom aktivna.


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow SharePoint online?
- [Stvaranje Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


