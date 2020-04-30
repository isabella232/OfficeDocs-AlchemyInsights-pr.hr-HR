---
title: Šifriranje s pomoću pravila prijenosa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915043"
---
# <a name="encryption-with-transport-rules"></a>Šifriranje s pomoću pravila prijenosa

Da biste pokrenuli šifriranje poruka, u [centru za administratore sustava Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) možete se koristiti mogućnostima šifriranja poruka u sustavu Office (OME) u pravilima tijeka pošte. Odaberite mogućnost **Primijeni šifriranje poruka u sustavu Office 365 te zaštitu prava** u stanju Pravila prijenosa.

- Dodatne informacije potražite u članku [Definiranje pravila tijeka pošte za šifriranje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- U aplikaciji PowerShell upotrijebite cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) i postavite parametar *ApplyOME* na $true.
