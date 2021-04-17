---
title: Omogućivanje besprijekornog SSO-a
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825723"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="a0280-102">Omogućivanje besprijekornog SSO-a</span><span class="sxs-lookup"><span data-stu-id="a0280-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="a0280-103">Omogućivanje besprijekornog SSO-a putem [servisa Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="a0280-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="a0280-104">Ako radite novu instalaciju servisa Azure AD Connect, odaberite prilagođeni [put instalacije.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)</span><span class="sxs-lookup"><span data-stu-id="a0280-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="a0280-105">Na **stranici Prijava korisnika** odaberite mogućnost Omogući **jedinstvenu** prijavu.</span><span class="sxs-lookup"><span data-stu-id="a0280-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="a0280-106">Da biste provjerili jeste li omogućili besprijekornu SSO ispravan način:</span><span class="sxs-lookup"><span data-stu-id="a0280-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="a0280-107">Prijavite se u [administrativni centar servisa Azure Active Directory](https://aad.portal.azure.com) kao globalni administrator.</span><span class="sxs-lookup"><span data-stu-id="a0280-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="a0280-108">U **lijevom oknu odaberite Azure Active Directory.**</span><span class="sxs-lookup"><span data-stu-id="a0280-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="a0280-109">Provjerite je li jedinstvena jedinstvena prijava **omogućena**.</span><span class="sxs-lookup"><span data-stu-id="a0280-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="a0280-110">Dodatne informacije potražite u članku [Besprijekorna jedinstvena prijava servisa Azure Active Directory: brzi početak rada.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)</span><span class="sxs-lookup"><span data-stu-id="a0280-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  