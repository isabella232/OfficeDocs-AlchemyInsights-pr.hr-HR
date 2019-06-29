---
title: 932 Nadogradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365882"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="fe1b6-102">Nadogradnja Azure AD povezivanje</span><span class="sxs-lookup"><span data-stu-id="fe1b6-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="fe1b6-103">Po zadanom, automatsko nadogradnje je omogućena za Azure AD povezivanje, što pomaže vam osigurati koristite najnoviju verziju.</span><span class="sxs-lookup"><span data-stu-id="fe1b6-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="fe1b6-104">Da biste provjerili postavke automatskog nadogradnje, koristite cmdlet **Get-ADSyncAutoUpgrade** u PowerShellu AD Azure.</span><span class="sxs-lookup"><span data-stu-id="fe1b6-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="fe1b6-105">U cmdlet vratit će jedna od sljedećih vrijednosti:</span><span class="sxs-lookup"><span data-stu-id="fe1b6-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="fe1b6-106">**Omogućeno**: omogućeno automatsko nadogradnju.</span><span class="sxs-lookup"><span data-stu-id="fe1b6-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="fe1b6-107">**Onemogućen**: automatsko Nadogradnja je onemogućena.</span><span class="sxs-lookup"><span data-stu-id="fe1b6-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="fe1b6-108">**Suspended**: više nije pravo na primanje automatske nadogradnje sustava.</span><span class="sxs-lookup"><span data-stu-id="fe1b6-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="fe1b6-109">Nije moguće konfigurirati vrijednost; postavite je sustav.</span><span class="sxs-lookup"><span data-stu-id="fe1b6-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="fe1b6-110">Za dodatne informacije pogledajte [Automatsko nadogradnje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="fe1b6-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="fe1b6-111">Da biste preuzeli najnoviju verziju Azure AD povezivanje, idite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="fe1b6-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
