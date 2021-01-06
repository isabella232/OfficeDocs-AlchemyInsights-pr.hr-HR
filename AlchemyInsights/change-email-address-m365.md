---
title: Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756549"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="71017-102">Promijenite adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="71017-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="71017-103">Možete promijeniti adresu e-pošte grupe sustava Microsoft 365 ili aplikacije Microsoft Teams uz pomoć [Centra za administratore okruženja Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="71017-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="71017-104">Samo odaberite grupu i @uredite adresu e-pošte.</span><span class="sxs-lookup"><span data-stu-id="71017-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="71017-105">Možete upotrijebiti i sljedeću naredbu EXO PowerShell za promjenu primarne SMTP adrese grupe sustava Microsoft 365/aplikacije Teams:</span><span class="sxs-lookup"><span data-stu-id="71017-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="71017-106">Primjer:</span><span class="sxs-lookup"><span data-stu-id="71017-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
