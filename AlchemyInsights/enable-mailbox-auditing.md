---
title: Omogući nadzor poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500274"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="f5b87-102">Omogući nadzor poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="f5b87-102">Enable mailbox auditing</span></span>

<span data-ttu-id="f5b87-103">Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijeloj organizaciji sljedeće Cmdletovi morate pokrenuti iz Remote Shell uštede energije:</span><span class="sxs-lookup"><span data-stu-id="f5b87-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="f5b87-104">**Jedan korisnik**</span><span class="sxs-lookup"><span data-stu-id="f5b87-104">**Single User**</span></span>
  
<span data-ttu-id="f5b87-105">Skup-poštanski sandučić - identitet "Dow Ane" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="f5b87-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="f5b87-106">Organization</span><span class="sxs-lookup"><span data-stu-id="f5b87-106">**Organization**</span></span>
  
<span data-ttu-id="f5b87-107">Dohvati poštanski sandučić - ResultSize neograničen - filtriranje {RecipientTypeDetails - eq "UserMailbox"} | Skup poštanski sandučić - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="f5b87-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
<span data-ttu-id="f5b87-108">Dodatne informacije</span><span class="sxs-lookup"><span data-stu-id="f5b87-108">[Learn more](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)</span></span>
  

