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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545149"
---
# <a name="issues-with-mfa"></a>Problemi s MFA
Postoji nekoliko stvari koje je moguće provjeriti ako se korisnici ne mogu prijaviti pomoću višefaktorske provjere autentičnosti (MFP)

1. Zahvaćeni korisnik može biti blokiran na portalu Azure Active Directory. Ako je to slučaj, pokušaji provjere autentičnosti za tog određenog korisnika automatski će se uskratiti. [Slijedite korake u ovom članku da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako deblokiranje korisnika nije pomoglo ili korisnik nije blokiran možete pokušati resetirati MFA za korisnika i oni će opet proći kroz postupak upisa. [Slijedite korake u ovom članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako je ovo prvi put da ste omogućili MFA i vaši korisnici se ne mogu prijaviti na klijente koji nisu preglednici kao što su Outlook, Skype, itd, možda ADAL (biblioteka autentičnosti Active Directory) nije omogućena na vašoj O365 pretplate. U tom slučaju morat ćete se spojiti na Exchange Online PowerShell i pokrenuti ovaj cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*