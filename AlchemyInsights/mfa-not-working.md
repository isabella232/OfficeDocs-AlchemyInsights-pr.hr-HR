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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768829"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="1858d-102">Problemi s uslugom Azure MFA</span><span class="sxs-lookup"><span data-stu-id="1858d-102">Issues with Azure MFA</span></span>
<span data-ttu-id="1858d-103">Postoji nekoliko stvari koje je moguće provjeriti ako se korisnici ne mogu prijaviti pomoću višefaktorske provjere autentičnosti (MFP)</span><span class="sxs-lookup"><span data-stu-id="1858d-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="1858d-104">Zahvaćeni korisnik može biti blokiran na portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1858d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="1858d-105">Ako je to slučaj, pokušaji provjere autentičnosti za tog određenog korisnika automatski će se uskratiti.</span><span class="sxs-lookup"><span data-stu-id="1858d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="1858d-106">Slijedite korake u ovom članku da biste ih deblokirali.</span><span class="sxs-lookup"><span data-stu-id="1858d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="1858d-107">Ako deblokiranje korisnika nije pomoglo ili korisnik nije blokiran možete pokušati resetirati MFA za korisnika i oni će opet proći kroz postupak upisa.</span><span class="sxs-lookup"><span data-stu-id="1858d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="1858d-108">Slijedite korake u ovom članku.</span><span class="sxs-lookup"><span data-stu-id="1858d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="1858d-109">Ako je ovo prvi put da ste omogućili MFA i vaši korisnici se ne mogu prijaviti na klijente koji nisu preglednici kao što su Outlook, Skype, itd, možda ADAL (biblioteka autentičnosti Active Directory) nije omogućena na vašoj O365 pretplate.</span><span class="sxs-lookup"><span data-stu-id="1858d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="1858d-110">U tom slučaju morat ćete se spojiti na Exchange Online PowerShell i pokrenuti ovaj cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="1858d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>