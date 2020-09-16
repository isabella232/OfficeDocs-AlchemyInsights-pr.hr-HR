---
title: Više aktivnih sesija s istim poštanskim sandučićem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769715"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="d3c59-102">Više aktivnih sesija s istim poštanskim sandučićem</span><span class="sxs-lookup"><span data-stu-id="d3c59-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="d3c59-103">Da biste kontrolirali korištenje resursa sustava Exchange, poštanski sandučić sadrži "proračun".</span><span class="sxs-lookup"><span data-stu-id="d3c59-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="d3c59-104">Iznimku nad budžetom može pokrenuti, ali nije ograničen na sljedeće okolnosti:</span><span class="sxs-lookup"><span data-stu-id="d3c59-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="d3c59-105">U istoj sesiji programa Outlook Web App otvaraju se nekoliko kartica preglednika.</span><span class="sxs-lookup"><span data-stu-id="d3c59-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="d3c59-106">Malo aktivnih sesija web-aplikacije Outlook na istom poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="d3c59-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="d3c59-107">Neke druge klijentske aplikacije (Outlook, Outlook Mobile, klijentska aplikacija trećih strana) istodobno pristupaju poštanskom sandučiću.</span><span class="sxs-lookup"><span data-stu-id="d3c59-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="d3c59-108">Dugoročne operacije, kao što je izvršavanje zahtjeva za pretraživanje, izvode se iz drugog aktivnog sastanka poštanskog sandučića.</span><span class="sxs-lookup"><span data-stu-id="d3c59-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

