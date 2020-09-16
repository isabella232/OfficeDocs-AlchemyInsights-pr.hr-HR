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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748981"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta tijeka rada ne šalje se na popis ili biblioteku sustava SharePoint

1. E-pošta iz tijekova rada ne šalje se svim korisnicima ili samo određenim korisnicima ili vam se prikazuje pogreška **poruke e-pošte nije moguće poslati. Provjerite ima li e-pošta valjani primatelj**.

    Provjerite postoji li korisnik u grupi dozvole za **sve osobe** (popis korisničkih informacija) za tu zbirku web-mjesta.  Ogledni Direktni URL: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? Člana Članigrupe = 0

    - Ako korisnik ne postoji, provjerite je li korisnik potpisan na stranicu. 
    - Ako se radi o vanjskom korisniku, provjerite je li pozivnica prihvaćena.
    - Ako korisnik postoji u grupi dozvole, provjerite je li adresa e-pošte točna.
    - Ako adresa e-pošte korisnika nije postavljena ovdje, stvorite ogledno upozorenje za tog korisnika koji prisiljava sinkronizaciju tog korisničkog računa iz korisničkih profila sustava SharePoint na ovu zbirku web-mjesta.
 
2. E-pošta iz tijekova rada šalje se administratorima zbirke web-mjesta, ali ne i drugim korisnicima i prikazuje pogrešku **http zabranjen za <span>https:</span>/_vti_bin/Client.XVC.SP.Utilities.Utility.sendemail**.
 

    Prikaz [odbijanja kada šaljete poruku e-pošte u grupu sustava SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Provjerite i je li funkcija **ograničen pristup korisničkim dozvolama za zaključavanje** web-mjesta aktivna.


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvaranje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


