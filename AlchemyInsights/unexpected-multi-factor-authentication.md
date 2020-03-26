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
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946609"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="dd271-102">Neočekivana višestruka provjera autentičnosti</span><span class="sxs-lookup"><span data-stu-id="dd271-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="dd271-103">Ako je vaš klijent stvoren nakon 21. listopada 2019., a vi neočekivano dobivate upit za MFA, vjerojatno imate [omogućene sigurnosne zadane postavke](http://aka.ms/securitydefaults) u svom klijentu.</span><span class="sxs-lookup"><span data-stu-id="dd271-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="dd271-104">Da biste upravljali zadanim postavkama sigurnosti:</span><span class="sxs-lookup"><span data-stu-id="dd271-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="dd271-105">Prijavite se u [centar za administratore](https://go.microsoft.com/fwlink/p/?linkid=834822) pomoću globalnih vjerodajnica administratora.</span><span class="sxs-lookup"><span data-stu-id="dd271-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="dd271-106">Idite na [svojstva servisa Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="dd271-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="dd271-107">Pri dnu stranice kliknite **Upravljanje zadanim postavkama sigurnosti**.</span><span class="sxs-lookup"><span data-stu-id="dd271-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="dd271-108">Kliknite **da** kako biste omogućili zadane postavke sigurnosti i **ne** kako biste onemogućili zadane postavke sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="dd271-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
