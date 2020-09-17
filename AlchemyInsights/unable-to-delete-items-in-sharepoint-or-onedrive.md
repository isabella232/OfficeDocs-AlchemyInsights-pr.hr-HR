---
title: Brisanje stavki u sustavu SharePoint ili na servisu OneDrive nije moguće
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806103"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e2aae-102">Brisanje stavki nije moguće</span><span class="sxs-lookup"><span data-stu-id="e2aae-102">Unable to delete items</span></span>

<span data-ttu-id="e2aae-103">Pravila zadržavanja mogu izazvati to, morate onemogućiti ili isključiti odgovarajuće zadržavanje koje uzrokuje taj problem.</span><span class="sxs-lookup"><span data-stu-id="e2aae-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e2aae-104">Nakon uklanjanja pravilnika o zadržavanju ili zadržavanja, može potrajati i do 24 sata da bi promjena stupila na pamet.</span><span class="sxs-lookup"><span data-stu-id="e2aae-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="e2aae-105">Provjerite ne postoji li postavljanje [pravilnika o zadržavanju](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) na stavci.</span><span class="sxs-lookup"><span data-stu-id="e2aae-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="e2aae-106">Web-mjesto je moglo premašiti ograničenje prostora za pohranu, povećati [kvotu web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisati stavku.</span><span class="sxs-lookup"><span data-stu-id="e2aae-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="e2aae-107">Provjerite nije li stavka [odjavljena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.</span><span class="sxs-lookup"><span data-stu-id="e2aae-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="e2aae-108">Na kraju administratori mogu koristiti [obrasce i prakse sustava SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koji sadrže biblioteku programa PowerShell koje omogućuju obavljanje složenih akcija upravljanja, kao što je prisilno brisanje tvrdoglavih stavki.</span><span class="sxs-lookup"><span data-stu-id="e2aae-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e2aae-109">Uklanjanje PNP datoteke</span><span class="sxs-lookup"><span data-stu-id="e2aae-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e2aae-110">Uklanjanje mape PNP</span><span class="sxs-lookup"><span data-stu-id="e2aae-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e2aae-111">Uklanjanje stavke PNP popisa</span><span class="sxs-lookup"><span data-stu-id="e2aae-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e2aae-112">Uklanjanje PNP popisa</span><span class="sxs-lookup"><span data-stu-id="e2aae-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e2aae-113">Uklanjanje PNP polja (stupca)</span><span class="sxs-lookup"><span data-stu-id="e2aae-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)