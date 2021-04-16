---
title: Šifriranje s pomoću pravila prijenosa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813860"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="05849-102">Šifriranje s pomoću pravila prijenosa</span><span class="sxs-lookup"><span data-stu-id="05849-102">Encryption with transport rules</span></span>

<span data-ttu-id="05849-103">Da biste pokrenuli šifriranje poruka, u [centru za administratore sustava Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) možete se koristiti mogućnostima šifriranja poruka u sustavu Office (OME) u pravilima tijeka pošte.</span><span class="sxs-lookup"><span data-stu-id="05849-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="05849-104">Odaberite mogućnost **Primijeni šifriranje poruka u sustavu Office 365 te zaštitu prava** u stanju Pravila prijenosa.</span><span class="sxs-lookup"><span data-stu-id="05849-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="05849-105">Dodatne informacije potražite u članku [Definiranje pravila tijeka pošte za šifriranje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="05849-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="05849-106">U aplikaciji PowerShell upotrijebite cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) i postavite parametar *ApplyOME* na $true.</span><span class="sxs-lookup"><span data-stu-id="05849-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
