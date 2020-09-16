---
title: Oznake osjetljivosti se ne prikazuju
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801176"
---
# <a name="sensitivity-labels-not-appearing"></a>Oznake osjetljivosti se ne prikazuju

Oznake osjetljivosti omogućuju vam klasificiranje i zaštita osjetljivog sadržaja. Mogu se stvoriti u centru za usklađenost sustava Microsoft 365, Microsoft 365 Security Center ili Microsoft 365 Security & centar za usklađenost u odjeljku klasifikacija > oznake osjetljivosti. Dodatne informacije o toj značajci potražite u članku [Pregled naljepnica s osjetljivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ako ste konfigurirali naljepnice osjetljivosti, ali se ne prikazuju u aplikacijama Microsoft 365, provjerite sljedeće:

- Provjerite je li natpis osjetljivosti [objavljen](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) korisnicima i grupama koje želite.

- Potvrdite da korisnik koristi aplikaciju koja podržava naljepnice s osjetljivosti – pogledajte [natpise osjetljivosti u dokumentu](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Ako [migrirate oznake zaštite informacija o Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), budite svjesni razmatranja navedenih [ovdje](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Podrška za prevencija gubitka podataka (DLP): trenutno se samo oznake zadržavanja mogu koristiti kao uvjet u pravilima programa DLP.  Podrška za naljepnice osjetljivosti u pravilima programa DLP još nije dostupna, ali radimo na tome.

- Kada je omogućeno šifriranje na naljepnici osjetljivosti, možete odabrati sljedeće:
    - Dodjela dozvola odmah
    - Dopusti korisnicima dodjeljivanje dozvola


Dodatne informacije o mogućim pitanjima potražite u članku [poznati problemi s naljepnicama osjetljivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).