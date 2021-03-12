---
title: Otklanjanje poteškoća s jedinstvenom prijavom (SSO) koje se temelje na lozinkama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714678"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="8e1e9-102">Otklanjanje poteškoća s jedinstvenom prijavom (SSO) koje se temelje na lozinkama</span><span class="sxs-lookup"><span data-stu-id="8e1e9-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="8e1e9-103">Da biste naučili osnove dodatka SSO, pročitajte članak [Provjera autentičnosti temeljena na lozinkama pomoću servisa Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="8e1e9-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="8e1e9-104">**Konfigurirajte SSO utemeljenu na lozinci**</span><span class="sxs-lookup"><span data-stu-id="8e1e9-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="8e1e9-105">[Konfigurirajte jedinstvenu prijavu utemeljenu na lozinci](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) u ovom članku prikazuje se detaljnije o mogućnosti SSO koje se temelje na lozinkama.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="8e1e9-106">Ako aplikacija koju dodajete zahtijeva prilagođenu konfiguraciju i morate koristiti SSO na temelju lozinke, ovaj je članak namijenjen vama.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="8e1e9-107">[Konfigurirajte jedinstvenu prijavu utemeljenu na lozinkama za aplikacije na – Prem Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -Application proksiji podržava nekoliko pojedinačnih načina prijave.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="8e1e9-108">Prijava temeljena na lozinkama namijenjena je aplikacijama koje koriste kombinaciju korisničkog imena i lozinke za provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="8e1e9-109">Kada konfigurirate prijavu utemeljenu na lozinci za aplikaciju, korisnici se moraju prijaviti u lokalnu aplikaciju jednom.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="8e1e9-110">Nakon toga, Azure Active Directory pohranjuje podatke za prijavu i automatski ga pruža aplikaciji kada korisnici na daljinu pristupe.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="8e1e9-111">Već ste trebali objaviti i testirati aplikaciju uz proxy aplikacije.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="8e1e9-112">Ako ne, slijedite korake u članku [Objava aplikacija pomoću proxy poslužitelja Azure ad Application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) , a zatim nastavite s konfiguracijom SSO-a utemeljenih na lozinkama za aplikacije u programu on-Prem.</span><span class="sxs-lookup"><span data-stu-id="8e1e9-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="8e1e9-113">Da biste otklonili problem sa SSO-om, pročitajte članak [Otklanjanje poteškoća s jedinstvenom prijavom u Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="8e1e9-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
