---
title: O identitetu u servisu Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664162"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="4b641-102">O identitetu u servisu Yammer</span><span class="sxs-lookup"><span data-stu-id="4b641-102">About identity in Yammer</span></span>

<span data-ttu-id="4b641-103">Preporučuje se da sve mreže poduzmu sljedeće korake da bi izbjegli probleme vezane uz identitet:</span><span class="sxs-lookup"><span data-stu-id="4b641-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="4b641-104">Provedba identiteta sustava Office 365 nakon dodjele resursa Microsoftovim 365 računima za korisnike u programu Azure AD da biste osigurali da se svi korisnici prijave pomoću primarnog računa za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b641-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="4b641-105">Dodatne informacije potražite u članku [Provedba identiteta sustava Office 365 za korisnike servisa Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="4b641-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="4b641-106">Konsolidirate više mreža servisa Yammer.</span><span class="sxs-lookup"><span data-stu-id="4b641-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="4b641-107">Naslijeđene konfiguracije servisa Yammer dozvoljavaju povezivanje više mreža servisa Yammer s jednim zakupcem.</span><span class="sxs-lookup"><span data-stu-id="4b641-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="4b641-108">Dodatne informacije potražite u članku [Mrežna migracija – konsolidiranje više mreža servisa Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="4b641-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="4b641-109">Po želji možete nametnuti licenciranje za Yammer da biste blokirali korisnike iz servisa Yammer ako nemaju licencu.</span><span class="sxs-lookup"><span data-stu-id="4b641-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="4b641-110">Dodatne informacije potražite u članku [Upravljanje korisničkim dozvolama za Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4b641-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="4b641-111">Konačno, revidirajte popis korisnika starijih mreža servisa Yammer i obustavite naslijeđene korisnike.</span><span class="sxs-lookup"><span data-stu-id="4b641-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="4b641-112">Preporučuje se da obustavite (deaktivirajte) korisnike umjesto da ih izbrišete jer je brisanje nepovratno.</span><span class="sxs-lookup"><span data-stu-id="4b641-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="4b641-113">Dodatne informacije potražite u članku [nadzor nad korisnicima servisa Yammer u mrežama povezanim sa sustavom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [uklanjanjem korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="4b641-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="4b641-114">Ako konfigurirate Yammer pomoću ovih koraka, bit ćete spremni i konfigurirati mrežu servisa Yammer za izvorni način rada za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4b641-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="4b641-115">Dodatne informacije potražite u članku [Konfiguriranje mreže servisa Yammer za izvorni način rada za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="4b641-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>