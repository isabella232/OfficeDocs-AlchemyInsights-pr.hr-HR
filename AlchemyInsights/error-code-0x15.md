---
title: Kod pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526972"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="247ab-103">Pogreška tijekom aktivacije Office 2013 na udaljene radne površine</span><span class="sxs-lookup"><span data-stu-id="247ab-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="247ab-104">Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.</span><span class="sxs-lookup"><span data-stu-id="247ab-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="247ab-105">**Ključ registra**</span><span class="sxs-lookup"><span data-stu-id="247ab-105">**Registry key**</span></span>|<span data-ttu-id="247ab-106">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="247ab-106">**Type**</span></span>|<span data-ttu-id="247ab-107">**Vrijednost**</span><span class="sxs-lookup"><span data-stu-id="247ab-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="247ab-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="247ab-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="247ab-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="247ab-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="247ab-110">1</span><span class="sxs-lookup"><span data-stu-id="247ab-110">1</span></span>  <br/> |

<span data-ttu-id="247ab-111">Dodatne informacije potražite [Omogućiti Moderna provjere autentičnosti 2013 Office na Windows uređajima](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="247ab-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="247ab-112">ADAL je po zadanom omogućen u Office 365 ProPlus i 2016 za Office.</span><span class="sxs-lookup"><span data-stu-id="247ab-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="247ab-113">Usluge udaljene radne površine (ZAPISI) je prethodno pod nazivom servisa Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="247ab-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  