---
title: Kod pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499374"
---
<span data-ttu-id="c4983-103">Ako si primanje pogreške tijekom aktivacije Office 2013 na uvođenja usluge udaljene radne površine (ZAPISI), razmislite o omogućavanju ADAL uređivanjem registra.</span><span class="sxs-lookup"><span data-stu-id="c4983-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="c4983-104">**Ključ registra**</span><span class="sxs-lookup"><span data-stu-id="c4983-104">**Registry key**</span></span>|<span data-ttu-id="c4983-105"> upišite </span><span class="sxs-lookup"><span data-stu-id="c4983-105">**Type**</span></span>|<span data-ttu-id="c4983-106">Vrijednost</span><span class="sxs-lookup"><span data-stu-id="c4983-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c4983-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="c4983-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="c4983-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="c4983-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="c4983-109">1</span><span class="sxs-lookup"><span data-stu-id="c4983-109">1</span></span>  <br/> |
   
<span data-ttu-id="c4983-110">Dodatne informacije potražite [Omogućiti Moderna provjere autentičnosti 2013 Office na Windows uređajima](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c4983-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="c4983-p101">ADAL je po zadanom omogućen u Office 365 ProPlus i 2016 za Office. > usluge udaljene radne površine (ZAPISI) je prethodno pod nazivom servisa Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="c4983-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

