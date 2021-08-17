---
title: Single-Sign za Azure Active Directory spojene uređaje
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050002"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Jedinstvena prijava za spojene Azure Active Directory uređaje

Ako imate lokalno okruženje servisa Active Directory (AD) i želite se pridružiti računalima pridruženima AD domeni servisu Azure AD, to možete postići hibridnim pridruživanjem servisa Azure AD. [Upute: planiranje hibridne implementacije Azure Active Directory pridruživanja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) nudi vam povezane korake za implementaciju hibridnog pridruživanja servisa Azure AD u vašem okruženju.

[Konfiguriranje uređaja pridruženih servisu Azure AD za lokalne Single-Sign Na Windows Hello za tvrtke](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemi s tokenom primarnog osvježavanja (PRT)** Primarni token za osvježavanje (PRT) ključan je element provjere autentičnosti servisa Azure AD na uređajima sa sustavom Windows 10, Windows Server 2016 i novijim verzijama, uređajima sa sustavom iOS i Android. To je JSON web-token (JWT) koji je posebno izdan Microsoftovim tokenima za tokene prve strane da bi omogućio jedinstvenu prijavu (SSO) u aplikacijama koje se koriste na tim uređajima. [U programu Što je token primarnog osvježavanja?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)na uređajima ćemo navesti pojedinosti o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima.

**WamDefaultSet: DA i AzureADPrt: DA** Ta polja označavaju je li korisnik uspješno provjerio autentičnost servisa Azure AD prilikom prijave na uređaj. Ako su vrijednosti **NO**, može biti potrebno:

- Loš ključ za pohranu u TPM-u povezanom s uređajem nakon registracije (provjerite KeySignTest dok je pokrenuta povišena razina).
- Zamjenski ID za prijavu
- HTTP proxy nije pronađen

Otklanjanje poteškoća s uređajima pomoću naredbe dsregcmd – [stanje SSO-a](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
