---
title: Upravljanje globalnim popisom adresa tvrtke ili ustanove i izvanmrežnim adresarom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022439"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="41ab5-102">Upravljanje globalnim popisom adresa tvrtke ili ustanove (GAL) i izvanmrežnim adresarom (OAB)</span><span class="sxs-lookup"><span data-stu-id="41ab5-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="41ab5-103">Globalni popis adresa (GAL) popis je objekata s omogućenom e-poštom (svih vrsta primatelja koji mogu primati e-poštu) u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="41ab5-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="41ab5-104">Jedan se GAL automatski stvara u svakoj tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="41ab5-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="41ab5-105">Možete stvarati dodatne GAL-ove da biste razdvojili korisnike po tvrtki ili ustanovi ili mjestu, ali jedan korisnik može istodobno vidjeti i koristiti samo jedan GAL.</span><span class="sxs-lookup"><span data-stu-id="41ab5-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="41ab5-106">Neki klijenti za e-poštu, kao što je Outlook za Windows, preuzimaju GAL za izvanmrežni rad.</span><span class="sxs-lookup"><span data-stu-id="41ab5-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="41ab5-107">To je poznato kao izvanmrežni adresar (OAB).</span><span class="sxs-lookup"><span data-stu-id="41ab5-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="41ab5-108">U sustavu Exchange online OAB se ažurira samo jedanput svakih 8 sati, a potom ga klijenti moraju preuzeti da bi ažurirali svoju lokalnu kopiju OAB-a.</span><span class="sxs-lookup"><span data-stu-id="41ab5-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="41ab5-109">Svaka promjena primatelja mora najprije biti vidljiva u GAL-u da bi se kasnije mogla prenijeti u OAB.</span><span class="sxs-lookup"><span data-stu-id="41ab5-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="41ab5-110">Evo nekoliko uobičajenih postupaka koji se koriste za GAL i OAB:</span><span class="sxs-lookup"><span data-stu-id="41ab5-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="41ab5-111">Zbog niza razloga dobro je sakriti neke objekte od GAL-a.</span><span class="sxs-lookup"><span data-stu-id="41ab5-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="41ab5-112">Pročitajte članak [Sakrivanje primatelja od popisa adresa](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="41ab5-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="41ab5-113">Ako trebate pojedinim grupama korisnika omogućiti prilagođene prikaze GAL-a tvrtke ili ustanove, pročitajte članak [Pravilnici za adresare u sustavu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="41ab5-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="41ab5-114">[Stvorite globalni popis adresa u sustavu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), a da biste saznali kako raditi s dozvolama za GAL, pročitajte članak [Popisi adresa u sustavu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="41ab5-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="41ab5-115">Imajte na umu da je, ako stvarate nove GAL-ove, dobro stvoriti i novi OAB.</span><span class="sxs-lookup"><span data-stu-id="41ab5-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="41ab5-116">Pročitajte članak [Postupci s izvanmrežnim adresarom](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="41ab5-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
