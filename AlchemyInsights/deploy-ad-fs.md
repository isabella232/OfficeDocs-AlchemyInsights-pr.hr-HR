---
title: Implementacija oglasa FS-a
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177398"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="a8312-102">Implementacija oglasa FS-a</span><span class="sxs-lookup"><span data-stu-id="a8312-102">Deploy AD FS</span></span>

<span data-ttu-id="a8312-103">Implementacija Active Directory Federation Services (AD FS) koristi lokalnu infrastrukturu za provjeru autentičnosti korisnika za Office 365 Services.</span><span class="sxs-lookup"><span data-stu-id="a8312-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="a8312-104">Ako imate udruženu prijavu, korisnicima možete omogućiti prijavu u Office 365 Services i Software kao servisne (SAAS) aplikacije koje su integrirane sa servisom Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a8312-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="a8312-105">Udruženu prijavu potvrđuje korisnike u lokalnim servisima Active Directory putem aplikacije AD FS.</span><span class="sxs-lookup"><span data-stu-id="a8312-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="a8312-106">I dok se nalazite na mreži tvrtke, korisnici neće morati ponovno unositi lozinke.</span><span class="sxs-lookup"><span data-stu-id="a8312-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="a8312-107">[Savjetnik za implementaciju servisa AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) nudi detaljne upute o implementaciji lokalne infrastrukture AD FS koja provjerava autentičnost korisnika za Microsoft 365 i Office 365 Services.</span><span class="sxs-lookup"><span data-stu-id="a8312-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="a8312-108">Uz ovaj vodič vaša tvrtka ili ustanova može pregledavati komponente i preduvjete AD FS-a, steći i instalirati SSL certifikate koji su neophodni za implementaciju i instalirati obavezan proxy poslužitelj web-aplikacije.</span><span class="sxs-lookup"><span data-stu-id="a8312-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
