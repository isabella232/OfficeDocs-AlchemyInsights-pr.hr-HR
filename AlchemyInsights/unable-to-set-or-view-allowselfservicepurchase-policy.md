---
title: Nije moguće postaviti ili prikazati pravilnik AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826083"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="69b08-102">Nije moguće postaviti ili prikazati pravilnik AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="69b08-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="69b08-103">Kada pokušate postaviti ili prikazati pravilnik AllowSelfServicePurchase, primit ćete sljedeću poruku o pogrešci:</span><span class="sxs-lookup"><span data-stu-id="69b08-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="69b08-104">*HandleError : Nije uspjelo dohvaćanje pravilnika o proizvodu uz PolicyId 'AllowSelfServicePurchase', ErrorMessage – veza u podlozi je zatvorena: došlo je do neočekivane pogreške prilikom slanja.*</span><span class="sxs-lookup"><span data-stu-id="69b08-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="69b08-105">To može biti zbog starije verzije sigurnosti transportnog sloja (TLS).</span><span class="sxs-lookup"><span data-stu-id="69b08-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="69b08-106">Da biste povezali servis MSCommerce, morate koristiti TLS 1.2 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="69b08-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="69b08-107">Isprobajte sljedeće korake da biste omogućili/postavili TLS protokol na 1.2, potvrdili i ponovno pokušali.</span><span class="sxs-lookup"><span data-stu-id="69b08-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="69b08-108">U naredbeni redak komponente PowerShell (PS C: unesite sljedeću naredbu da biste \) protokol TLS postavili na verziju 1.2:</span><span class="sxs-lookup"><span data-stu-id="69b08-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="69b08-109">Provjerite protokole TLS koji se koriste pomoću sljedeće naredbe:</span><span class="sxs-lookup"><span data-stu-id="69b08-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="69b08-110">Po potrebi ponovno pokušajte s naredbama Get or Update.</span><span class="sxs-lookup"><span data-stu-id="69b08-110">Retry the Get or Update commands as needed.</span></span>

