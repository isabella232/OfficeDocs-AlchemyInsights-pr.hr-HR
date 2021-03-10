---
title: Otklanjanje poteškoća sa servisom SSO za provjeru autentičnosti na temelju
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "9409"
ms.openlocfilehash: c053e252edfcc51c95214c4bff4aded2bded2e23
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692797"
---
# <a name="troubleshoot-saml-based-sso-authentication-issues"></a><span data-ttu-id="e5471-102">Otklanjanje poteškoća sa servisom SSO za provjeru autentičnosti na temelju</span><span class="sxs-lookup"><span data-stu-id="e5471-102">Troubleshoot SAML-based SSO authentication issues</span></span>

<span data-ttu-id="e5471-103">Većina korisnika može razriješiti probleme s pomoću servisa SSO za provjeru autentičnosti na temelju sljedećih preporučenih koraka:</span><span class="sxs-lookup"><span data-stu-id="e5471-103">Most users are able to resolve their SAML-based SSO authentication issues using the following recommended steps:</span></span>

<span data-ttu-id="e5471-104">**Preporučeni koraci**</span><span class="sxs-lookup"><span data-stu-id="e5471-104">**Recommended Steps**</span></span>
1. <span data-ttu-id="e5471-105">Pronalaženje [aktualnih podataka o kodu pogreške](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information).</span><span class="sxs-lookup"><span data-stu-id="e5471-105">Lookup [current error code information](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information).</span></span>
1. <span data-ttu-id="e5471-106">Da biste riješili pogreške provjere autentičnosti, na servisu [Azure Active Directory pogledajte odjeljak debug SAML na temelju jedinstvene prijave](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) .</span><span class="sxs-lookup"><span data-stu-id="e5471-106">See [Debug SAML-based single sign-on to applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) to resolve authentication errors.</span></span>
1. <span data-ttu-id="e5471-107">Pogledajte članak, [Single Sign-On saml protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) da biste saznali više o zahtjevima za provjeru autentičnosti saml 2,0 i odgovorima koje podržava Azure Active Directory (Azure AD) za single Sign-On (SSO).</span><span class="sxs-lookup"><span data-stu-id="e5471-107">Refer to the article, [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) to learn about the SAML 2.0 authentication requests and responses that Azure Active Directory (Azure AD) supports for Single Sign-On (SSO).</span></span>


