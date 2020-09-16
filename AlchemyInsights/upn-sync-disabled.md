---
title: Onemogućeno je sinkronizaciju UPN-a
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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749506"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="ec357-102">Onemogućeno je sinkronizaciju UPN-a</span><span class="sxs-lookup"><span data-stu-id="ec357-102">UPN sync disabled</span></span>

<span data-ttu-id="ec357-103">Ako ste pokrenuli sinkronizaciju sa servisom Azure AD prije 30. ožujka 2016, pokrenite sljedeći cmdlet Azure AD PowerShell da biste omogućili UPN meki podudaranje samo za vašu tvrtku ili ustanovu:</span><span class="sxs-lookup"><span data-stu-id="ec357-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="ec357-104">**Set-MsolDirSyncFeature-značajka Enablesoftmatchibirn-Enable $True**</span><span class="sxs-lookup"><span data-stu-id="ec357-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="ec357-105">UPN mekana podudarnost automatski se uključi za tvrtke ili ustanove koje su pokrenule sinkronizaciju sa servisom Azure AD na ili nakon 30. ožujka 2016.</span><span class="sxs-lookup"><span data-stu-id="ec357-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="ec357-106">Da biste saznali više o omogućivanju meke podudaranja na UPN-u i drugim značajkama sinkronizacije, pročitajte [značajke servisa Azure ad Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="ec357-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

