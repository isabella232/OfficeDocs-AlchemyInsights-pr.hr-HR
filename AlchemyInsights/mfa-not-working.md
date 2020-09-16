---
title: Problemi s programom MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755123"
---
# <a name="issues-with-azure-mfa"></a>Problemi s programom Azure MFA
Ako se korisnici ne mogu prijaviti pomoću višečimbenika provjere autentičnosti (MFA), možete provjeriti nekoliko stavki.

1. Pogođeni korisnik može biti blokiran u portalu Azure Active Directory. Ako je to slučaj, pokušaji provjere autentičnosti tog određenog korisnika automatski će se odbiti. [Slijedite korake u ovom članku da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako vam deblokiranje korisnika nije pomoglo ili korisnik nije blokiran, možete pokušati ponovno postaviti MFA za korisnika, a oni će ponovno proći kroz postupak prijave. [Slijedite korake u ovom članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako je ovo prvi put da ste omogućili MFA i korisnici se ne mogu prijaviti na klijente koji nisu preglednici, kao što su Outlook, Skype i sl., možda ADAL (biblioteka za provjeru autentičnosti Active Directory) nije omogućena na pretplatnoj O365. U ovom slučaju morat ćete se povezati s komponenti Exchange Online PowerShell i pokrenuti ovaj cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*