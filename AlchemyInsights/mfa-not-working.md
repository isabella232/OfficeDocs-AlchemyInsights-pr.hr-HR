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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="887d8-102">Problemi sa servisom Azure MFA</span><span class="sxs-lookup"><span data-stu-id="887d8-102">Issues with Azure MFA</span></span>
<span data-ttu-id="887d8-103">Nekoliko je stvari koje je moguće provjeriti ne mogu li se korisnici prijaviti pomoću višestruke provjere autentičnosti (MFA)</span><span class="sxs-lookup"><span data-stu-id="887d8-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="887d8-104">Zahvaćeni korisnik može biti blokiran na portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="887d8-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="887d8-105">Ako je tako, pokušaji provjere autentičnosti za tog određenog korisnika bit će automatski odbijeni.</span><span class="sxs-lookup"><span data-stu-id="887d8-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="887d8-106">Slijedite korake u ovom članku da biste ih deblokirali.</span><span class="sxs-lookup"><span data-stu-id="887d8-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="887d8-107">Ako deblokiranje korisnika nije pomoglo ili korisnik nije blokiran, možete pokušati ponovno postaviti MFA za korisnika i on će ponovno proći kroz postupak registracije.</span><span class="sxs-lookup"><span data-stu-id="887d8-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="887d8-108">Slijedite korake u ovom članku.</span><span class="sxs-lookup"><span data-stu-id="887d8-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="887d8-109">Ako je ovo prvi put da ste omogućili MFA i korisnici se ne mogu prijaviti na klijente koji nisu preglednici, kao što su Outlook, Skype itd., možda ADAL (Biblioteka provjere autentičnosti servisa Active Directory) nije omogućen u sklopu pretplate na O365.</span><span class="sxs-lookup"><span data-stu-id="887d8-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="887d8-110">U tom ćete se slučaju morati povezati sa ljuskom Exchange Online Powershell i pokrenuti ovaj cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="887d8-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>