---
title: Prijenos vlasništva Azure za naplatu
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922003"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="2c3a6-102">Prijenos vlasništva Azure za naplatu</span><span class="sxs-lookup"><span data-stu-id="2c3a6-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="2c3a6-103">Prijavite se na [portal Azure](https://portal.azure.com/) kao administrator računa za naplatu koji sadrži pretplatu koju želite prenijeti.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="2c3a6-104">Ako niste sigurni jeste li i administrator ili ako morate odrediti tko jest, pročitajte članak [određivanje administratora naplate računa](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="2c3a6-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="2c3a6-105">Pretraživanje za **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="2c3a6-106">Odaberite **pretplate** iz lijevog okna.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="2c3a6-107">Ovisno o pristupu, možda ćete morati odabrati opseg naplate, **a zatim pretplate** ili **Azure pretplate**.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="2c3a6-108">Odaberite **prijenos vlasništva za naplatu** za pretplatu koju želite prenijeti</span><span class="sxs-lookup"><span data-stu-id="2c3a6-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="2c3a6-109">Unesite adresu e-pošte korisnika koji je administrator naplate računa koji će biti novi vlasnik pretplate, a zatim odaberite **Pošalji zahtjev za prijenos**</span><span class="sxs-lookup"><span data-stu-id="2c3a6-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="2c3a6-110">Korisnik će dobiti poruku e-pošte s uputama za pregled vašeg zahtjeva za prijenos.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="2c3a6-111">Da biste odobrili zahtjev za prijenos, korisnik će odabrati vezu u poruci e-pošte i slijediti upute.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="2c3a6-112">**Pažnja** : Ako prenesete vlasništvo nad pretplatom na korisnički račun u drugom servisu Azure AD, svi zadaci koji se [temelje na ulogama (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)za upravljanje resursima u pretplati trajno se uklanjaju.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="2c3a6-113">Samo novi vlasnik imat će pristup resursima u pretplati.</span><span class="sxs-lookup"><span data-stu-id="2c3a6-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="2c3a6-114">Dodatne informacije potražite u članku [prijenos pretplate na korisnika u nekom drugom klijentu za Azure ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2c3a6-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="2c3a6-115">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="2c3a6-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="2c3a6-116">Prijenos vlasništva nad pretplatom za Azure na drugi račun</span><span class="sxs-lookup"><span data-stu-id="2c3a6-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="2c3a6-117">Prijenos vlasništva nad plaćama za pretplatu na Azure</span><span class="sxs-lookup"><span data-stu-id="2c3a6-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="2c3a6-118">Prijenos Visual Studio, Microsoft partner Network (MPN) i pay kao što ste ići dev/test pretplate</span><span class="sxs-lookup"><span data-stu-id="2c3a6-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="2c3a6-119">Najčešća pitanja o prijenosu vlasništva</span><span class="sxs-lookup"><span data-stu-id="2c3a6-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="2c3a6-120">Otklanjanje poteškoća s vlasničkim prijenosom</span><span class="sxs-lookup"><span data-stu-id="2c3a6-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
