---
title: Omogućivanje nadzora poštanskog sandučića
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806283"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="be054-102">Omogućivanje nadzora poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="be054-102">Enable mailbox auditing</span></span>

<span data-ttu-id="be054-103">Da biste omogućili nadziranje poštanskog sandučića za jednog korisnika ili cijelu tvrtku ili ustanovu, sljedeći se cmdleti moraju pokrenuti iz udaljenog dodatka Power Shell:</span><span class="sxs-lookup"><span data-stu-id="be054-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="be054-104">**Jedan korisnik**</span><span class="sxs-lookup"><span data-stu-id="be054-104">**Single User**</span></span>
  
<span data-ttu-id="be054-105">Zalazak-poštanski sandučić – identitet "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="be054-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="be054-106">**Tvrtke ili ustanove**</span><span class="sxs-lookup"><span data-stu-id="be054-106">**Organization**</span></span>
  
<span data-ttu-id="be054-107">Nabavite-Mailbox-rezultat neograničeno-filtar {RecipientTypeDetails-aq "UserMailbox"} | $true s mogućnošću postavljanje poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="be054-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="be054-108">uči više</span><span class="sxs-lookup"><span data-stu-id="be054-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

