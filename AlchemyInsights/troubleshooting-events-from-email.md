---
title: Otklanjanje poteškoća s događajima iz poruke e-pošte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105344"
---
# <a name="troubleshooting-events-from-email"></a>Otklanjanje poteškoća s događajima iz poruke e-pošte

1. Provjera je li značajka omogućena za poštanski sandučić: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Zatim pogledajte zapisnike "Događaji iz **e-pošte" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. U zapisnicima "Događaji iz e-pošte" pronađite InternetMessageId koji odgovara stavci u poštanskom sandučiću.  

4. TrustScore određuje je li stavka dodana ili nije. Događaji će se dodati samo ako je TrustScore = "Pouzdano".

TrustScore određuje SPF, Dkim ili Dmarc svojstva koja se nalaze u zaglavlju poruke.

Da biste pogledali ova svojstva:

**Radna površina Outlook**

- Otvaranje stavke
- Svojstva datoteka -> -> Internet Headers

ili

**MFCMapi**

- Prelazak na stavku u ulaznoj pošti
- Potražite PR_TRANSPORT_MESSAGE_HEADERS_W

Ta se svojstva određuju i bilježe tijekom prijenosa i usmjeravanja. Da biste dodatno otkloniti poteškoće, možda ćete morati nastaviti s podrškom za transport o pogreškama u SPF-u, DKIM-u i.ili DMARC-u.