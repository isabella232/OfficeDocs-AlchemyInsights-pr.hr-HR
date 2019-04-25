---
title: Omogući nadzor poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403739"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="8ab9b-102">Omogući nadzor poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="8ab9b-102">Enable mailbox auditing</span></span>

<span data-ttu-id="8ab9b-103">Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijeloj organizaciji sljedeće Cmdletovi morate pokrenuti iz Remote Shell uštede energije:</span><span class="sxs-lookup"><span data-stu-id="8ab9b-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="8ab9b-104">**Jedan korisnik**</span><span class="sxs-lookup"><span data-stu-id="8ab9b-104">**Single User**</span></span>
  
<span data-ttu-id="8ab9b-105">Skup-poštanski sandučić - identitet "Dow Ane" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="8ab9b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="8ab9b-106">**Organizacija**</span><span class="sxs-lookup"><span data-stu-id="8ab9b-106">**Organization**</span></span>
  
<span data-ttu-id="8ab9b-107">Dohvati poštanski sandučić - ResultSize neograničen - filtriranje {RecipientTypeDetails - eq "UserMailbox"} | Skup poštanski sandučić - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="8ab9b-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="8ab9b-108">uči više</span><span class="sxs-lookup"><span data-stu-id="8ab9b-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

