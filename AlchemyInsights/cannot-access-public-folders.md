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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959487"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="65eb6-102">Outlook se ne može povezati s javnim mapama</span><span class="sxs-lookup"><span data-stu-id="65eb6-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="65eb6-103">Ako pristup javnim mapama ne funkcionira za nekoliko korisnika, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="65eb6-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="65eb6-104">Povežite se s EXO PowerShell i konfigurirati Defaultpublicfolderpoštanski sandučić na problem korisničkog računa da odgovara jedan na radnom korisničkom računu.</span><span class="sxs-lookup"><span data-stu-id="65eb6-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="65eb6-105">Primjer:</span><span class="sxs-lookup"><span data-stu-id="65eb6-105">Example:</span></span>

<span data-ttu-id="65eb6-106">Get-poštanski sandučić WorkingUser | ft Defaultpublicfolderpoštanski sandučić, Učinkovitjepublicfolderpoštanski sandučić</span><span class="sxs-lookup"><span data-stu-id="65eb6-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="65eb6-107">Set-poštanski sandučić ProblemUser-Defaultpublicfolderpoštanski sandučić \<vrijednosti iz prethodne naredbe></span><span class="sxs-lookup"><span data-stu-id="65eb6-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="65eb6-108">Pričekajte najmanje jedan sat kako bi promjena stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="65eb6-108">Wait at least one hour for the change to take effect.</span></span>