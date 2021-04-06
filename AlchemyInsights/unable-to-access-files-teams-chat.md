---
title: Nije moguće pristupiti datotekama koje se zajednički koriste u čavrljanja aplikacije Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51595501"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="e1fa1-102">Nije moguće pristupiti datotekama koje se zajednički koriste u čavrljanja aplikacije Teams</span><span class="sxs-lookup"><span data-stu-id="e1fa1-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="e1fa1-103">U aplikaciji Microsoft Teams datoteka koju korisnik zajednički koristi u prozoru čavrljanja automatski se pohranjuje na web-mjestu servisa OneDrive korisnika za zajedničko korištenje.</span><span class="sxs-lookup"><span data-stu-id="e1fa1-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="e1fa1-104">Kada drugi korisnik pokuša otvoriti datoteku u aplikaciji Teams i primi poruku o pogrešci "Nemate pristup ovoj datoteci", problem se pojavljuje jer je značajka zaključavanja korisničkih dozvola ograničenog pristupa aktivirana na web-mjestu servisa OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e1fa1-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="e1fa1-105">Upute za onemogućivanje značajke na web-mjestu servisa OneDrive potražite u članku [Pogreška prilikom otvaranja datoteke u aplikaciji Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span><span class="sxs-lookup"><span data-stu-id="e1fa1-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="e1fa1-106">Provjerite ima li drugi korisnik pristup web-mjestu servisa OneDrive i omogućite pristup slijedeći upute u sustavu [Share OneDrive datoteke i mape](https://go.microsoft.com/fwlink/?linkid=2156017).</span><span class="sxs-lookup"><span data-stu-id="e1fa1-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>