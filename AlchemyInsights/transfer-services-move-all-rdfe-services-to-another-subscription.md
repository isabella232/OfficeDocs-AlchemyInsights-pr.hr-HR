---
title: Prijenos servisa – Premještanje svih servisa RDFE na drugu pretplatu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691945"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="ae39d-102">Prijenos servisa – Premještanje svih servisa RDFE na drugu pretplatu</span><span class="sxs-lookup"><span data-stu-id="ae39d-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="ae39d-103">**Premještanje resursa**</span><span class="sxs-lookup"><span data-stu-id="ae39d-103">**Move resources**</span></span>

<span data-ttu-id="ae39d-104">Resursi za Azure mogu se premjestiti u neku drugu pretplatu na Azure ili grupu resursa u istoj pretplati pomoću portala Azure, Azure PowerShell, Azure CLI ili ostatka API-ja za premještanje resursa.</span><span class="sxs-lookup"><span data-stu-id="ae39d-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="ae39d-105">Da biste mogli premještati resurse, pročitajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="ae39d-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="ae39d-106">Kontrolni popis prije preseljenja resursa</span><span class="sxs-lookup"><span data-stu-id="ae39d-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="ae39d-107">Servisi koje je moguće premjestiti</span><span class="sxs-lookup"><span data-stu-id="ae39d-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="ae39d-108">Provjera valjanosti premještanja</span><span class="sxs-lookup"><span data-stu-id="ae39d-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="ae39d-109">Premještanje smjernica za servise</span><span class="sxs-lookup"><span data-stu-id="ae39d-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="ae39d-110">Da biste postojeće resurse premjestili u neku drugu grupu resursa ili pretplatu, možete koristiti sljedeće:</span><span class="sxs-lookup"><span data-stu-id="ae39d-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="ae39d-111">Portal Azure</span><span class="sxs-lookup"><span data-stu-id="ae39d-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="ae39d-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="ae39d-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="ae39d-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ae39d-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="ae39d-114">REST API</span><span class="sxs-lookup"><span data-stu-id="ae39d-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="ae39d-115">Udžbenik: [Premještanje resursa za Azure u neku drugu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="ae39d-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="ae39d-116">**Otklanjanje pogrešaka s programom Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="ae39d-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="ae39d-117">Pogledajte članke u nastavku da biste saznali više o nekim uobičajenim pogreškama implementacije Azura i primili informacije da biste ih riješili.</span><span class="sxs-lookup"><span data-stu-id="ae39d-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="ae39d-118">Ako ne možete pronaći kôd pogreške za vašu pogrešku pri implementaciji, pročitajte članak [Traženje koda pogreške](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="ae39d-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="ae39d-119">Otklanjanje poteškoća s pogreškama prilikom implementacije</span><span class="sxs-lookup"><span data-stu-id="ae39d-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="ae39d-120">Otklanjanje poteškoća s premještanjem resursa Azure na novu grupu resursa ili pretplatu</span><span class="sxs-lookup"><span data-stu-id="ae39d-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="ae39d-121">Imajte na glavi da ako želite nadograditi pretplatu na Azure, kao što je prebacivanje s besplatnog na plaćanje-kao-te-go, morat ćete pretvoriti pretplatu.</span><span class="sxs-lookup"><span data-stu-id="ae39d-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="ae39d-122">Da biste nadogradili besplatnu probnu verziju, pročitajte članak [Nadogradnja besplatne probne ili Microsoftove pretplate na Azure da plati-kao-ti-ići](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="ae39d-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="ae39d-123">Da biste promijenili račun Pay-It-te-go, pročitajte članak [Promjena pretplate na Azure Pay-kao-te-go u neku drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="ae39d-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="ae39d-124">**Da biste dodali ili povezali pretplatu na Azure u servisu Azure Active Directory, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="ae39d-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="ae39d-125">Prijavite se i odaberite pretplatu koju želite koristiti na [stranici pretplate na portalu Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="ae39d-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="ae39d-126">Odaberite **Promijeni direktorij**.</span><span class="sxs-lookup"><span data-stu-id="ae39d-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="ae39d-127">Pregledajte sva upozorenja koja se prikazuju, a zatim odaberite **Promijeni**.</span><span class="sxs-lookup"><span data-stu-id="ae39d-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="ae39d-128">Direktorij se mijenja za pretplatu i prikazat će vam se poruka o uspjehu.</span><span class="sxs-lookup"><span data-stu-id="ae39d-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="ae39d-129">Otvorite *direktorij* mjenjač da biste otvorili novi direktorij.</span><span class="sxs-lookup"><span data-stu-id="ae39d-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="ae39d-130">Da bi se sve ispravno prikazalo, može potrajati i do 10 minuta.</span><span class="sxs-lookup"><span data-stu-id="ae39d-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="ae39d-131">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="ae39d-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="ae39d-132">Prijenos vlasništva nad pretplatom na Azure</span><span class="sxs-lookup"><span data-stu-id="ae39d-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="ae39d-133">Premještanje resursa u novu grupu resursa ili pretplatu</span><span class="sxs-lookup"><span data-stu-id="ae39d-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="ae39d-134">Upravljanje resursima pomoću portala Azure</span><span class="sxs-lookup"><span data-stu-id="ae39d-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
