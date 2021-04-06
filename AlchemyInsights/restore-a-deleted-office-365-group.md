---
title: Vraćanje izbrisane grupe sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597435"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="ec398-102">Vraćanje izbrisane grupe sustava Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ec398-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="ec398-103">Izbrisanu grupu sustava Microsoft 365 ili Microsoft Teams možete vratiti u roku od 30 dana od brisanja.</span><span class="sxs-lookup"><span data-stu-id="ec398-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="ec398-104">Idite u [centar za administratore sustava Microsoft 365](https://aka.ms/RestoreDeletedGroup) da biste se prijavite i na popisu popisa izbrisanih grupa i timova.</span><span class="sxs-lookup"><span data-stu-id="ec398-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="ec398-105">**Napomena:** Prijavite se pomoću računa dodijeljenog administratoru klijenta ili administratoru grupe.</span><span class="sxs-lookup"><span data-stu-id="ec398-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="ec398-106">Odaberite izbrisanu grupu microsoft 365/Teams koju želite vratiti i kliknite **vrati grupu**.</span><span class="sxs-lookup"><span data-stu-id="ec398-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="ec398-107">Ako grupu nije moguće vratiti zbog smtp adrese koja je u sukobu, pomoću sljedeće naredbe pronađite objekt koji uzrokuje sukob i uklonite SMTP adresu:</span><span class="sxs-lookup"><span data-stu-id="ec398-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="ec398-108">**Napomena:** U nekim slučajevima može potrajati i do 24 sata da se grupa i svi njezini podaci vrate.</span><span class="sxs-lookup"><span data-stu-id="ec398-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="ec398-109">Dodatne informacije ili upute za vraćanje grupa pomoću komponente PowerShell potražite u članku [Vraćanje izbrisane grupe sustava Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).</span><span class="sxs-lookup"><span data-stu-id="ec398-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>