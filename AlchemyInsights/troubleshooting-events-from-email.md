---
title: Otklanjanje poteškoća s događajima iz e-pošte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568941"
---
# <a name="troubleshooting-events-from-email"></a>Otklanjanje poteškoća s događajima iz e-pošte

1. Provjerite je li značajka omogućena za poštanski sandučić: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Zatim pogledajte 'Događaji iz e-pošte' trupaca **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. U zapisnicima "Događaji iz e-pošte" pronađite InternetMessageId koji odgovara stavci u poštanskom sandučiću.  

4. TrustScore određuje je li stavka dodana ili ne. Događaji će se dodati samo ako trustscore = "Pouzdano".

TrustScore je određen SPF, Dkim ili Dmarc svojstvima, koja se nalaze u zaglavlju poruke.

Da biste pregledali ova svojstva:

**Outlook za radnu površinu**

- Otvaranje stavke
- File -> Properties -> Internet Headers

Ili

**MFCMapi (U**

- Navigacija do stavke u pristigloj pošti
- Potražite PR_TRANSPORT_MESSAGE_HEADERS_W

Ta se svojstva određuju i bilježe tijekom prijevoza i usmjeravanja. Za daljnje otklanjanje poteškoća, možda ćete morati pratiti uz podršku za promet o kvarovima u SPF, DKIM i.ili DMARC.