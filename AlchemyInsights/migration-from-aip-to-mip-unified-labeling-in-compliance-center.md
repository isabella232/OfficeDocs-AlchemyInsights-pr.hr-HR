---
title: Migracija iz AIP-a u MIP/Sjedinjeno označavanje u centru za usklađenost
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825363"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="d60cc-102">Migracija iz AIP-a u MIP/Sjedinjeno označavanje u centru za usklađenost</span><span class="sxs-lookup"><span data-stu-id="d60cc-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="d60cc-103">Da biste migrirati s AIP naljepnica na sjedinjeno označavanje u centru za sigurnost i usklađenost, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="d60cc-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="d60cc-104">**Aktivacija zaštite s portala Azure**</span><span class="sxs-lookup"><span data-stu-id="d60cc-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="d60cc-105">Ako to još niste učinili, otvorite novi prozor preglednika i [prijavite se na portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="d60cc-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="d60cc-106">Pomaknite se do **oštrice Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="d60cc-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="d60cc-107">Na izborniku središte, primjerice, kliknite **Svi servisi i** počnite **upisivati informacije** u okvir Filtar.</span><span class="sxs-lookup"><span data-stu-id="d60cc-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="d60cc-108">Odaberite **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="d60cc-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="d60cc-109">Ako još niste pristupili oštrici Azure Information Protection, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pogledajte dodatne korake za dodavanje ove oštrice na portal.</span><span class="sxs-lookup"><span data-stu-id="d60cc-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="d60cc-110">Da biste otvorili oštricu Azure Information Protection, morate imati plan [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili plan sustava Office 365 koji obuhvaća upravljanje pravima.</span><span class="sxs-lookup"><span data-stu-id="d60cc-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="d60cc-111">Ako imate jednu od tih pretplata, ali vidite poruku da nije moguće pronaći valjanu pretplatu, obratite se [Microsoftovoj](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) podršci ili koristite standardne kanale podrške.</span><span class="sxs-lookup"><span data-stu-id="d60cc-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="d60cc-112">Pronađite mogućnosti **izbornika Upravljanje** i odaberite **Aktivacija zaštite**.</span><span class="sxs-lookup"><span data-stu-id="d60cc-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="d60cc-113">Kliknite **Aktiviraj**, a zatim potvrdite akciju.</span><span class="sxs-lookup"><span data-stu-id="d60cc-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="d60cc-114">Kada aktivacija završi, informativna traka prikazuje uspješno **dovršenu aktivaciju.**</span><span class="sxs-lookup"><span data-stu-id="d60cc-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="d60cc-115">**Migriranje naljepnica za Azure Information Protection u centar za sigurnost sustava Office 365 & za usklađenost**</span><span class="sxs-lookup"><span data-stu-id="d60cc-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="d60cc-116">Provjerite jeste li prijavljeni kao korisnik s dozvolom globalnog administratora.</span><span class="sxs-lookup"><span data-stu-id="d60cc-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="d60cc-117">Pomaknite se do **oštrice Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="d60cc-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="d60cc-118">Na **izborniku Upravljanje** odaberite **Sjedinjeno označavanje**.</span><span class="sxs-lookup"><span data-stu-id="d60cc-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="d60cc-119">Na **alatu Azure Information Protection - Unified labeling** blade (Sjedinjeno **označavanje) kliknite Aktiviraj** i slijedite mrežne upute.</span><span class="sxs-lookup"><span data-stu-id="d60cc-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="d60cc-120">**Napomena:** provjerite imate li odgovarajuće dozvole prije aktivacije migracije centra za & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="d60cc-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="d60cc-121">Dodatne informacije potražite u ovim člancima:</span><span class="sxs-lookup"><span data-stu-id="d60cc-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="d60cc-122">Morate li biti globalni administrator da biste konfigurirali Azure Information Protection ili mogu delegirati drugim administratorima?</span><span class="sxs-lookup"><span data-stu-id="d60cc-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="d60cc-123">Važne informacije o administrativnim ulogama nakon migracije u centar za & usklađenost.</span><span class="sxs-lookup"><span data-stu-id="d60cc-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="d60cc-124">Dodatne informacije o migraciji AIP-a u sjedinjeno označavanje u centar za sigurnost i usklađenost potražite u [članku Migracija naljepnica](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="d60cc-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
