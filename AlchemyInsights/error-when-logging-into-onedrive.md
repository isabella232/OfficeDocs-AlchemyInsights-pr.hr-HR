---
title: 0x8004de40 prilikom pokretanja servisa OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813644"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="ef2e9-102">0x8004de40 prilikom pokretanja servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="ef2e9-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="ef2e9-103">Ako vam se prilikom 0x8004de40 **na** OneDrive prikazuje pogreška, ponovno pokrenite računalo dok ste povezani s domenom tvrtke ili škole.</span><span class="sxs-lookup"><span data-stu-id="ef2e9-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="ef2e9-104">Ako se ta pogreška pojavi nakon ponovnog pokretanja, pokušajte to dok ste povezani s domenom na poslu ili u školi:</span><span class="sxs-lookup"><span data-stu-id="ef2e9-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="ef2e9-105">Kliknite Start, a zatim  u okvir za pretraživanje upišite **cmd** ili naredbeni redak, desnom tipkom miša kliknite aplikaciju naredbenog retka, a zatim **odaberite Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="ef2e9-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="ef2e9-106">Ako se od vas zatraži da upišete administratorsku lozinku ili potvrdu, upišite lozinku ili kliknite **Dopusti**.</span><span class="sxs-lookup"><span data-stu-id="ef2e9-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="ef2e9-107">U prozor naredbenog retka upišite **dsregcmd /leave**  i pričekajte da se naredba dovrši.</span><span class="sxs-lookup"><span data-stu-id="ef2e9-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="ef2e9-108">Zatim **upišite dsregcmd /join** i pričekajte da se naredba dovrši.</span><span class="sxs-lookup"><span data-stu-id="ef2e9-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="ef2e9-109">Ponovno pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="ef2e9-109">Reboot your computer.</span></span>
