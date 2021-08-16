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
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070676"
---
# <a name="change-strong-password-requirement"></a>Promjena preduvjeta za jaku lozinku

Microsoft po zadanom zahtijeva jake lozinke.

Pomoću komponente PowerShell možete onemogućiti jake lozinke za određene korisnike pomoću ovih naredbi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Da biste onemogućili jake lozinke za sve korisnike, koristite sljedeće:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Dodatne informacije o pravilniku za lozinke](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Povezivanje s Microsoft 365 ljuskom PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Dodatne informacije o naredbama komponente PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
