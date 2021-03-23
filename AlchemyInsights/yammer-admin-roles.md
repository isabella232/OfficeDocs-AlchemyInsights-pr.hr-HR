---
title: O administratorima servisa Yammer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2021
ms.locfileid: "51035237"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="06197-102">O administratorima servisa Yammer</span><span class="sxs-lookup"><span data-stu-id="06197-102">About Yammer admins</span></span>

<span data-ttu-id="06197-103">**Administratori mreže**</span><span class="sxs-lookup"><span data-stu-id="06197-103">**Network admins**</span></span>

<span data-ttu-id="06197-104">Globalni administratori automatski se promoviraju u ulogu verificirane administracije u mreži servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="06197-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="06197-105">U sljedećim slučajevima ova se promocija možda neće ispravno pojaviti:</span><span class="sxs-lookup"><span data-stu-id="06197-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="06197-106">Postoji više mreža servisa Yammer, a administrator je potpisan u pogrešnu.</span><span class="sxs-lookup"><span data-stu-id="06197-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="06197-107">Da biste dobili neku mrežu servisa Yammer, potrebna je [Mrežna konsolidacija](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) .</span><span class="sxs-lookup"><span data-stu-id="06197-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="06197-108">Koristi se Azure PIM.</span><span class="sxs-lookup"><span data-stu-id="06197-108">Azure PIM is being used.</span></span> <span data-ttu-id="06197-109">Korisnik možda neće biti unaprijeđen u Global admin dovoljno dugo da se promocija pojavi.</span><span class="sxs-lookup"><span data-stu-id="06197-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="06197-110">Buduće ažuriranje za Yammer može riješiti taj problem, no najbolje je ručno promicati korisnike u globalnom administratore.</span><span class="sxs-lookup"><span data-stu-id="06197-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="06197-111">U mreži servisa Yammer postoji problem s sinkronizacijom.</span><span class="sxs-lookup"><span data-stu-id="06197-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="06197-112">U ovom slučaju zahtjev za podršku bit će obavezan za daljnju istragu.</span><span class="sxs-lookup"><span data-stu-id="06197-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="06197-113">Dodatne informacije o ulogama administratora servisa Yammer potražite u članku [Upravljanje administratorima servisa Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="06197-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="06197-114">**Administratori grupe**</span><span class="sxs-lookup"><span data-stu-id="06197-114">**Group admins**</span></span>

<span data-ttu-id="06197-115">Administratori grupe za Microsoft 365 povezane grupe sinkroniziraju se s članstvom grupe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="06197-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="06197-116">Za velike grupe ova sinkronizacija može potrajati dulje vrijeme.</span><span class="sxs-lookup"><span data-stu-id="06197-116">For large groups, this sync can take an extended period.</span></span>
