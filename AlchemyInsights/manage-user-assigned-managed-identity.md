---
title: Upravljanje upravljanim identitetom dodijeljenim korisniku
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177405"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="875bc-102">Upravljanje upravljanim identitetom dodijeljenim korisniku</span><span class="sxs-lookup"><span data-stu-id="875bc-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="875bc-103">Upravljanje upravljanim identitetom dodijeljenim korisniku obuhvaća:</span><span class="sxs-lookup"><span data-stu-id="875bc-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="875bc-104">Dodjela uloga korisniku kojima je dodijeljen upravljani identitet</span><span class="sxs-lookup"><span data-stu-id="875bc-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="875bc-105">Brisanje upravljanog identiteta koji je dodijeljen korisniku</span><span class="sxs-lookup"><span data-stu-id="875bc-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="875bc-106">Popis korisnika koji je dodijelio upravljani identitet</span><span class="sxs-lookup"><span data-stu-id="875bc-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="875bc-107">Dodatne informacije o navedenim zadacima potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="875bc-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="875bc-108">[Stvaranje korisnikovog upravljanog identiteta](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – za dodjelu uloga korisniku kojima je dodijeljen upravljani identitet</span><span class="sxs-lookup"><span data-stu-id="875bc-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="875bc-109">[Brisanje korisniku dodijeljenog upravljanog identiteta](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – za brisanje upravljanog identiteta koji je dodijeljen korisniku</span><span class="sxs-lookup"><span data-stu-id="875bc-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="875bc-110">[Popis korisnika koji je dodijelio upravljani identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – za ispis upravljanog identiteta koji je dodijeljen korisniku</span><span class="sxs-lookup"><span data-stu-id="875bc-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="875bc-111">Provjerite imate li dodjelu uloge **suradnika za upravljane identitete** .</span><span class="sxs-lookup"><span data-stu-id="875bc-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="875bc-112">Ta je dodjela uloga obavezna za stvaranje/Brisanje korisničkih identiteta dodijeljenih korisniku.</span><span class="sxs-lookup"><span data-stu-id="875bc-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
