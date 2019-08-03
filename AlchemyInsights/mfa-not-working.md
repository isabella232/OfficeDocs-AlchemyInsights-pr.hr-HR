---
title: Problemi s MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250157"
---
# <a name="issues-with-mfa"></a>Problemi s MFA
Postoji nekoliko stvari koje treba provjeriti Ako korisnici ne Prijava pomoću višestruku provjeru autentičnosti (MFA)

1. Zahvaćeni korisnik možda blokiran Azure Active Directory portalu. Ako je to slučaj, provjera autentičnosti pokušava za taj određeni korisnik bit će automatski odbijen. [Slijedite korake u ovom članku da biste ih deblokirati.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako niste pomoći deblokiranja korisnika ili korisnik je blokiran pokušajte vratiti MFA za korisnika i oni će proći kroz proces enroll ponovo. [Slijedite korake u ovom članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako je ovo prvi put MFA omogućen i korisnici se ne prijava-preglednici klijentima za Outlook, servisa Skype itd, možda ADAL (Active Directory provjere autentičnosti biblioteka) nije omogućen na O365 pretplate. U tom slučaju morat ćete se povezati s Exchange Online Powershell i pokretanje tog cmdleta:  *Set OrganizationConfig-OAuth2ClientProfileEnabled: $true*