---
title: Vraćanje izbrisane datoteke ili mape
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797540"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="68dcc-102">Vraćanje izbrisane datoteke ili mape</span><span class="sxs-lookup"><span data-stu-id="68dcc-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="68dcc-103">SharePoint Online zadržava sigurnosne kopije cjelokupnog sadržaja 14 dodatnih dana nakon stvarnog brisanja.</span><span class="sxs-lookup"><span data-stu-id="68dcc-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="68dcc-104">Ako se sadržaj ne može vratiti putem koša za smeće ili vraćanja datoteka, administrator se može obratiti Microsoftovoj podršci da bi zahtijevao vraćanje u bilo kojem trenutku u prozoru 14 dana.</span><span class="sxs-lookup"><span data-stu-id="68dcc-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="68dcc-105">Vraćanja iz sigurnosnih kopija mogu se dovršiti samo za zbirke web-mjesta ili podstranice, a ne za pojedinačne datoteke, popise ni biblioteke.</span><span class="sxs-lookup"><span data-stu-id="68dcc-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="68dcc-106">Kada izbrišete stavku ili web-mjesto iz sustava SharePoint, ona se ne uklanja odmah.</span><span class="sxs-lookup"><span data-stu-id="68dcc-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="68dcc-107">Izbrisane stavke premještaju se u koš za smeće na određeno vrijeme.</span><span class="sxs-lookup"><span data-stu-id="68dcc-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="68dcc-108">Tijekom toga vremena možete vratiti stavke koje ste izbrisali na njihovu izvornu lokaciju.</span><span class="sxs-lookup"><span data-stu-id="68dcc-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="68dcc-109">Da biste saznali više, posjetite poveznice u nastavku.</span><span class="sxs-lookup"><span data-stu-id="68dcc-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="68dcc-110">[Vraćanje stavki u koš za smeće web-mjesta sustava SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="68dcc-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="68dcc-111">Vraćanje izbrisanih datoteka ili mapa na servisu OneDrive</span><span class="sxs-lookup"><span data-stu-id="68dcc-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="68dcc-112">Vraćanje izbrisane zbirke web-mjesta (uključujući grupu, komunikaciju i druga web-mjesta)</span><span class="sxs-lookup"><span data-stu-id="68dcc-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="68dcc-113">Vraćanje izbrisanog web-mjesta servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="68dcc-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="68dcc-114">Da bi se u nastavku skupnih akcija koša za smeće, administratori mogu razmotriti pomoću [sustava SharePoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="68dcc-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="68dcc-115">**Značajka vraćanja datoteka**</span><span class="sxs-lookup"><span data-stu-id="68dcc-115">**Files Restore feature**</span></span>

<span data-ttu-id="68dcc-116">Ako se mnogo datoteka sa servisa OneDrive ili sustava SharePoint izbriše, briše, ošteti ili inficira zlonamjernim softverom, možete vratiti cijelu biblioteku servisa OneDrive ili SharePoint u prethodno razdoblje pomoću značajke vraćanja datoteka.</span><span class="sxs-lookup"><span data-stu-id="68dcc-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="68dcc-117">Vraćanje biblioteke servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="68dcc-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="68dcc-118">Vraćanje biblioteke dokumenata</span><span class="sxs-lookup"><span data-stu-id="68dcc-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

