---
title: Šifra pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako se prilikom aktivacije sustava Office 2013 na implementacijama servisa udaljene radne površine (RDS) pojavljuje pogreška, razmislite o omogućivanju ADAL-a uređivanjem registra.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703130"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="b2e26-103">Pogreška prilikom aktivacije sustava Office 2013 na servisima udaljene radne površine</span><span class="sxs-lookup"><span data-stu-id="b2e26-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="b2e26-104">Ako se prilikom aktivacije sustava Office 2013 na implementacijama servisa udaljene radne površine (RDS) pojavljuje pogreška, razmislite o omogućivanju ADAL-a uređivanjem registra.</span><span class="sxs-lookup"><span data-stu-id="b2e26-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="b2e26-105">**Ključ registra**</span><span class="sxs-lookup"><span data-stu-id="b2e26-105">**Registry key**</span></span>|<span data-ttu-id="b2e26-106">**Tip**</span><span class="sxs-lookup"><span data-stu-id="b2e26-106">**Type**</span></span>|<span data-ttu-id="b2e26-107">**Vrijednost**</span><span class="sxs-lookup"><span data-stu-id="b2e26-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2e26-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b2e26-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b2e26-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="b2e26-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b2e26-110">1</span><span class="sxs-lookup"><span data-stu-id="b2e26-110">1</span></span>  <br/> |

<span data-ttu-id="b2e26-111">Dodatne informacije potražite u [odjeljku Omogućivanje moderne provjere autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b2e26-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b2e26-112">ADAL je omogućen prema zadanim postavkama u Aplikacijama microsoft 365 za tvrtke i Office 2016.</span><span class="sxs-lookup"><span data-stu-id="b2e26-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="b2e26-113">Servisi udaljene radne površine (RDS) prethodno su bili nazvani Servisi terminala.</span><span class="sxs-lookup"><span data-stu-id="b2e26-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  