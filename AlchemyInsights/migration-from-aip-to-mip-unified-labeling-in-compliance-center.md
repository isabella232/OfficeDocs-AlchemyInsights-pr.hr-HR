---
title: Migracija iz AIP-a na MIP/Unified označavanje u centru za usklađenost
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674318"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="6ee6e-102">Migracija iz AIP-a na MIP/Unified označavanje u centru za usklađenost</span><span class="sxs-lookup"><span data-stu-id="6ee6e-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="6ee6e-103">Da biste migrirali iz Alp naljepnica na sjedinjenje označavanja u centru za sigurnost i usklađenost, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="6ee6e-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="6ee6e-104">**Aktivacija zaštite s portala Azure**</span><span class="sxs-lookup"><span data-stu-id="6ee6e-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="6ee6e-105">Ako to već niste učinili, otvorite novi prozor preglednika i [prijavite se na portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="6ee6e-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="6ee6e-106">Dođite do noža za **zaštitu podataka za Azure** .</span><span class="sxs-lookup"><span data-stu-id="6ee6e-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="6ee6e-107">Na izborniku koncentrator, primjerice, kliknite **sve servise** i počnite upisivati **podatke** u okvir Filtar.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="6ee6e-108">Odaberite **zaštiti informacija o Azure**.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="6ee6e-109">Ako prije niste pristupili oštrici zaštite za Azure, pogledajte [upute](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) za dodavanje ove oštrice na portal.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="6ee6e-110">Da biste otvorili nož za zaštitu informacija za Azure, morate imati [tarifu za zaštitu informacija za Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) , ili plan sustava Office 365 koji obuhvaća upravljanje pravima.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="6ee6e-111">Ako imate neku od tih pretplata, ali pogledajte poruku da nije moguće pronaći valjanu pretplatu, obratite se [Microsoftovoj podršci](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ili koristite standardne kanale za podršku.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="6ee6e-112">Pronađite mogućnosti izbornika **Upravljanje** , a zatim odaberite **Zaštita**.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="6ee6e-113">Kliknite **Aktiviraj**, a zatim potvrdite akciju.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="6ee6e-114">Kada aktivacija bude dovršena, ta će se informacijska traka prilikom aktivacije prikazati **uspješno dovršena**.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="6ee6e-115">**Migracija naljepnica s zaštitom servisa Azure na servisu Office 365 Security & centar za usklađenost**</span><span class="sxs-lookup"><span data-stu-id="6ee6e-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="6ee6e-116">Provjerite jeste li prijavljeni kao korisnik s dozvolom globalnog administratora.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="6ee6e-117">Dođite do noža za **zaštitu podataka za Azure** .</span><span class="sxs-lookup"><span data-stu-id="6ee6e-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="6ee6e-118">Na **stranici Upravljanje** izbornikom odaberite **sjedinjeno označavanje**.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="6ee6e-119">Na stranici za **zaštitu od Azure – jedinstven** okvir za označavanje kliknite **Aktiviraj** , a zatim slijedite upute na internetu.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="6ee6e-120">**Pažnja**: Provjerite imate li odgovarajuće dozvole prije aktiviranja migracije centra za sigurnost &.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="6ee6e-121">Dodatne informacije potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="6ee6e-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="6ee6e-122">Morate li biti globalni administrator da biste konfigurirali zaštitu za informacije o Azure ili mogu li delegirati drugim administratorima?</span><span class="sxs-lookup"><span data-stu-id="6ee6e-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="6ee6e-123">Važne informacije o administratorskim ulogama nakon migracije u centar za sigurnost & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="6ee6e-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="6ee6e-124">Dodatne informacije o programu AIP za sjedinjenje označavanja migracije u centar za sigurnost i usklađenost potražite u članku [migracija naljepnica](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="6ee6e-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
