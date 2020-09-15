---
title: Kod pogreške 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako vam se prikaže pogreška prilikom aktivacije sustava Office 2013 u implementacijama servisa udaljene radne površine (RDS-a), razmotrite Omogućivanje ADALA uređivanjem registra.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709179"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="29529-103">Pogreška prilikom aktivacije sustava Office 2013 na servisima udaljene radne površine</span><span class="sxs-lookup"><span data-stu-id="29529-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="29529-104">Ako vam se prikaže pogreška prilikom aktivacije sustava Office 2013 u implementacijama servisa udaljene radne površine (RDS-a), razmotrite Omogućivanje ADALA uređivanjem registra.</span><span class="sxs-lookup"><span data-stu-id="29529-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="29529-105">**Ključ registra**</span><span class="sxs-lookup"><span data-stu-id="29529-105">**Registry key**</span></span>|<span data-ttu-id="29529-106">**Upišite**</span><span class="sxs-lookup"><span data-stu-id="29529-106">**Type**</span></span>|<span data-ttu-id="29529-107">**Vrijednost**</span><span class="sxs-lookup"><span data-stu-id="29529-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="29529-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="29529-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="29529-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="29529-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="29529-110">1</span><span class="sxs-lookup"><span data-stu-id="29529-110">1</span></span>  <br/> |

<span data-ttu-id="29529-111">Dodatne informacije potražite u članku [Omogućivanje moderne provjere autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="29529-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="29529-112">ADAL je prema zadanim postavkama omogućen u aplikacijama Microsoft 365 za Enterprise i Office 2016.</span><span class="sxs-lookup"><span data-stu-id="29529-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="29529-113">Servisi udaljene radne površine (RDS) prethodno su imenovani terminalskim servisima.</span><span class="sxs-lookup"><span data-stu-id="29529-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  