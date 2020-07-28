---
title: Nije moguće promijeniti Korisničko ime
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438887"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="b7d80-102">Nije moguće promijeniti Korisničko ime</span><span class="sxs-lookup"><span data-stu-id="b7d80-102">Unable to change UserName</span></span>

<span data-ttu-id="b7d80-103">U nekim slučajevima promjene UPN (UserPrincipalName) nisu propagirane u oblak.</span><span class="sxs-lookup"><span data-stu-id="b7d80-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="b7d80-104">Možda ćete primiti pogreške provjere valjanosti na portalu sustava Office 365 ili ne možete promijeniti korisničko ime ili adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="b7d80-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="b7d80-105">Da biste riješili taj problem, ručno postavite UserPrincipalName pomoću ove naredbe PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b7d80-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="b7d80-106">**Primjer: Preimenovanje korisnika**</span><span class="sxs-lookup"><span data-stu-id="b7d80-106">**Example: Rename a user**</span></span>

<span data-ttu-id="b7d80-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="b7d80-107">PowerShellCopy</span></span>

<span data-ttu-id="b7d80-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="b7d80-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="b7d80-109">Ova naredba davidc@contoso.com preimenuje u davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="b7d80-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="b7d80-110">Dodatne informacije potražite [u odjeljku Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="b7d80-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>