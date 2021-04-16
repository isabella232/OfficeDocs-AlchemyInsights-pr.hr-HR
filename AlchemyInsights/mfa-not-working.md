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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810476"
---
# <a name="issues-with-azure-mfa"></a>Problemi sa servisom Azure MFA
Nekoliko je stvari koje je moguće provjeriti ne mogu li se korisnici prijaviti pomoću višestruke provjere autentičnosti (MFA)

1. Zahvaćeni korisnik može biti blokiran na portalu Azure Active Directory. Ako je tako, pokušaji provjere autentičnosti za tog određenog korisnika bit će automatski odbijeni. [Slijedite korake u ovom članku da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako deblokiranje korisnika nije pomoglo ili korisnik nije blokiran, možete pokušati ponovno postaviti MFA za korisnika i on će ponovno proći kroz postupak registracije. [Slijedite korake u ovom članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako je ovo prvi put da ste omogućili MFA i korisnici se ne mogu prijaviti na klijente koji nisu preglednici, kao što su Outlook, Skype itd., možda ADAL (Biblioteka provjere autentičnosti servisa Active Directory) nije omogućen u sklopu pretplate na O365. U tom ćete se slučaju morati povezati sa ljuskom Exchange Online Powershell i pokrenuti ovaj cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*