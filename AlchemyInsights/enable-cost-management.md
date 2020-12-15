---
title: Omogućivanje upravljanja troškovima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676957"
---
# <a name="enable-cost-management"></a><span data-ttu-id="1a510-102">Omogućivanje upravljanja troškovima</span><span class="sxs-lookup"><span data-stu-id="1a510-102">Enable cost management</span></span>

<span data-ttu-id="1a510-103">**Što znači "troškovi su onemogućeni za vašu tvrtku ili ustanovu"?**</span><span class="sxs-lookup"><span data-stu-id="1a510-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="1a510-104">Tvrtke ili ustanove koje koriste Enterprise Agreement (EA) ili Microsoftov ugovor o kupcu (MCA) mogu onemogućiti pristup podacima o troškovima i cijenama.</span><span class="sxs-lookup"><span data-stu-id="1a510-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="1a510-105">Nakon prijave na portal Azure može koristiti API za naplatu za programsko dohvaćanje faktura (kada je uključena) i pojedinosti o korištenju.</span><span class="sxs-lookup"><span data-stu-id="1a510-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="1a510-106">**Omogućavanje dodatnog korisnika za pristup fakturama**</span><span class="sxs-lookup"><span data-stu-id="1a510-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="1a510-107">Idite na **pretplatu Blade** na portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="1a510-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="1a510-108">Odaberite **fakture** , a zatim **pristupite računima**.</span><span class="sxs-lookup"><span data-stu-id="1a510-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="1a510-109">Uključite pristup, a zatim spremite promjene da biste korisnicima u ulogama koje imaju opseg pretplate dopustili preuzimanje faktura.</span><span class="sxs-lookup"><span data-stu-id="1a510-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="1a510-110">Administrator računa može konfigurirati i da imaju fakture poslane putem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="1a510-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="1a510-111">Dodatne informacije potražite u članku [dohvaćanje fakture u poruci e-pošte](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="1a510-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="1a510-112">**Dodavanje korisnika u ulogu čitača naplate**</span><span class="sxs-lookup"><span data-stu-id="1a510-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="1a510-113">Idite na **pretplatu Blade** na portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="1a510-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="1a510-114">Odaberite **Control Access (IAM)** , a zatim kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="1a510-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="1a510-115">Na stranici **Odabir uloge** odaberite **čitač naplate** .</span><span class="sxs-lookup"><span data-stu-id="1a510-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="1a510-116">Upišite poruku e-pošte korisnika kojeg želite pozvati, a zatim kliknite **u redu** da biste slali pozivnicu.</span><span class="sxs-lookup"><span data-stu-id="1a510-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="1a510-117">Slijedite upute navedene u pozivnici e-pošte da biste se prijavili kao čitač naplate.</span><span class="sxs-lookup"><span data-stu-id="1a510-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="1a510-118">Dodatne informacije potražite u članku [Dodjela pristupa naplati](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="1a510-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="1a510-119">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="1a510-119">**Recommended documents**</span></span>

- [<span data-ttu-id="1a510-120">Omogući prikaz DA i AO putem EA portala</span><span class="sxs-lookup"><span data-stu-id="1a510-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="1a510-121">Troškovi uključeni u upravljanje troškovima</span><span class="sxs-lookup"><span data-stu-id="1a510-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="1a510-122">Podržane ponude za Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1a510-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="1a510-123">Pregled troškova u analizi troškova</span><span class="sxs-lookup"><span data-stu-id="1a510-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="1a510-124">Pružanje pristupa podacima za naplatu</span><span class="sxs-lookup"><span data-stu-id="1a510-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="1a510-125">Provjera pristupa Microsoftovu ugovoru o klijentu</span><span class="sxs-lookup"><span data-stu-id="1a510-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






