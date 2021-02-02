---
title: Promjena postavki ograničenja za IWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075889"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="0d97e-102">Promjena postavki ograničenja za IWS</span><span class="sxs-lookup"><span data-stu-id="0d97e-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="0d97e-103">Pokrenite naš automatizirani test koji će vam dopustiti promjenu pravilnika o ograničavanju EWS-a za trajanje migracije.</span><span class="sxs-lookup"><span data-stu-id="0d97e-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="0d97e-104">Imajte na sebi da će, čak i nakon ovog pokretanja, Uvoz e-pošta i dalje biti ograničen na 150mb po 5 minuta po poštanskom sandučiću. Da biste postigli veću brzinu prelaska migracije, molimo vas da istodobno migrirate više korisnika.</span><span class="sxs-lookup"><span data-stu-id="0d97e-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="0d97e-105">Napominjemo da promjene pravilnika za EWS ograničavanja ne utječu na sljedeće vrste migracije (pomoću Microsoftova alata): hibridno, rezanje/organizirano (RPC/HTTP), IMAP, G suite, javna mapa ili PST uvoz servisa.</span><span class="sxs-lookup"><span data-stu-id="0d97e-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>