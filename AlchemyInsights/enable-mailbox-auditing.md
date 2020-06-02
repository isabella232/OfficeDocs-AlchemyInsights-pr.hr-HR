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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506946"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="84233-102">Omogućivanje nadzora poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="84233-102">Enable mailbox auditing</span></span>

<span data-ttu-id="84233-103">Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijelu organizaciju, sljedeći cmdleti moraju se izvoditi iz ljuske udaljene snage:</span><span class="sxs-lookup"><span data-stu-id="84233-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="84233-104">**Jedan korisnik**</span><span class="sxs-lookup"><span data-stu-id="84233-104">**Single User**</span></span>
  
<span data-ttu-id="84233-105">Set-Mailbox -Identitet "Jane Dow" -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="84233-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="84233-106">**Organizacije**</span><span class="sxs-lookup"><span data-stu-id="84233-106">**Organization**</span></span>
  
<span data-ttu-id="84233-107">Get-Mailbox-ResultSize Neograničeno -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="84233-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="84233-108">uči više</span><span class="sxs-lookup"><span data-stu-id="84233-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

