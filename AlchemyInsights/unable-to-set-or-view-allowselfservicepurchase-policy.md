---
title: Nije moguće postaviti ili pregledati pravila AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091674"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="91fda-102">Nije moguće postaviti ili pregledati pravila AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="91fda-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="91fda-103">Prilikom pokušaja postavljanja ili prikaza pravila AllowSelfServicePurchase dobivate sljedeću poruku o pogrešci:</span><span class="sxs-lookup"><span data-stu-id="91fda-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="91fda-104">*HandleError : Dohvaćanje pravila proizvoda s Pravilima Id 'AllowSelfServicePurchase', ErrorMessage - Veza u podlozi je zatvorena: Došlo je do neočekivane pogreške prilikom slanja.*</span><span class="sxs-lookup"><span data-stu-id="91fda-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="91fda-105">To može biti zbog starije verzije Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="91fda-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="91fda-106">Da biste povezali uslugu MSCommerce, morate koristiti TLS 1.2 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="91fda-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="91fda-107">Pokušajte sljedeće korake da biste omogućili/postavili TLS protokol na 1.2, provjerili i ponovno pokušali.</span><span class="sxs-lookup"><span data-stu-id="91fda-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="91fda-108">U naredbeni redak PowerShell\) (PS C: unesite sljedeću naredbu da biste TLS protokol postavili na verziju 1.2:</span><span class="sxs-lookup"><span data-stu-id="91fda-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="91fda-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="91fda-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="91fda-110">Provjerite TLS protokole koji se koriste pomoću sljedeće naredbe:</span><span class="sxs-lookup"><span data-stu-id="91fda-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="91fda-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="91fda-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="91fda-112">Po potrebi ponovno pokušajte naredbe Get or Update.</span><span class="sxs-lookup"><span data-stu-id="91fda-112">Retry the Get or Update commands as needed.</span></span>

