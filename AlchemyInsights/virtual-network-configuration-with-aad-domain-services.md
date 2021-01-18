---
title: Virtualna konfiguracija s servisima AAD domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884857"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="f8c27-102">Virtualna konfiguracija s servisima AAD domene</span><span class="sxs-lookup"><span data-stu-id="f8c27-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="f8c27-103">Virtualna konfiguracija uz usluge AAD domene obuhvaća sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="f8c27-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="f8c27-104">Provjeru zdravlja domene na portalu Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="f8c27-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="f8c27-105">Provjeru programa NSG za pravila koja blokiraju priključke potrebne za sinkronizaciju na servisu Azure AD domene na portalu https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="f8c27-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="f8c27-106">Osiguravanje da je Virtualna mreža raspoređena u istoj regiji Azure kao domena servisa Azure AD</span><span class="sxs-lookup"><span data-stu-id="f8c27-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="f8c27-107">Osiguravanje da nemate postojeću domenu s istim nazivom domene dostupnom na virtualnoj mreži.</span><span class="sxs-lookup"><span data-stu-id="f8c27-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="f8c27-108">Dodatne informacije o prikazu dizajna na virtualnoj mreži Azure za podršku servisima AAD domene potražite u članku [razmatranje virtualne mreže](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="f8c27-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

