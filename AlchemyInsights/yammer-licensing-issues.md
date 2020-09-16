---
title: Problemi s licenciranjem servisa Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657268"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="4667f-102">Problemi s licenciranjem servisa Yammer</span><span class="sxs-lookup"><span data-stu-id="4667f-102">Yammer licensing issues</span></span>

<span data-ttu-id="4667f-103">Svi korisnici moraju imati licencu za korištenje servisa Yammer Enterprise, ali po zadanom Yammer ne zahtijeva da korisnici imaju licencu za pristup servisu.</span><span class="sxs-lookup"><span data-stu-id="4667f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="4667f-104">Kada administrator promijeni postavku da bi blokirao korisnike tvrtke Microsoft 365 bez licenci za Yammer, korisnici koji nisu dodijelili licencu za Yammer Enterprise ne mogu pristupiti servisu Yammer.</span><span class="sxs-lookup"><span data-stu-id="4667f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="4667f-105">Dodatne informacije potražite u članku [Upravljanje korisničkim dozvolama za Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="4667f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="4667f-106">Kada se licence uklanjaju od korisnika, pločica servisa Yammer više se ne prikazuje, a drugi servisi mogu koristiti licencu za uklanjanje za sakrivanje značajki.</span><span class="sxs-lookup"><span data-stu-id="4667f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="4667f-107">U drugim slučajevima značajke se i dalje mogu prikazivati, no potrebna je dodjela licenci za rad.</span><span class="sxs-lookup"><span data-stu-id="4667f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="4667f-108">**Licenca nije ažurirana za korisnika**</span><span class="sxs-lookup"><span data-stu-id="4667f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="4667f-109">Korisniku se povremeno dodjeljuje licenca, ali i dalje ne može pristupiti servisu Yammer.</span><span class="sxs-lookup"><span data-stu-id="4667f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="4667f-110">Veća je vjerojatnost da će kašnjenja nastati kada je u tijeku dodjela licence za masovnu licencu.</span><span class="sxs-lookup"><span data-stu-id="4667f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="4667f-111">Korisnici servisa Yammer možda se neće ažurirati istim redoslijedom kada se licence promijene u servisu Azure AD jer sustav radi asinkrono.</span><span class="sxs-lookup"><span data-stu-id="4667f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="4667f-112">Pričekajte do 24 sata prije otvaranja slučaja podrške da biste prijavili probleme s sinkronizacijom licenci.</span><span class="sxs-lookup"><span data-stu-id="4667f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="4667f-113">**Dodjela skupnih dozvola**</span><span class="sxs-lookup"><span data-stu-id="4667f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="4667f-114">Licence se mogu dodijeliti putem centra za administratore ili skripte za PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4667f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="4667f-115">Dodatne informacije potražite u članku [dodjeljivanje licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [dodjeljivanje licenci korisničkim računima pomoću komponente Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="4667f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="4667f-116">Microsoftova podrška ne nudi pomoć za stvaranje skripti, ali je dostupna dokumentacija na dodjeli licenci za Yammer.</span><span class="sxs-lookup"><span data-stu-id="4667f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="4667f-117">Dodatne informacije potražite u članku [Upravljanje licencama servisa Yammer pomoću komponente Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="4667f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>