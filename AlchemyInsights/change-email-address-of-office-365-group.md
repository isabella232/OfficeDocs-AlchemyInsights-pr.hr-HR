---
title: Promjena adrese e-pošte grupe sustava Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580649"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="9e9d8-102">Promjena adrese e-pošte grupe sustava Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9e9d8-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="9e9d8-103">Adresu e-pošte grupe microsoft 365 možete promijeniti pomoću centra za administratore.</span><span class="sxs-lookup"><span data-stu-id="9e9d8-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="9e9d8-104">Samo odaberite grupu i odaberite @edit adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="9e9d8-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="9e9d8-105">Možete koristiti i sljedeću naredbu EXO PowerShell da biste promijenili primarnu SMTP adresu grupe microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="9e9d8-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="9e9d8-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="9e9d8-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="9e9d8-107">Primjer:</span><span class="sxs-lookup"><span data-stu-id="9e9d8-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
