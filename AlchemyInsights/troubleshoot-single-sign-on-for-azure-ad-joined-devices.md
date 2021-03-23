---
title: Otklanjanje poteškoća s jednom prijavom za uređaje koji se spajaju na Azure AD
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035105"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Otklanjanje poteškoća s jednom prijavom za uređaje koji se spajaju na Azure AD

Ako imate lokalno okruženje servisa Active Directory (AD) i želite se uključiti u svoju oglasnu domenu u sustavu Azure AD, to možete postići pomoću hibridnih Azure AD Join. [Kako: planirati svoj hibridni Azure Active Directory implementacija](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) servisa nudi vam odgovarajuće korake za implementaciju hibridnog Azure ad Join u vašem okruženju.

Dodatne informacije potražite u članku [Konfiguriranje dodatka Azure ad pridruženi uređaji za lokalne Single-Sign na servisu Windows Hello za tvrtke](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Problemi s primarnim Osvježavanjem (PRT)**

Primarni token za osvježavanje (PRT) ključan je artefakt za provjeru autentičnosti Azure AD u sustavima Windows 10, Windows Server 2016 i novije verzije, iOS i android uređaji. To je web-token za JSON (JWT) koji se posebno izdaje Microsoftovoj prvoj stranci token za tokene da bi omogućio jedinstvenu prijavu (SSO) u svim aplikacijama koje se koriste na tim uređajima. Pojedinosti o tome kako se PRT izdaje, koristi i štiti na uređajima sa sustavom Windows 10 potražite [u članku što je primarni token osvježavanja?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: da i AzureADPrt: da**

Ova polja ukazuju na to je li korisnik uspješno ovjerio Azure AD prilikom prijave na uređaj. Ako vrijednosti **nisu, možda** je posljedica:

- Loš ključ za pohranu u TPM-u povezan s uređajem pri registriranju (provjera tabulatora prilikom izvođenja povišenog)
- Zamjenski ID za prijavu
- HTTP proxy nije pronađen

Otklanjanje poteškoća s uređajima pomoću naredbe dsregcmd potražite u članku [SSO State](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
