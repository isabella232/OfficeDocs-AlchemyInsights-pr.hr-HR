---
title: Kod pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929080"
---
<span data-ttu-id="b3a03-103">Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.</span><span class="sxs-lookup"><span data-stu-id="b3a03-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="b3a03-104">**Ključ registra**</span><span class="sxs-lookup"><span data-stu-id="b3a03-104">**Registry key**</span></span>|<span data-ttu-id="b3a03-105">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="b3a03-105">**Type**</span></span>|<span data-ttu-id="b3a03-106">**Vrijednost**</span><span class="sxs-lookup"><span data-stu-id="b3a03-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b3a03-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b3a03-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b3a03-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b3a03-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b3a03-109">1</span><span class="sxs-lookup"><span data-stu-id="b3a03-109">1</span></span>  <br/> |
   
<span data-ttu-id="b3a03-110">Dodatne informacije potražite [Omogućiti Moderna provjere autentičnosti 2013 Office na Windows uređajima](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b3a03-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b3a03-p101">ADAL je po zadanom omogućen u Office 365 ProPlus i 2016 za Office. > usluge udaljene radne površine (ZAPISI) je prethodno pod nazivom servisa Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="b3a03-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

