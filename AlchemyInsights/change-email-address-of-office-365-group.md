---
title: Promjena adrese e-pošte grupe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733679"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="aed38-102">Promjena adrese e-pošte grupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="aed38-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="aed38-103">Adresu e-pošte grupe Microsoft 365 možete promijeniti pomoću centra za administratore.</span><span class="sxs-lookup"><span data-stu-id="aed38-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="aed38-104">Samo odaberite grupu pa odaberite @edit adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="aed38-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="aed38-105">Možete koristiti i sljedeće naredbe EXO PowerShell da biste promijenili primarnu SMTP adresu grupe Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="aed38-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="aed38-106">Set-UnifiedGroup <Group Name> -primarni ysmtpaddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="aed38-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="aed38-107">Primjer</span><span class="sxs-lookup"><span data-stu-id="aed38-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
