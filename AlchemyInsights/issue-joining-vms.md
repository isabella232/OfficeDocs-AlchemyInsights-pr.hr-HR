---
title: Problem s pridruživanjem VMs-a
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884860"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="648e1-102">Problem s pridruživanjem VMs-a</span><span class="sxs-lookup"><span data-stu-id="648e1-102">Issue joining VMs</span></span>

<span data-ttu-id="648e1-103">Da biste riješili probleme koji se javljaju prilikom pokušaja pridruživanja VMs-u, slijedite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="648e1-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="648e1-104">Pokušajte se prijaviti pomoću oblika **UPN** (primjerice, "joeuser@contoso.com") umjesto oblika **SAMAccountName** ("CONTOSO\joeuser").</span><span class="sxs-lookup"><span data-stu-id="648e1-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="648e1-105">Provjerite jeste li omogućili sinkronizaciju lozinki u skladu sa koracima navedenim u vodiču za *početak rada* .</span><span class="sxs-lookup"><span data-stu-id="648e1-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="648e1-106">Pobrinite se da izvještačen korisnički račun nije vanjski račun u zakupcu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="648e1-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="648e1-107">Vanjski se korisnici ne mogu prijaviti u upravljane domene budući da usluge Azure AD domena nemaju vjerodajnice za takve korisničke račune.</span><span class="sxs-lookup"><span data-stu-id="648e1-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="648e1-108">Ako je izvještačen korisnički račun korisnički račun samo u oblaku, provjerite jesu li korisnici promijenili lozinku nakon što ste omogućili usluge Azure AD domene.</span><span class="sxs-lookup"><span data-stu-id="648e1-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="648e1-109">U ovom se koraku uzrokuje generiranje skice vjerodajnica potrebnih za izvoz servisa Azure AD Domain.</span><span class="sxs-lookup"><span data-stu-id="648e1-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="648e1-110">Ako se prijavljeni korisnički računi sinkroniziraju iz lokalnog direktorija, provjerite je li preporučeno izdanje servisa Azure AD Connect konfigurirano za kompletnu sinkronizaciju.</span><span class="sxs-lookup"><span data-stu-id="648e1-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="648e1-111">Ako se problem nastavi pojavljivati i nakon potvrđene četvrtog koraka, izvršite sljedeće naredbe na uređaju za sinkronizaciju:</span><span class="sxs-lookup"><span data-stu-id="648e1-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="648e1-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="648e1-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>