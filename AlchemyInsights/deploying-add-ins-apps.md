---
title: Implementacija dodataka za Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124842"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="8dc1c-102">Implementacija dodataka za Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="8dc1c-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="8dc1c-103">Centralizirana implementacija preporučeni je način implementacije Office dodataka korisnicima i grupama u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="8dc1c-104">Da biste implementirati dodatke, slijedite korake u nastavku:</span><span class="sxs-lookup"><span data-stu-id="8dc1c-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="8dc1c-105">**Napomena:** Da biste instalirali dodatke za Office kao pojedinačnog korisnika, pogledajte prikaz dodataka, upravljanje njima i [instalaciju Office programima](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span><span class="sxs-lookup"><span data-stu-id="8dc1c-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="8dc1c-106">Osim toga, provjerite je li omogućeno Office pojedinačnih dodataka trgovine Store.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="8dc1c-107">Provjerite ispunjava li vaše okruženje preduvjete za implementaciju dodataka pomoću centralizirane implementacije.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="8dc1c-108">Detalje potražite u odjeljku [Preduvjeti](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="8dc1c-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="8dc1c-109">Idite **na Postavke**  >  **integrirane**  >  **aplikacije Nabavite aplikacije** u centru Microsoft 365 za administratore da biste implementirani dodatke.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="8dc1c-110">Napomene:</span><span class="sxs-lookup"><span data-stu-id="8dc1c-110">Notes:</span></span> 

- <span data-ttu-id="8dc1c-111">Integrirane aplikacije zahtijevaju da administrator ima dozvole globalnog administratora Exchange administratora.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="8dc1c-112">Prilikom implementacije dodataka na više korisnika preporučujemo da zadatke postavite pomoću grupa umjesto pojedinačnih korisnika.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="8dc1c-113">Detalje potražite u [članku Razmatranja prilikom dodjele dodatka korisnicima i grupama](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="8dc1c-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="8dc1c-114">Centralizirana implementacija ne podržava korisnike u ugniježđenim grupama ili grupama koje imaju nadređene grupe.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="8dc1c-115">Detalje potražite u članku [Korisnički i grupni zadaci](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="8dc1c-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="8dc1c-116">Provjerite je li Microsoft 365 servis za upravljanje aplikacijama (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogućen za prijavu.</span><span class="sxs-lookup"><span data-stu-id="8dc1c-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="8dc1c-117">Detalje potražite u članku [Konfiguriranje svojstava aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="8dc1c-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="8dc1c-118">Ako se pojave problemi prilikom implementacije dodataka pomoću integriranih aplikacija, pokušajte implementirati pomoću [dodataka](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="8dc1c-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="8dc1c-119">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="8dc1c-119">For more information, see:</span></span>

<span data-ttu-id="8dc1c-120">[Implementacija dodataka u centru za administratore](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje dodacima u centru za administratore](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Upravljanje dodacima pomoću cmdleta komponente PowerShell za centraliziranu implementaciju](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Objavljivanje Office dodataka pomoću centralizirane implementacije putem centra za Microsoft 365 administratore](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Otklanjanje poteškoća: korisnik ne vidi dodatke](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Otklanjanje poteškoća s Office dodacima](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="8dc1c-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>