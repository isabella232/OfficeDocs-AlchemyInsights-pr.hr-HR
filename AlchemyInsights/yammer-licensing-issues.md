---
title: Problemi s licenciranjem servisa Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148180"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="af71f-102">Problemi s licenciranjem servisa Yammer</span><span class="sxs-lookup"><span data-stu-id="af71f-102">Yammer licensing issues</span></span>

<span data-ttu-id="af71f-103">Svi korisnici moraju imati licencu za korištenje servisa Yammer Enterprise, ali na zadanom servis Yammer ne zahtijeva da korisnici imaju licencu za pristup servisu.</span><span class="sxs-lookup"><span data-stu-id="af71f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="af71f-104">Kada administrator promijeni postavku da blokira korisnike sustava Microsoft 365 bez licenci servisa Yammer, korisnicima koji nisu dodijeljeni licenci za Yammer Enterprise ne mogu pristupiti servisu servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="af71f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="af71f-105">Dodatne informacije [potražite u članku Upravljanje korisničkim licencama servisa Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="af71f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="af71f-106">Kada se licence uklanjaju iz korisnika, pločica servisa Yammer više se ne prikazuje, a drugi servisi mogu koristiti uklanjanje licenci da bi sakrili značajke.</span><span class="sxs-lookup"><span data-stu-id="af71f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="af71f-107">U drugim slučajevima značajke se i dalje mogu pojaviti, ali zahtijevaju da dodjela dozvola radi.</span><span class="sxs-lookup"><span data-stu-id="af71f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="af71f-108">**Licenca se ne ažurira za korisnika**</span><span class="sxs-lookup"><span data-stu-id="af71f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="af71f-109">Korisniku se povremeno dodjeljuje licenca, ali i dalje ne može pristupiti servisu Yammer.</span><span class="sxs-lookup"><span data-stu-id="af71f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="af71f-110">Veća je vjerojatnost da će doći do kašnjenja kada je dodjela masovne licence u tijeku.</span><span class="sxs-lookup"><span data-stu-id="af71f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="af71f-111">Korisnici servisa Yammer možda se neće ažurirati istim redoslijedom kao i licence u azure AD jer sustav izvodi asinkrono.</span><span class="sxs-lookup"><span data-stu-id="af71f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="af71f-112">Pričekajte do 24 sata prije otvaranja slučaja podrške da biste prijavili probleme sa sinkronizacijom licence.</span><span class="sxs-lookup"><span data-stu-id="af71f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="af71f-113">**Dodjela skupne dozvole**</span><span class="sxs-lookup"><span data-stu-id="af71f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="af71f-114">Licence se mogu dodijeliti putem centra za administratore ili skriptiranja u powershellu.</span><span class="sxs-lookup"><span data-stu-id="af71f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="af71f-115">Dodatne informacije potražite u članku [Dodjela licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [Dodjela licenci korisničkim računima pomoću komponente Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="af71f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="af71f-116">Microsoftova podrška ne pruža pomoć pri stvaranju skripti, ali dostupna je dokumentacija o dodjeli licence za Yammer.</span><span class="sxs-lookup"><span data-stu-id="af71f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="af71f-117">Dodatne informacije [potražite u odjeljku Upravljanje licencama za Yammer pomoću komponente Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="af71f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>