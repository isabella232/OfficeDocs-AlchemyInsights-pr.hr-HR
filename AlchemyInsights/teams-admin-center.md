---
title: Centar za administratore aplikacije Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826371"
---
# <a name="teams-admin-center"></a>Centar za administratore aplikacije Teams

Saznajte više o upravljanju aplikacijom Teams pomoću [centra za administratore aplikacije Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ako ne možete pristupiti centru za administratore aplikacije Teams, provjerite sljedeće stavke:

- Provjerite jeste li dopustili odgovarajuće [IP adrese i URL-ove sustava Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na svim uređajima na vanjskoj crti obrane (vatrozidu itd.) ili u pravilima vatrozida na lokalnom računalu.
- Provjerite odgovaraju li podaci za prijavu koje koristite za pristup portalu za administratore aplikacije Teams vašem korisničkom imenu na [portalu za administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ako se u centru za administratore aplikacije Teams ne prikazuju korisnici, provjerite sljedeće:

- Jeste li tijekom zadnja 24 sata stvarali korisnike ili dodjeljivali licence? Pričekajte barem 24 sata prije nego što prijavite problem službi za podršku.
- Provjerite jeste li dodijelili odgovarajuće licence?
- Ako imate lokalni Active Directory, provjerite je li [vrijednost msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ili SIP adrese u polju ProxyAddresses u lokalnom servisu Active Directory jedinstvena, a oblik odgovara sipu: korisničko ime korisnika iz centra za [administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ako namjeravate zadržati implementaciju servisa Skype za tvrtke server i imate kućne korisnike na lokalnoj i mrežnoj mreži: slijedite "Postavljanje hibridne implementacije sa servisom Teams i **Skypeom za tvrtke online"** na upravljačkoj ploči poslužitelja Skypea za tvrtke i premjestite korisnike online.
