---
title: Problemi s MFA-om
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098594"
---
# <a name="issues-with-azure-mfa"></a>Problemi sa servisom Azure MFA
Nekoliko je stvari koje je moguće provjeriti ne mogu li se korisnici prijaviti pomoću višestruke provjere autentičnosti (MFA)

1. Zahvaćeni korisnik može biti blokiran na Azure Active Directory portalu. Ako je tako, pokušaji provjere autentičnosti za tog određenog korisnika bit će automatski odbijeni. [Slijedite korake u ovom članku da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako deblokiranje korisnika nije pomoglo ili korisnik nije blokiran, možete pokušati ponovno postaviti MFA za korisnika i on će ponovno proći kroz postupak registracije. [Slijedite korake u ovom članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako ste prvi put omogućili MFA i korisnici se ne mogu prijaviti na klijente koji nisu preglednici, kao što su Outlook, Skype itd., možda ADAL (Biblioteka provjere autentičnosti servisa Active Directory) nije omogućen u sklopu pretplate na O365. U tom ćete se slučaju morati povezati s Exchange Online Powershell i pokrenuti ovaj cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*