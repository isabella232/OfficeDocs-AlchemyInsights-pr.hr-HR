---
title: Omogućivanje nadzora poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703563"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="0b6e9-102">Omogućivanje nadzora poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="0b6e9-102">Enable mailbox auditing</span></span>

<span data-ttu-id="0b6e9-103">Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijelu organizaciju, sljedeći cmdleti moraju se pokrenuti iz ljuske udaljene energije:</span><span class="sxs-lookup"><span data-stu-id="0b6e9-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="0b6e9-104">**Jedan korisnik**</span><span class="sxs-lookup"><span data-stu-id="0b6e9-104">**Single User**</span></span>
  
<span data-ttu-id="0b6e9-105">Set-Mailbox -Identitet "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0b6e9-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="0b6e9-106">**Organizacije**</span><span class="sxs-lookup"><span data-stu-id="0b6e9-106">**Organization**</span></span>
  
<span data-ttu-id="0b6e9-107">Get-Mailbox-ResultSize Neograničeno -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0b6e9-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="0b6e9-108">uči više</span><span class="sxs-lookup"><span data-stu-id="0b6e9-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

