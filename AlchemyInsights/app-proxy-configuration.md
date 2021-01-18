---
title: Konfiguracija proxyja aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884839"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="0db29-102">Konfiguracija proxyja aplikacija</span><span class="sxs-lookup"><span data-stu-id="0db29-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="0db29-103">Da biste razumjeli kako konfigurirati aplikaciju proxyja aplikacije u sklopu servisa Azure AD da biste u oblak izložili lokalne aplikacije, pročitajte članak [Konfiguriranje aplikacije proxyja aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="0db29-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="0db29-104">Jedinstvena prijava (SSO) korisnicima omogućuje pristup aplikaciji bez provjere autentičnosti više puta.</span><span class="sxs-lookup"><span data-stu-id="0db29-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="0db29-105">Omogućuje jedinstvenu provjeru autentičnosti u oblaku, na servisu Azure Active Directory i omogućuje oponašaju korisnika da izvrši dodatne izazove provjere autentičnosti u aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="0db29-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="0db29-106">Dodatne informacije potražite u članku [Konfiguriranje jedinstvene prijave u aplikaciju za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="0db29-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="0db29-107">Pomoću [ovog članka](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) možete otkloniti česte probleme s kojima se suočavaju osobe pri stvaranju nove aplikacije za proxy aplikacije.</span><span class="sxs-lookup"><span data-stu-id="0db29-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="0db29-108">Ako imate problema s postavljanjem sigurnosne provjere autentičnosti u aplikaciji, možda ćete morati [otkloniti poteškoće s ograničenjem programa za delegiranje poslužitelja za proxy poslužitelje](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ili pratiti upute za [Konfiguriranje aplikacije pomoću servisa pingaccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) da biste riješili problem.</span><span class="sxs-lookup"><span data-stu-id="0db29-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
