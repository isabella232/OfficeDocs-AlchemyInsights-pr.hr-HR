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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282613"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="5172f-102">Promjena adrese e-pošte grupe sustava Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5172f-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="5172f-103">Adresu e-pošte grupe microsoft 365 možete promijeniti pomoću centra za administratore.</span><span class="sxs-lookup"><span data-stu-id="5172f-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="5172f-104">Samo odaberite grupu i odaberite @edit adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="5172f-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="5172f-105">Možete koristiti i naredbu EXO PowerShell da biste promijenili primarnu SMTP adresu grupe sustava Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="5172f-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="5172f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="5172f-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="5172f-107">Primjer:</span><span class="sxs-lookup"><span data-stu-id="5172f-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
