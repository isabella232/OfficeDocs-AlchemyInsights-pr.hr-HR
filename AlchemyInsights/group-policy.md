---
title: Pravilnik grupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256666"
---
# <a name="group-policy"></a><span data-ttu-id="cd089-102">Pravilnik grupe</span><span class="sxs-lookup"><span data-stu-id="cd089-102">Group policy</span></span>

<span data-ttu-id="cd089-103">Postavke za korisničke i računalne objekte u servisu Azure Active Directory domene (Azure AD DS) često se upravljaju pomoću objekata pravilnika grupe (GPOs-a).</span><span class="sxs-lookup"><span data-stu-id="cd089-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="cd089-104">Azure AD DS sadrži ugrađene GPOs-ove za korisnike AADDC i kontejnere AADDC Computers.</span><span class="sxs-lookup"><span data-stu-id="cd089-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="cd089-105">Te ugrađene GPOs možete prilagoditi za konfiguriranje pravilnika grupe prema potrebi za okruženje.</span><span class="sxs-lookup"><span data-stu-id="cd089-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="cd089-106">Članovi grupe Administratori Azure AD DC imaju privilegije za administraciju pravilnika grupe u domeni Azure AD DS, a mogu stvarati i prilagođene GPOs i organizacijske jedinice (OUs).</span><span class="sxs-lookup"><span data-stu-id="cd089-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="cd089-107">Dodatne informacije o pravilima grupe i načinu rada potražite u članku [Pregled pravilnika grupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="cd089-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="cd089-108">U hibridnom okruženju pravila grupe konfigurirana u lokalnom okruženju AD DS nisu sinkronizirane sa servisom Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="cd089-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="cd089-109">Da biste definirali konfiguracijske postavke za korisnike ili računala u servisu Azure AD DS, uredite jedan od zadanih GPOs-a ili stvorite prilagođeni GPO.</span><span class="sxs-lookup"><span data-stu-id="cd089-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="cd089-110">U ovom se članku [upravlja pravilima grupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) , a prikazuje se kako instalirati alate za upravljanje pravilima grupe, kako ton uređivati ugrađene gpos-ove i kako stvoriti prilagođene gpos-ove.</span><span class="sxs-lookup"><span data-stu-id="cd089-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



