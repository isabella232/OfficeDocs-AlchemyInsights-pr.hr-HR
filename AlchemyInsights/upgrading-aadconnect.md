---
title: 932 Nadogradnja AADConnect-a
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806031"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="79520-102">Nadogradnja servisa Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="79520-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="79520-103">Po zadanom je omogućena automatska nadogradnja za Azure AD Connect, čime se omogućuje da koristite najnoviju verziju.</span><span class="sxs-lookup"><span data-stu-id="79520-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="79520-104">Da biste potvrdili postavke automatskog nadogradnje, upotrijebite cmdlet **Get-Adsyncautouprazreda** u aplikaciji Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="79520-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="79520-105">Cmdlet će vratiti jednu od sljedećih vrijednosti:</span><span class="sxs-lookup"><span data-stu-id="79520-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="79520-106">**Omogućeno**: omogućeno je automatsko ažuriranje.</span><span class="sxs-lookup"><span data-stu-id="79520-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="79520-107">**Onemogućeno**: automatska nadogradnja je onemogućena.</span><span class="sxs-lookup"><span data-stu-id="79520-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="79520-108">**Suspendirane**: sustav više ne ispunjava uvjete za primanje automatskih nadogradnji.</span><span class="sxs-lookup"><span data-stu-id="79520-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="79520-109">Ne možete konfigurirati tu vrijednost; postavlja ga sustav.</span><span class="sxs-lookup"><span data-stu-id="79520-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="79520-110">Dodatne informacije potražite u članku [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="79520-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="79520-111">Da biste preuzeli najnoviju verziju servisa Azure AD Connect, otvorite [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="79520-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
