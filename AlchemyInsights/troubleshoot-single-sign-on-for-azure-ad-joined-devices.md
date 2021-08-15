---
title: Otklanjanje poteškoća s jedinstvenom prijavom za uređaje pridružene servisu Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039238"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Otklanjanje poteškoća s jedinstvenom prijavom za uređaje pridružene servisu Azure AD

Ako imate lokalno okruženje servisa Active Directory (AD) i želite se pridružiti računalima pridruženima AD domeni servisu Azure AD, to možete postići hibridnim pridruživanjem servisa Azure AD. [Upute: planiranje hibridne implementacije Azure Active Directory pridruživanja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) nudi vam povezane korake za implementaciju hibridnog pridruživanja servisa Azure AD u vašem okruženju.

Dodatne informacije potražite u članku [Konfiguriranje uređaja pridruženih servisu Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)za lokalne Single-Sign u sustavu Windows Hello za tvrtke .

**Problemi s tokenom primarnog osvježavanja (PRT)**

Primarni token za osvježavanje (PRT) ključan je element provjere autentičnosti servisa Azure AD na uređajima sa sustavom Windows 10, Windows Server 2016 i novijim verzijama, uređajima sa sustavom iOS i Android. To je JSON web-token (JWT) koji je posebno izdan Microsoftovim tokenima za tokene prve strane da bi omogućio jedinstvenu prijavu (SSO) u aplikacijama koje se koriste na tim uređajima. Detalje o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima potražite [u članku Što je token primarnog osvježavanja?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: DA i AzureADPrt: DA**

Ta polja označavaju je li korisnik uspješno provjerio autentičnost servisa Azure AD prilikom prijave na uređaj. Ako su vrijednosti **NO**, to može biti zbog:

- Loš ključ za pohranu u TPM-u povezanom s uređajem nakon registracije (provjerite KeySignTest tijekom povišenog pokretanja)
- Zamjenski ID za prijavu
- HTTP proxy nije pronađen

Da biste otklonili poteškoće s uređajima pomoću naredbe dsregcmd, pogledajte [SSO stanje](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
