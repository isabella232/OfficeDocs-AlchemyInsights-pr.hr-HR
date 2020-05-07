---
title: Exchange PowerShell i osnovna provjera autentičnosti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015681"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="cd41b-102">Exchange PowerShell i osnovna provjera autentičnosti</span><span class="sxs-lookup"><span data-stu-id="cd41b-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="cd41b-103">Najnovije informacije o povezivanju sa sustavom Exchange Online PowerShell bez upotrebe osnovne provjere autentičnosti [pronađite ovdje](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="cd41b-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="cd41b-104">Imajte na umu da osnovna provjera autentičnosti još uvijek mora biti omogućena na klijentskom uređaju.</span><span class="sxs-lookup"><span data-stu-id="cd41b-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="cd41b-105">Novi modul PowerShell V2 koristi modernu provjeru autentičnosti kako bi uspostavio vezu i omogućio sve V2 cmdlete koji se oslanjaju na REST.</span><span class="sxs-lookup"><span data-stu-id="cd41b-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="cd41b-106">Osim V2 cmdleta, on vam omogućuje i pristup starijim cmdletima za Remote PowerShell (RPS) za koje je potrebno uspostaviti sesiju ljuske Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd41b-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="cd41b-107">Uspostavljanje RPS sesije na računalu sa sustavom Windows zahtijeva da se na klijentskom računalu omogući WinRM BasicAuth čak i u slučaju da za provjeru autentičnosti prilikom pristupanja servisu modul koristi mehanizam moderne provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="cd41b-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="cd41b-108">Za prijenos tokena moderne provjere autentičnosti koristi se komunikacijski kanal provjere autentičnosti WinRM Basic.</span><span class="sxs-lookup"><span data-stu-id="cd41b-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="cd41b-109">Ako je provjera autentičnosti WinRM Basic onemogućena na klijentskom računalu, novi će V2 cmdleti i dalje funkcionirati (no stariji RPS cmdleti neće).</span><span class="sxs-lookup"><span data-stu-id="cd41b-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
