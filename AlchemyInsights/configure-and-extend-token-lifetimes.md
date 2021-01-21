---
title: Konfiguriranje i proširivanje životnog razdoblja tokena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916687"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="0e3f6-102">Konfiguriranje i proširivanje životnog razdoblja tokena</span><span class="sxs-lookup"><span data-stu-id="0e3f6-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="0e3f6-103">Možete navesti vijek trajanja programa Access, SAML ili ID token koji je izdala Microsoftova osobna platforma.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="0e3f6-104">U svim aplikacijama u vašoj tvrtki ili ustanovi možete postaviti znak trajanja tokena, za višečlansku (multi-organizacijsku) aplikaciju ili za određenog upravitelja servisa u vašoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="0e3f6-105">Dodatne informacije potražite u odjeljku [simbol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)</span><span class="sxs-lookup"><span data-stu-id="0e3f6-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="0e3f6-106">Primjeri, pročitajte [primjere kako konfigurirati životni vijek tokena](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="0e3f6-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="0e3f6-107">Upute za konfiguriranje životnog vijeka i kompatibilnosti tokena u servisu Azure Active Directory B2C (Azure AD B2C) potražite [u članku Konfiguriranje žetona u servisu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="0e3f6-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="0e3f6-108">U članku [Konfiguriranje ponašanja sesije u servisu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) opisuje metode jedinstvenog prijave (SSO) koje se koriste u servisu Azure ad B2C i olakšava odabir NAJPRIKLADNIJE metode SSO prilikom konfiguriranja pravilnika.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="0e3f6-109">**Koliko dugo traje tokeni? Koliko dugo vrijede?**</span><span class="sxs-lookup"><span data-stu-id="0e3f6-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="0e3f6-110">Životni vijek tokena je 1 sat, a Trajanje sesije 24 sata.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="0e3f6-111">To znači da ako u 24 sata ne bude nikakvih zahtjeva, morat ćete se ponovno prijaviti prije nego što zatražite novi token.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="0e3f6-112">Nakon 30 svibnja 2020, nijedan novi stanar neće moći koristiti pravilnik o životnom vijeku tokena za konfiguriranje sesija i osvježavanja žetona.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="0e3f6-113">Ukidanje će se dogoditi u roku od nekoliko mjeseci nakon toga, što znači da ćemo prekinuti s poštivanju postojećih sesija i osvježavanjem znakova tokena.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="0e3f6-114">Još uvijek možete konfigurirati Access token za životni vijek nakon razdiobe.</span><span class="sxs-lookup"><span data-stu-id="0e3f6-114">You can still configure access token lifetimes after the deprecation.</span></span>






