---
title: Problemi s prijavom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900799"
---
# <a name="sign-out-issues"></a><span data-ttu-id="000ad-102">Problemi s prijavom</span><span class="sxs-lookup"><span data-stu-id="000ad-102">Sign-out issues</span></span>

<span data-ttu-id="000ad-103">Da biste riješili probleme vezane uz odjavu, slijedite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="000ad-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="000ad-104">Ako ste vi ili korisnik prijavljeni ili ste ga izbacili iz aplikacija, slijedite upute u člancima [konfigurirajte upravljanje sesijom provjere autentičnosti pomoću uvjetnog pristupa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) ili [konfiguriranog vremena tokena u Microsoftovoj platformi Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="000ad-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="000ad-105">Većina drugih pogrešaka pri odjavi ili problema može se riješiti otklanjanjem poteškoća s integracijom servisa Azure Active Directory (Azure AD) s određenom aplikacijom.</span><span class="sxs-lookup"><span data-stu-id="000ad-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="000ad-106">Upute za određenu integraciju možete pronaći tako da odete na [zbirku Tutoriali za integraciju aplikacija pomoću servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), uključujući sljedeće:</span><span class="sxs-lookup"><span data-stu-id="000ad-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="000ad-107">Tutoriali aplikacije SaaS</span><span class="sxs-lookup"><span data-stu-id="000ad-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="000ad-108">Tutoriali za jedinstvenu prijavu</span><span class="sxs-lookup"><span data-stu-id="000ad-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="000ad-109">Vodiči za korisnike – dodjelu resursa</span><span class="sxs-lookup"><span data-stu-id="000ad-109">User-provisioning tutorials</span></span>