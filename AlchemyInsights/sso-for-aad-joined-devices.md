---
title: Single-Sign za pridružene uređaje servisa Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404361"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Jednostruka prijava za uređaje pridružene servisu Azure Active Directory

Ako imate lokalno okruženje servisa Active Directory (AD) i želite se pridružiti računalima pridruženima AD domeni servisu Azure AD, to možete postići hibridnim pridruživanjem servisa Azure AD. [Upute: planiranje hibridne implementacije pridruživanja servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) nudi vam povezane korake za implementaciju hibridnog pridruživanja servisa Azure AD u okruženju.

[Konfiguriranje uređaja pridruženih servisu Azure AD za lokalne Single-Sign u sustavu Windows Hello za tvrtke](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemi s tokenom primarnog osvježavanja (PRT)** Primarni token za osvježavanje (PRT) ključan je element provjere autentičnosti servisa Azure AD na uređajima sa sustavom Windows 10, Windows Server 2016 i novijim verzijama, uređajima sa sustavom iOS i Android. To je JSON web-token (JWT) koji je posebno izdan Microsoftovim tokenima za tokene prve strane da bi omogućio jedinstvenu prijavu (SSO) u aplikacijama koje se koriste na tim uređajima. [U aplikaciji Što je token](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)primarnog osvježavanja? na uređajima sa sustavom Windows 10 na uređajima sa sustavom Windows 10 pronaći ćemo pojedinosti o tome kako se izdaje, koristi i štiti PRT.

**WamDefaultSet: DA i AzureADPrt: DA** Ta polja označavaju je li korisnik uspješno provjerio autentičnost servisa Azure AD prilikom prijave na uređaj. Ako su vrijednosti **NO**, može biti potrebno:

- Loš ključ za pohranu u TPM-u povezanom s uređajem nakon registracije (provjerite KeySignTest dok je pokrenuta povišena razina).
- Zamjenski ID za prijavu
- HTTP proxy nije pronađen

Otklanjanje poteškoća s uređajima pomoću naredbe dsregcmd – [stanje SSO-a](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
