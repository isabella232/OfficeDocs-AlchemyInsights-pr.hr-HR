---
title: Promjena potrebe za jakom lozinkom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804415"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="9815b-102">Promjena potrebe za jakom lozinkom</span><span class="sxs-lookup"><span data-stu-id="9815b-102">Change strong password requirement</span></span>

<span data-ttu-id="9815b-103">Za Microsoft je po zadanom potrebna snažna lozinka.</span><span class="sxs-lookup"><span data-stu-id="9815b-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="9815b-104">Pomoću komponente PowerShell možete onemogućiti snažne lozinke za određene korisnike ovim naredbama:</span><span class="sxs-lookup"><span data-stu-id="9815b-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="9815b-105">Da biste onemogućili jake lozinke za sve korisnike, koristite:</span><span class="sxs-lookup"><span data-stu-id="9815b-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="9815b-106">Dodatne informacije o pravilniku o lozinci</span><span class="sxs-lookup"><span data-stu-id="9815b-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="9815b-107">Povezivanje s Microsoftovim 365 pomoću komponente PowerShell</span><span class="sxs-lookup"><span data-stu-id="9815b-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="9815b-108">Dodatne informacije o naredbama Msolusera za PowerShell</span><span class="sxs-lookup"><span data-stu-id="9815b-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
