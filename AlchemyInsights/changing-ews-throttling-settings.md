---
title: Promjena postavki ograničavanja EWS-a
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818028"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="2145d-102">Promjena postavki ograničavanja EWS-a</span><span class="sxs-lookup"><span data-stu-id="2145d-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="2145d-103">Pokrenite naš automatizirani test koji će vam omogućiti izmjenu pravilnika ograničavanja EWS-a tijekom trajanja migracije.</span><span class="sxs-lookup"><span data-stu-id="2145d-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="2145d-104">Imajte na umu da će uvoz EWS-a i nakon toga biti ograničen na 150 mb po 5 minuta po poštanskom sandučiću. da biste postigli veće brzine propusnosti migracije, istodobno migrirati više korisnika.</span><span class="sxs-lookup"><span data-stu-id="2145d-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="2145d-105">Imajte na umu da promjene pravilnika ograničavanja EWS-a ne utječu na sljedeće vrste migracije (pomoću Microsoftovih alata): hibridni, posložni (RPC/HTTP), IMAP, G Suite, javna mapa ili PST servis za uvoz.</span><span class="sxs-lookup"><span data-stu-id="2145d-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>