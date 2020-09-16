---
title: Otklanjanje poteškoća s e-poštom
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658726"
---
# <a name="troubleshooting-events-from-email"></a>Otklanjanje poteškoća s e-poštom

1. Provjera je li značajka omogućena za poštanski sandučić: **dohvaćanje-EventsFromEmailConfiguration – Identity <mailbox> **

2. Zatim pogledajte "događaji iz poruka e-pošte" **Export-Mailboxdijagnostički zapisnici <mailbox> -komponenta timeprofile**

3. U zapisnicima "događaji iz e-pošte" Pronađite aplikaciju InternetMessageId koja odgovara stavci u poštanskom sandučiću.  

4. Rezultat pouzdanosti određuje je li stavka dodana ili nije. Događaji će se dodati samo ako je TrustScore = "pouzdan".

Funkcija TrustScore određuje se pomoću funkcija SPF, depet ili DeMarka, koje se nalaze u zaglavlju poruke.

Da biste pogledali ta svojstva, učinite sljedeće:

**Outlook za stolna računala**

- Otvaranje stavke
- Svojstva datoteka->-> Internetska zaglavlja

ili

**MFCMapi**

- Navigacija do stavke u ulaznoj pošti
- Potražite PR_TRANSPORT_MESSAGE_HEADERS_W

Ta se svojstva određuju i snimaju tijekom transporta i proizvodnog postupka. Da biste dodatno otklanjanja poteškoća, možda ćete morati pratiti podršku za transport o neuspjehom u programu SPF, DKIM i. ili DMARC.