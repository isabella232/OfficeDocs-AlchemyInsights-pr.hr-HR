---
title: 932 Nadogradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766485"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="3db92-102">Nadogradnja usluge Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3db92-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="3db92-103">Prema zadanim postavkama, automatska nadogradnja omogućena je za Azure AD Connect, čime se osigurava da koristite najnoviju verziju.</span><span class="sxs-lookup"><span data-stu-id="3db92-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="3db92-104">Da biste provjerili postavke automatske nadogradnje, koristite cmdlet **Get-ADSyncAutoUpgrade** u Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3db92-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="3db92-105">Cmdlet će vratiti jednu od sljedećih vrijednosti:</span><span class="sxs-lookup"><span data-stu-id="3db92-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="3db92-106">**Omogućeno**: Omogućena je automatska nadogradnja.</span><span class="sxs-lookup"><span data-stu-id="3db92-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="3db92-107">**Onemogućeno:** Automatska nadogradnja je onemogućena.</span><span class="sxs-lookup"><span data-stu-id="3db92-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="3db92-108">**Obustavljeno:** sustav više ne ispunjava uvjete za primanje automatskih nadogradnji.</span><span class="sxs-lookup"><span data-stu-id="3db92-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="3db92-109">Tu vrijednost ne možete konfigurirati; To je postavljen od strane sustava.</span><span class="sxs-lookup"><span data-stu-id="3db92-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="3db92-110">Dodatne informacije potražite u [odjeljku Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="3db92-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="3db92-111">Da biste preuzeli najnoviju verziju [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)usluge Azure AD Connect, idite na .</span><span class="sxs-lookup"><span data-stu-id="3db92-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
