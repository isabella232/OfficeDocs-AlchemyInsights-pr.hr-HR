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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736245"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="bf16b-102">Omogući nadzor poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="bf16b-102">Enable mailbox auditing</span></span>

<span data-ttu-id="bf16b-103">Da biste omogućili nadzor poštanskog sandučića za jednog korisnika ili cijeloj organizaciji sljedeće Cmdletovi morate pokrenuti iz Remote Shell uštede energije:</span><span class="sxs-lookup"><span data-stu-id="bf16b-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="bf16b-104">**Jedan korisnik**</span><span class="sxs-lookup"><span data-stu-id="bf16b-104">**Single User**</span></span>
  
<span data-ttu-id="bf16b-105">Skup-poštanski sandučić - identitet "Dow Ane" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bf16b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="bf16b-106">**Organizacija**</span><span class="sxs-lookup"><span data-stu-id="bf16b-106">**Organization**</span></span>
  
<span data-ttu-id="bf16b-107">Dohvati poštanski sandučić - ResultSize neograničen - filtriranje {RecipientTypeDetails - eq "UserMailbox"} | Skup poštanski sandučić - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bf16b-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="bf16b-108">uči više</span><span class="sxs-lookup"><span data-stu-id="bf16b-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

