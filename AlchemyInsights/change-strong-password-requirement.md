---
title: Promjena preduvjeta za jaku lozinku
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818460"
---
# <a name="change-strong-password-requirement"></a>Promjena preduvjeta za jaku lozinku

Microsoft po zadanom zahtijeva jake lozinke.

Pomoću komponente PowerShell možete onemogućiti jake lozinke za određene korisnike pomoću ovih naredbi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Da biste onemogućili jake lozinke za sve korisnike, koristite sljedeće:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Dodatne informacije o pravilniku za lozinke](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Povezivanje sa sustavom Microsoft 365 pomoću komponente PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Dodatne informacije o naredbama komponente PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
