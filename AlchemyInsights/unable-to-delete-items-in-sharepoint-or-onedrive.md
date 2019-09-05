---
title: Nije moguće izbrisati stavke u SharePoint ili OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748530"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="4dc0b-102">Nije moguće izbrisati stavke</span><span class="sxs-lookup"><span data-stu-id="4dc0b-102">Unable to delete items</span></span>

<span data-ttu-id="4dc0b-103">Imate li problema brisanje stavki SharePoint?</span><span class="sxs-lookup"><span data-stu-id="4dc0b-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="4dc0b-104">Uvijek provjerite imate li [odgovarajuće dozvole](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) za brisanje artikla ili ste [administrator zbirke web-mjesta](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) pokušaj ukloniti stavku.</span><span class="sxs-lookup"><span data-stu-id="4dc0b-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="4dc0b-105">Provjerite postoji li nije postavljanje [pravila zadržavanja](https://docs.microsoft.com/office365/securitycompliance/retention-policies) na stavku.</span><span class="sxs-lookup"><span data-stu-id="4dc0b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="4dc0b-106">Provjerite je li stavka nije [odjavljen](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.</span><span class="sxs-lookup"><span data-stu-id="4dc0b-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="4dc0b-107">Konačno, administratori mogu koristiti [SharePoint uzorke i postupci](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) koji sadrži biblioteku PowerShell naredbe koje dopuštaju izvođenje složenih upravljanja akcije kao što su prisilno brisanje stubborn stavki.</span><span class="sxs-lookup"><span data-stu-id="4dc0b-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="4dc0b-108">Uklanjanje PNP datoteke</span><span class="sxs-lookup"><span data-stu-id="4dc0b-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="4dc0b-109">Uklanjanje PNP mape</span><span class="sxs-lookup"><span data-stu-id="4dc0b-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="4dc0b-110">Ukloni stavku PNP popisa</span><span class="sxs-lookup"><span data-stu-id="4dc0b-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="4dc0b-111">Uklanjanje PNP popisa</span><span class="sxs-lookup"><span data-stu-id="4dc0b-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="4dc0b-112">Ukloni PNP polje (stupac)</span><span class="sxs-lookup"><span data-stu-id="4dc0b-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)