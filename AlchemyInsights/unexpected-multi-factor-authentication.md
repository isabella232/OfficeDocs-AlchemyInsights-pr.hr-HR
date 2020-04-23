---
title: Neočekivana višestruka provjera autentičnosti
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766593"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="d2160-102">Neočekivana višestruka provjera autentičnosti</span><span class="sxs-lookup"><span data-stu-id="d2160-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="d2160-103">Ako je vaš klijent stvoren nakon 21. listopada 2019., a vi neočekivano dobivate upit za MFA, vjerojatno imate [omogućene sigurnosne zadane postavke](https://aka.ms/securitydefaults) u svom klijentu.</span><span class="sxs-lookup"><span data-stu-id="d2160-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="d2160-104">Da biste upravljali zadanim postavkama sigurnosti:</span><span class="sxs-lookup"><span data-stu-id="d2160-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="d2160-105">Prijavite se u [centar za administratore](https://go.microsoft.com/fwlink/p/?linkid=834822) pomoću globalnih vjerodajnica administratora.</span><span class="sxs-lookup"><span data-stu-id="d2160-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="d2160-106">Idite na [svojstva servisa Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="d2160-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="d2160-107">Pri dnu stranice kliknite **Upravljanje zadanim postavkama sigurnosti**.</span><span class="sxs-lookup"><span data-stu-id="d2160-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="d2160-108">Kliknite **da** kako biste omogućili zadane postavke sigurnosti i **ne** kako biste onemogućili zadane postavke sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="d2160-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
