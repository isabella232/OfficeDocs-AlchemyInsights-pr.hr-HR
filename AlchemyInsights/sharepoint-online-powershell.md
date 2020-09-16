---
title: PowerShell sustava SharePoint Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770831"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="e0f9e-102">PowerShell sustava SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e0f9e-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="e0f9e-103">Rad s pomoću komponente PowerShell ili skripte u sustavu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="e0f9e-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="e0f9e-104">Dodatne informacije potražite u nastavku.</span><span class="sxs-lookup"><span data-stu-id="e0f9e-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="e0f9e-105">Početak rada s ljuskom za upravljanje sustavom SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e0f9e-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="e0f9e-106">Povezivanje sa sustavom SPO PowerShell s višestrukim čimbenikom za provjeru autentičnosti (MFA)</span><span class="sxs-lookup"><span data-stu-id="e0f9e-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="e0f9e-107">[Obrasci i prakse sustava SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrže biblioteku programa PowerShell koje omogućuju obavljanje složenih akcija upravljanja prema SPO-u.</span><span class="sxs-lookup"><span data-stu-id="e0f9e-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="e0f9e-108">Ako imate problema s povezivanjem s ljuskom za upravljanje SPO-om, provjerite jeste li ažurirali najnoviju verziju i pokušajte [ponovno uvesti modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomoću značajke *"Import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="e0f9e-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="e0f9e-109">Ako pokušavate pokretati klijentske skripte objektnog modela, na lokalnom ćete računalu morati imati instaliran SDK za [klijentske komponente sustava SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="e0f9e-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="e0f9e-110">Ako imate problema s pokretanjem skripti iz komponente PowerShell, možete razmotriti pokretanje komponente PowerShell kao administratora i promjena [pravilnika o izvršenju](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="e0f9e-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>