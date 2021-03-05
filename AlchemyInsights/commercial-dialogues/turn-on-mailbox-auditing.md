---
title: Uključivanje nadzora poštanskog sandučića
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481244"
---
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="84de7-102">Uključivanje nadzora poštanskog sandučića</span><span class="sxs-lookup"><span data-stu-id="84de7-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="84de7-103">Da biste uključili nadzor poštanskog sandučića za jednog korisnika ili cijelu tvrtku ili ustanovu, pokrenite sljedeće cmdlete iz udaljene komponente PowerShell:</span><span class="sxs-lookup"><span data-stu-id="84de7-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="84de7-104">**Jednostruki korisnik**: Set-Mailbox-Identity "Jane Dow" – auditenabled $True</span><span class="sxs-lookup"><span data-stu-id="84de7-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="84de7-105">**Tvrtka ili ustanova**: Get-Mailbox-Rezultsize neograničeno-filtar {RecipientTypeDetails-aq "UserMailbox"} | Set-Mailbox $true</span><span class="sxs-lookup"><span data-stu-id="84de7-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="84de7-106">Dodatne informacije potražite u članku [Upravljanje nadziranje poštanskog sandučića](https://go.microsoft.com/fwlink/?linkid=2103668).</span><span class="sxs-lookup"><span data-stu-id="84de7-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>