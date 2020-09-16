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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="756ef-102">Problemi s programom Azure MFA</span><span class="sxs-lookup"><span data-stu-id="756ef-102">Issues with Azure MFA</span></span>
<span data-ttu-id="756ef-103">Ako se korisnici ne mogu prijaviti pomoću višečimbenika provjere autentičnosti (MFA), možete provjeriti nekoliko stavki.</span><span class="sxs-lookup"><span data-stu-id="756ef-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="756ef-104">Pogođeni korisnik može biti blokiran u portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="756ef-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="756ef-105">Ako je to slučaj, pokušaji provjere autentičnosti tog određenog korisnika automatski će se odbiti.</span><span class="sxs-lookup"><span data-stu-id="756ef-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="756ef-106">Slijedite korake u ovom članku da biste ih deblokirali.</span><span class="sxs-lookup"><span data-stu-id="756ef-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="756ef-107">Ako vam deblokiranje korisnika nije pomoglo ili korisnik nije blokiran, možete pokušati ponovno postaviti MFA za korisnika, a oni će ponovno proći kroz postupak prijave.</span><span class="sxs-lookup"><span data-stu-id="756ef-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="756ef-108">Slijedite korake u ovom članku.</span><span class="sxs-lookup"><span data-stu-id="756ef-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="756ef-109">Ako je ovo prvi put da ste omogućili MFA i korisnici se ne mogu prijaviti na klijente koji nisu preglednici, kao što su Outlook, Skype i sl., možda ADAL (biblioteka za provjeru autentičnosti Active Directory) nije omogućena na pretplatnoj O365.</span><span class="sxs-lookup"><span data-stu-id="756ef-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="756ef-110">U ovom slučaju morat ćete se povezati s komponenti Exchange Online PowerShell i pokrenuti ovaj cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="756ef-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>