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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233509"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="d714f-102">Implementacija dodataka za Microsoft 365 Apps</span><span class="sxs-lookup"><span data-stu-id="d714f-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="d714f-103">Centralizirana implementacija preporučeni je način implementacije Office dodataka korisnicima i grupama u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="d714f-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="d714f-104">Da biste implementirati dodatke, slijedite korake u nastavku:</span><span class="sxs-lookup"><span data-stu-id="d714f-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="d714f-105">**Napomena:** Da biste instalirali dodatke za Office kao pojedinačnog korisnika, pogledajte prikaz dodataka, upravljanje njima i [instalaciju Office programima](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span><span class="sxs-lookup"><span data-stu-id="d714f-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="d714f-106">Osim toga, provjerite je li omogućeno Office pojedinačnih dodataka trgovine Store.</span><span class="sxs-lookup"><span data-stu-id="d714f-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="d714f-107">Detalje potražite u članku Sprječavanje preuzimanja dodataka tako da isključite Office trgovine u svim [klijentima (osim Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="d714f-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="d714f-108">Provjerite ispunjava li vaše okruženje preduvjete za implementaciju dodataka pomoću centralizirane implementacije.</span><span class="sxs-lookup"><span data-stu-id="d714f-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="d714f-109">Detalje potražite u odjeljku [Preduvjeti](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="d714f-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="d714f-110">Idite **na Postavke**  >  **integrirane**  >  **aplikacije Nabavite aplikacije** u centru Microsoft 365 za administratore da biste implementirani dodatke.</span><span class="sxs-lookup"><span data-stu-id="d714f-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="d714f-111">Napomene:</span><span class="sxs-lookup"><span data-stu-id="d714f-111">Notes:</span></span> 

- <span data-ttu-id="d714f-112">Integrirane aplikacije zahtijevaju da administrator ima dozvole globalnog administratora Exchange administratora.</span><span class="sxs-lookup"><span data-stu-id="d714f-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="d714f-113">Prilikom implementacije dodataka na više korisnika preporučujemo da zadatke postavite pomoću grupa umjesto pojedinačnih korisnika.</span><span class="sxs-lookup"><span data-stu-id="d714f-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="d714f-114">Detalje potražite u [članku Razmatranja prilikom dodjele dodatka korisnicima i grupama](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="d714f-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="d714f-115">Centralizirana implementacija ne podržava korisnike u ugniježđenim grupama ili grupama koje imaju nadređene grupe.</span><span class="sxs-lookup"><span data-stu-id="d714f-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="d714f-116">Detalje potražite u članku [Korisnički i grupni zadaci](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="d714f-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="d714f-117">Provjerite je li Microsoft 365 servis za upravljanje aplikacijama (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogućen za prijavu.</span><span class="sxs-lookup"><span data-stu-id="d714f-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="d714f-118">Detalje potražite u članku [Konfiguriranje svojstava aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="d714f-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="d714f-119">Ako se pojave problemi prilikom implementacije dodataka pomoću integriranih aplikacija, pokušajte implementirati pomoću [dodataka](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="d714f-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="d714f-120">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="d714f-120">For more information, see:</span></span>

<span data-ttu-id="d714f-121">[Implementacija dodataka u centru za administratore](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje dodacima u centru za administratore](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Upravljanje dodacima pomoću cmdleta komponente PowerShell za centraliziranu implementaciju](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Objavljivanje Office dodataka pomoću centralizirane implementacije putem centra za Microsoft 365 administratore](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Otklanjanje poteškoća: korisnik ne vidi dodatke](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Otklanjanje poteškoća s Office dodacima](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="d714f-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>