---
title: Nije moguće pristupiti javnim mapama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891741"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="1fe1d-102">Outlook se ne može povezati s javnim mapama</span><span class="sxs-lookup"><span data-stu-id="1fe1d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="1fe1d-103">Ako pristup javnoj mapi ne funkcionira za neke korisnike, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="1fe1d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="1fe1d-104">Povežite se s EXO PowerShell i konfigurirajte parametar DefaultPublicFolderMailbox na računu problema da odgovara parametru na radnom korisničkom računu.</span><span class="sxs-lookup"><span data-stu-id="1fe1d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="1fe1d-105">Primjer:</span><span class="sxs-lookup"><span data-stu-id="1fe1d-105">Example:</span></span>

<span data-ttu-id="1fe1d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="1fe1d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="1fe1d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<vrijednost iz prethodne naredbe></span><span class="sxs-lookup"><span data-stu-id="1fe1d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="1fe1d-108">Pričekajte najmanje jedan sat da promjena stupi na snagu.</span><span class="sxs-lookup"><span data-stu-id="1fe1d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="1fe1d-109">Ako problem ostane, slijedite [ovaj postupak](https://aka.ms/pfcte) da biste otklonili poteškoće s pristupom javnim mapama pomoću programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="1fe1d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>