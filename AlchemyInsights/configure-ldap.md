---
title: Konfiguriranje LDAP-a
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884845"
---
# <a name="configure-ldap"></a><span data-ttu-id="e01a5-102">Konfiguriranje LDAP-a</span><span class="sxs-lookup"><span data-stu-id="e01a5-102">Configure LDAP</span></span>

<span data-ttu-id="e01a5-103">Da biste konfigurirali LDAP, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e01a5-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="e01a5-104">Provjerite zdravlje domene na [portalu Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="e01a5-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="e01a5-105">Provjerite je li dostupna valjana pretplata na Azure AD, a omogućen je i Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="e01a5-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="e01a5-106">Certifikat potreban za omogućavanje sigurnog LDAP-a mora biti dobiven od pouzdanih javnih ustanova za izdavanje certifikata ili biti samopotpisani certifikat.</span><span class="sxs-lookup"><span data-stu-id="e01a5-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="e01a5-107">Uvjerite se da certifikat slijedi potrebne [smjernice](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="e01a5-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="e01a5-108">**Potvrda nije valjana**</span><span class="sxs-lookup"><span data-stu-id="e01a5-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="e01a5-109">Da biste obnovili certifikat, slijedite korake za stvaranje novog certifikata i Reupload: [Konfigurisanje LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)-a.</span><span class="sxs-lookup"><span data-stu-id="e01a5-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="e01a5-110">Da biste riješili poznat problem s sigurnim LDAP upozorenjima u domenama servisa Azure Active Directory, pročitajte članak [rješavanje LDAP upozorenja](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="e01a5-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
