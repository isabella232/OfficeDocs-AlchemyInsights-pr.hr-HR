---
title: Migracija iz AIP-a u MIP/objedinjeno označavanje u centru za usklađenost
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236362"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="876a8-102">Migracija iz AIP-a u MIP/objedinjeno označavanje u centru za usklađenost</span><span class="sxs-lookup"><span data-stu-id="876a8-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="876a8-103">Da biste migrirali s AIP oznaka u objedinjeno označavanje u centru za sigurnost i usklađenost, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="876a8-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="876a8-104">**Aktiviranje zaštite s portala Azure**</span><span class="sxs-lookup"><span data-stu-id="876a8-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="876a8-105">Ako to još niste učinili, otvorite novi prozor preglednika i [prijavite se na portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="876a8-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="876a8-106">Idite na oštricu **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="876a8-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="876a8-107">Na primjer, na izborniku koncentratora kliknite **Svi servisi** i počnite upisivati **informacije** u okvir Filtar.</span><span class="sxs-lookup"><span data-stu-id="876a8-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="876a8-108">Odaberite **Azure information protection**.</span><span class="sxs-lookup"><span data-stu-id="876a8-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="876a8-109">Ako još niste pristupili oštrici Azure Information Protection, pogledajte [jednokratne dodatne korake](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) za dodavanje ove oštrice na portal.</span><span class="sxs-lookup"><span data-stu-id="876a8-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="876a8-110">Da biste otvorili oštricu Azure Information Protection, morate imati [tarifu Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili tarifu za Office 365 koja uključuje upravljanje pravima.</span><span class="sxs-lookup"><span data-stu-id="876a8-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="876a8-111">Ako imate jednu od tih pretplata, ali vidite poruku da nije moguće pronaći valjanu pretplatu, [obratite se Microsoftovoj podršci](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ili koristite standardne kanale podrške.</span><span class="sxs-lookup"><span data-stu-id="876a8-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="876a8-112">Pronađite mogućnosti izbornika **Upravljanje** i odaberite **Aktivacija zaštite**.</span><span class="sxs-lookup"><span data-stu-id="876a8-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="876a8-113">Kliknite **Aktiviraj**, a zatim potvrdite akciju.</span><span class="sxs-lookup"><span data-stu-id="876a8-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="876a8-114">Kada se aktivacija dovrši, informativna traka prikazuje **aktivaciju uspješno dovršenu**.</span><span class="sxs-lookup"><span data-stu-id="876a8-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="876a8-115">**Migracija oznaka zaštite podataka za Azure u Centar za usklađenost sa sigurnosnim & sustava Office 365**</span><span class="sxs-lookup"><span data-stu-id="876a8-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="876a8-116">Provjerite jeste li prijavljeni kao korisnik s dozvolom globalnog administratora.</span><span class="sxs-lookup"><span data-stu-id="876a8-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="876a8-117">Idite na oštricu **Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="876a8-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="876a8-118">Na izborniku **Upravljanje** odaberite **Objedinjena oznaka**.</span><span class="sxs-lookup"><span data-stu-id="876a8-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="876a8-119">Na oštrici **Azure Information Protection - Unified labeling** kliknite **Aktiviraj** i slijedite mrežne upute.</span><span class="sxs-lookup"><span data-stu-id="876a8-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="876a8-120">**Napomena**: Provjerite imate li odgovarajuće dozvole prije aktivacije migracije centra za & sigurnosti & usklađenosti.</span><span class="sxs-lookup"><span data-stu-id="876a8-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="876a8-121">Pogledajte ove članke za više informacija:</span><span class="sxs-lookup"><span data-stu-id="876a8-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="876a8-122">Trebate li globalni administrator konfigurirati zaštitu podataka za Azure ili mogu delegirati drugim administratorima?</span><span class="sxs-lookup"><span data-stu-id="876a8-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="876a8-123">Važne informacije o administrativnim ulogama nakon migracije u centar za usklađenost & sigurnosti.</span><span class="sxs-lookup"><span data-stu-id="876a8-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="876a8-124">Dodatne informacije o AIP-u objedinjenoj migraciji označavanja u centar za sigurnost i usklađenost potražite u odjeljku [Migracija oznaka](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="876a8-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
