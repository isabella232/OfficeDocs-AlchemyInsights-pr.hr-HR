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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545149"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="34adc-102">Problemi s MFA</span><span class="sxs-lookup"><span data-stu-id="34adc-102">Issues with MFA</span></span>
<span data-ttu-id="34adc-103">Postoji nekoliko stvari koje treba provjeriti Ako korisnici ne Prijava pomoću višestruku provjeru autentičnosti (MFA)</span><span class="sxs-lookup"><span data-stu-id="34adc-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="34adc-104">Zahvaćeni korisnik možda blokiran Azure Active Directory portalu.</span><span class="sxs-lookup"><span data-stu-id="34adc-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="34adc-105">Ako je to slučaj, provjera autentičnosti pokušava za taj određeni korisnik bit će automatski odbijen.</span><span class="sxs-lookup"><span data-stu-id="34adc-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="34adc-106">Slijedite korake u ovom članku da biste ih deblokirati.</span><span class="sxs-lookup"><span data-stu-id="34adc-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="34adc-107">Ako niste pomoći deblokiranja korisnika ili korisnik je blokiran pokušajte vratiti MFA za korisnika i oni će proći kroz proces enroll ponovo.</span><span class="sxs-lookup"><span data-stu-id="34adc-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="34adc-108">Slijedite korake u ovom članku.</span><span class="sxs-lookup"><span data-stu-id="34adc-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="34adc-109">Ako je ovo prvi put MFA omogućen i korisnici se ne prijava-preglednici klijentima za Outlook, servisa Skype itd, možda ADAL (Active Directory provjere autentičnosti biblioteka) nije omogućen na O365 pretplate.</span><span class="sxs-lookup"><span data-stu-id="34adc-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="34adc-110">U tom slučaju morat ćete se povezati s Exchange Online Powershell i pokretanje tog cmdleta:  *Set OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="34adc-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>