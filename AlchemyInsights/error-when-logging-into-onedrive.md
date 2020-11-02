---
title: 0x8004de40 pogreška prilikom pokretanja servisa OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48822999"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="9f20b-102">0x8004de40 pogreška prilikom pokretanja servisa OneDrive</span><span class="sxs-lookup"><span data-stu-id="9f20b-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="9f20b-103">Ako se prilikom prijave na OneDrive pojavi pogreška **0x8004de40** , ponovno pokrenite računalo dok ste povezani s domenom rada ili škole.</span><span class="sxs-lookup"><span data-stu-id="9f20b-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="9f20b-104">Ako se ta pogreška pojavi nakon ponovnog pokretanja, isprobajte ovo dok ste spojeni na domenu rada ili škole:</span><span class="sxs-lookup"><span data-stu-id="9f20b-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="9f20b-105">Kliknite Start, a zatim u okvir za pretraživanje upišite **cmd** ili **naredbeni upit**  , desnom tipkom miša kliknite aplikaciju naredbenog upita, a zatim odaberite  **Pokreni kao administrator** .</span><span class="sxs-lookup"><span data-stu-id="9f20b-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="9f20b-106">Ako se od vas zatraži administratorska lozinka ili potvrda, upišite lozinku ili kliknite **Dopusti** .</span><span class="sxs-lookup"><span data-stu-id="9f20b-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="9f20b-107">U prozoru naredbenog upita upišite **dsregcmd/ostavite**  i pričekajte da se naredba dovrši.</span><span class="sxs-lookup"><span data-stu-id="9f20b-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="9f20b-108">Zatim upišite **dsregcmd/pridružite** se i pričekajte da se naredba dovrši.</span><span class="sxs-lookup"><span data-stu-id="9f20b-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="9f20b-109">Ponovno pokrenite računalo.</span><span class="sxs-lookup"><span data-stu-id="9f20b-109">Reboot your computer.</span></span>
