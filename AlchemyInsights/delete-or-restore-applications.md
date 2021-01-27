---
title: Brisanje ili vraćanje aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014751"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="83102-102">Brisanje ili vraćanje aplikacija</span><span class="sxs-lookup"><span data-stu-id="83102-102">Delete or restore applications</span></span>

<span data-ttu-id="83102-103">**Da biste izbrisali aplikaciju iz svog stanara Azure ad**:</span><span class="sxs-lookup"><span data-stu-id="83102-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="83102-104">Na **portalu Azure ad** odaberite **Enterprise Applications**.</span><span class="sxs-lookup"><span data-stu-id="83102-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="83102-105">Zatim pronađite i odaberite aplikaciju koju želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="83102-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="83102-106">U odjeljku **Upravljanje** u levom oknu odaberite **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="83102-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="83102-107">Odaberite **Izbriši**, a zatim **da** da biste potvrdili da želite izbrisati aplikaciju iz korisnika Azure AD.</span><span class="sxs-lookup"><span data-stu-id="83102-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="83102-108">Dodatne informacije o tome kako izbrisati aplikaciju potražite u članku [Quickstart: Brisanje aplikacije iz korisnika Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="83102-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="83102-109">U komponenti PowerShell, cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) uklanja konfiguracije proxyja aplikacija iz određene aplikacije u servisu Azure Active Directory i može potpuno izbrisati aplikaciju ako je navedeno.</span><span class="sxs-lookup"><span data-stu-id="83102-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="83102-110">**Izbrisanu aplikaciju možete vratiti** pomoću komponente PowerShell.</span><span class="sxs-lookup"><span data-stu-id="83102-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="83102-111">Kada se aplikacija koju želite vratiti identificira, možete je vratiti pomoću servisa [Vraćanje-azureaddeletedappje](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="83102-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
