---
title: Prepoznavanje problema s virtualnom radnom površinom sustava Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595513"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="344ab-102">Prepoznavanje problema s virtualnom radnom površinom sustava Windows</span><span class="sxs-lookup"><span data-stu-id="344ab-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="344ab-103">Dijagnostika virtualne radne površine sustava Windows koristi samo jedan cmdlet komponente PowerShell, ali sadrži brojne neobavezne parametre za sužavanje i izoliranje problema.</span><span class="sxs-lookup"><span data-stu-id="344ab-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="344ab-104">Da biste započeli s radom:</span><span class="sxs-lookup"><span data-stu-id="344ab-104">To get started:</span></span> 

1. <span data-ttu-id="344ab-105">Preuzmite i uvezite modul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="344ab-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="344ab-106">Detalje potražite u članku [Cmdleti virtualne radne površine sustava Windows za Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="344ab-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="344ab-107">Pokrenite sljedeći cmdlet da biste se prijavili na račun:</span><span class="sxs-lookup"><span data-stu-id="344ab-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="344ab-108">Primjer: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="344ab-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="344ab-109">**NAPOMENA:** Svi upiti koji koriste PowerShell moraju obuhvaćati parametre -UserName ili -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="344ab-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="344ab-110">Mogućnosti nadzora pogledajte u članku Korištenje [analitike zapisnika za značajku dijagnostike](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="344ab-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="344ab-111">Da biste filtrirali dijagnostičke aktivnosti po korisniku, pokrenite sljedeći cmdlet:</span><span class="sxs-lookup"><span data-stu-id="344ab-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="344ab-112">Primjer: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="344ab-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="344ab-113">Postoji popis filtara koje možete pokrenuti da biste dijagnosticirali probleme.</span><span class="sxs-lookup"><span data-stu-id="344ab-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="344ab-114">Dodatne informacije o dijagnosticiranju problema potražite u članku Prepoznavanje i dijagnosticiranje problema s virtualnom radnom [površinom sustava Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="344ab-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="344ab-115">Dodatne informacije o najčešćim pogreškama potražite u članku [Uobičajene pogreške senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="344ab-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
