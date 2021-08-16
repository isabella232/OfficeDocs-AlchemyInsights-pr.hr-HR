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
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049336"
---
# <a name="teams-admin-center"></a>Centar za administratore aplikacije Teams

Saznajte više o upravljanju aplikacijom Teams pomoću [centra za administratore aplikacije Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ako ne možete pristupiti centru za administratore aplikacije Teams, provjerite sljedeće stavke:

- Provjerite jeste li dopustili odgovarajuće [IP adrese i URL-ove sustava Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) na svim uređajima na vanjskoj crti obrane (vatrozidu itd.) ili u pravilima vatrozida na lokalnom računalu.
- Provjerite odgovaraju li podaci za prijavu koje koristite za pristup portalu za administratore aplikacije Teams vašem korisničkom imenu na [portalu za administratore sustava Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ako se u centru za administratore aplikacije Teams ne prikazuju korisnici, provjerite sljedeće:

- Jeste li tijekom zadnja 24 sata stvarali korisnike ili dodjeljivali licence? Pričekajte barem 24 sata prije nego što prijavite problem službi za podršku.
- Provjerite jeste li dodijelili odgovarajuće licence?
- Ako imate lokalni Active Directory, provjerite je li [vrijednost msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) ili SIP adrese u polju ProxyAddresses u lokalnom servisu Active Directory jedinstvena, a oblik odgovara sipu: Korisničko ime [korisnika iz Centar za administratore okruženja Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ako namjeravate održati implementaciju sustava Skype za tvrtke poslužiteljska verzija i korisnicima biti lokalno i na mreži: slijedite "Postavljanje hibridne implementacije **s Teams i Skype za tvrtke Online"** na upravljačkoj ploči Skype za tvrtke poslužiteljska verzija i premjestite korisnike na mreži.
