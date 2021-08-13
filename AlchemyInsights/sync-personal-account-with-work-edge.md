---
title: Omogućivanje sinkronizacije osobnog računa s poslovnim računom u programu Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813390"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Omogućivanje sinkronizacije osobnog računa s poslovnim računom u programu Microsoft Edge

Provjerite ispunjavate li sljedeće kriterije:

- Enterprise State Roaming omogućen je u centru Azure Active Directory za administratore, što zahtijeva pretplatu na Azure Active Directory premium ili Enterprise Mobility + Security (EMS). Dodatne informacije potražite u članku [Omogućivanje roaminga u sustavu Enterprise State u sustavu Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- Ispunjen je jedan ili oba sljedeća kriterija:
    - Servis Azure Information Protection omogućen je za vaš klijent. Detalje potražite u članku [Aktivacija zaštite upravljanja pravima na Azure Centar za administratore okruženja Microsoft 365](/azure/information-protection/activate-office365).
    - Značajka Azure Active Directory enterprise state roaming (ESR) omogućena je za bilo kojeg korisnika ili klijenta. Dodatne informacije potražite u članku [Što je roaming u poslovnom stanju?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Ako su AIP i ESR onemogućeni, poruka o pogrešci obavještava korisnike da sinkronizacija nije dostupna za njihove račune.
