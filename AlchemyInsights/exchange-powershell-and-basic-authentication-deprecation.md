---
title: Exchange PowerShell i osnovna provjera autentičnosti
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813464"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="5cc1c-102">Exchange PowerShell i osnovna provjera autentičnosti</span><span class="sxs-lookup"><span data-stu-id="5cc1c-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="5cc1c-103">Najnovije informacije o povezivanju sa sustavom Exchange Online PowerShell bez upotrebe osnovne provjere autentičnosti [pronađite ovdje](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="5cc1c-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="5cc1c-104">Modul PowerShell V2 ne upotrebljava osnovnu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="5cc1c-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="5cc1c-105">Imajte na umu da osnovna provjera autentičnosti još uvijek mora biti omogućena na klijentskom uređaju.</span><span class="sxs-lookup"><span data-stu-id="5cc1c-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="5cc1c-106">Novi modul PowerShell V2 koristi modernu provjeru autentičnosti kako bi uspostavio vezu i omogućio sve V2 cmdlete koji se oslanjaju na REST.</span><span class="sxs-lookup"><span data-stu-id="5cc1c-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="5cc1c-107">Osim V2 cmdleta, on vam omogućuje i pristup starijim cmdletima za Remote PowerShell (RPS) za koje je potrebno uspostaviti sesiju ljuske Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5cc1c-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="5cc1c-108">Uspostavljanje RPS sesije na računalu sa sustavom Windows zahtijeva da se na klijentskom računalu omogući WinRM BasicAuth čak i u slučaju da za provjeru autentičnosti prilikom pristupanja servisu modul koristi mehanizam moderne provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="5cc1c-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="5cc1c-109">Za prijenos tokena moderne provjere autentičnosti koristi se komunikacijski kanal provjere autentičnosti WinRM Basic.</span><span class="sxs-lookup"><span data-stu-id="5cc1c-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="5cc1c-110">Ako je provjera autentičnosti WinRM Basic onemogućena na klijentskom računalu, novi će V2 cmdleti i dalje funkcionirati (no stariji RPS cmdleti neće).</span><span class="sxs-lookup"><span data-stu-id="5cc1c-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
