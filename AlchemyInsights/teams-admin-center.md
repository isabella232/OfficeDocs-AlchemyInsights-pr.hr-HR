---
title: Centar za administratore aplikacije Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354080"
---
# <a name="teams-admin-center"></a>Centar za administratore aplikacije Teams

Saznajte više o upravljanju aplikacijom Teams pomoću [centra za administratore aplikacije Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ako ne možete pristupiti centru za administratore aplikacije Teams, provjerite sljedeće stavke:

- Provjerite jeste li dopustili odgovarajuće [IP adrese i URL-ove sustava Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na svim uređajima na vanjskoj crti obrane (vatrozidu itd.) ili u pravilima vatrozida na lokalnom računalu.
- Provjerite odgovaraju li podaci za prijavu koje koristite za pristup portalu za administratore aplikacije Teams vašem korisničkom imenu na [portalu za administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ako se u centru za administratore aplikacije Teams ne prikazuju korisnici, provjerite sljedeće:

- Jeste li tijekom zadnja 24 sata stvarali korisnike ili dodjeljivali licence? Pričekajte barem 24 sata prije nego što prijavite problem službi za podršku.
- Provjerite jeste li dodijelili odgovarajuće licence?
- Ako imate lokalni Active Directory, provjerite je li [vrijednost msRTCSIP-PrimaryUserAddress ili SIP adrese u polju ProxyAddresses u lokalnom servisu Active Directory jedinstvena, a oblik odgovara](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip: Korisničko**ime** korisnika iz [centra za administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ako namjeravate zadržati implementaciju servisa Skype za poslovne poslužitelje i korisnicima koji su lokalno i na mreži: slijedite **"Postavljanje hibridnog sustava sa servisima i skypeom za tvrtke online"** na upravljačkoj ploči servisa Skype za poslovne poslužitelje i premjestite korisnike na mreži.
