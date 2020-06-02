---
title: Nije moguće izbrisati stavke u sustavu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511968"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="732de-102">Nije moguće izbrisati stavke</span><span class="sxs-lookup"><span data-stu-id="732de-102">Unable to delete items</span></span>

<span data-ttu-id="732de-103">Pravila zadržavanja mogu uzrokovati to, morate onemogućiti ili isključiti odgovarajuće zadržavanje koje uzrokuje taj problem.</span><span class="sxs-lookup"><span data-stu-id="732de-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="732de-104">Nakon uklanjanja pravila zadržavanja ili zadržavanja može biti potrebno do 24 sata da promjena stupi na snagu.</span><span class="sxs-lookup"><span data-stu-id="732de-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="732de-105">Provjerite ne postoji postavljanje [pravila zadržavanja](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) na stavci.</span><span class="sxs-lookup"><span data-stu-id="732de-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="732de-106">Web-mjesto je možda premašilo ograničenje pohrane, povećalo [kvotu web-mjesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisalo stavku.</span><span class="sxs-lookup"><span data-stu-id="732de-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="732de-107">Provjerite nije li stavka [odjavljena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.</span><span class="sxs-lookup"><span data-stu-id="732de-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="732de-108">Naposljetku, administratori mogu koristiti [obrasce i prakse sustava SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koja sadrži biblioteku powershell naredbi koje vam omogućuju izvođenje složenih akcija upravljanja kao što je prisilno brisanje tvrdoglavih stavki.</span><span class="sxs-lookup"><span data-stu-id="732de-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="732de-109">Ukloni PNP datoteku</span><span class="sxs-lookup"><span data-stu-id="732de-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="732de-110">Ukloni PNP mapu</span><span class="sxs-lookup"><span data-stu-id="732de-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="732de-111">Ukloni stavku PNP popisa</span><span class="sxs-lookup"><span data-stu-id="732de-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="732de-112">Ukloni PNP popis</span><span class="sxs-lookup"><span data-stu-id="732de-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="732de-113">Ukloni PNP polje (stupac)</span><span class="sxs-lookup"><span data-stu-id="732de-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)