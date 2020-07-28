---
title: Više objekata ima istu adresu e-pošte kao i identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438801"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="3ddd3-102">Više objekata ima istu adresu e-pošte kao i identitet</span><span class="sxs-lookup"><span data-stu-id="3ddd3-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="3ddd3-103">**Više objekata**</span><span class="sxs-lookup"><span data-stu-id="3ddd3-103">**Multiple objects**</span></span>

<span data-ttu-id="3ddd3-104">Jedan od uobičajenih razloga ove pogreške nije u mogućnosti ispravno usmjeriti zahtjev za Outlook Web Access u prisutnosti više objekata koji imaju istu adresu e-pošte kao i identitet.</span><span class="sxs-lookup"><span data-stu-id="3ddd3-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="3ddd3-105">Da biste pronašli te objekte, pokrenite sljedeće naredbe:</span><span class="sxs-lookup"><span data-stu-id="3ddd3-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="3ddd3-106">· Primatelja<email address></span><span class="sxs-lookup"><span data-stu-id="3ddd3-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="3ddd3-107">· Get-User<email address></span><span class="sxs-lookup"><span data-stu-id="3ddd3-107">· Get-User <email address></span></span>

<span data-ttu-id="3ddd3-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="3ddd3-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="3ddd3-109">· Get-Kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="3ddd3-109">· Get-Contact <email address></span></span>

<span data-ttu-id="3ddd3-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="3ddd3-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="3ddd3-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="3ddd3-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="3ddd3-112">· Get-Mailbox <email address> -InactiveMailboxSamo</span><span class="sxs-lookup"><span data-stu-id="3ddd3-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="3ddd3-113">Da biste riješili problem, uklonite više objekata s istim identitetom e-pošte i provjerite postoji li jedan objekt s određenim identitetom e-pošte i da je vrsta primatelja UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="3ddd3-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="3ddd3-114">**Ista adresa koristi se za poslovne i potrošačke poštanske sandučiće**</span><span class="sxs-lookup"><span data-stu-id="3ddd3-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="3ddd3-115">Drugi uzrok je kada se ista adresa koristi za poslovne i potrošačke poštanske sandučiće.</span><span class="sxs-lookup"><span data-stu-id="3ddd3-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="3ddd3-116">U tom slučaju korisnik mora promijeniti svoj primarni pseudonim za korisnike dok Cafe ne podržava ovaj scenarij.</span><span class="sxs-lookup"><span data-stu-id="3ddd3-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="3ddd3-117">To je trajna pogreška koja ne prolazi bez intervencije.</span><span class="sxs-lookup"><span data-stu-id="3ddd3-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="3ddd3-118">Pojedinosti potražite [u odjeljku Promjena adrese e-pošte ili telefonskog broja microsoftova računa](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="3ddd3-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>