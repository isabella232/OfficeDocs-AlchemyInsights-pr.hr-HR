---
title: Podržane vrste pretplate
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807247"
---
# <a name="supported-subscription-types"></a><span data-ttu-id="f8fb4-102">Podržane vrste pretplate</span><span class="sxs-lookup"><span data-stu-id="f8fb4-102">Supported subscription types</span></span>

<span data-ttu-id="f8fb4-103">Pregledajte podržane vrste pretplata da biste nastavili dalje.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-103">Please review the supported subscription types to proceed further.</span></span>

[<span data-ttu-id="f8fb4-104">Podržane vrste pretplate</span><span class="sxs-lookup"><span data-stu-id="f8fb4-104">Supported subscription types</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

<span data-ttu-id="f8fb4-105">**Prijenos vlasništva nad naplaćivanje**</span><span class="sxs-lookup"><span data-stu-id="f8fb4-105">**Transfer billing ownership**</span></span>

<span data-ttu-id="f8fb4-106">Azure portal kao [administrator računa](https://ms.portal.azure.com/) za račun za naplatu s pretplatom koju želite prenijeti</span><span class="sxs-lookup"><span data-stu-id="f8fb4-106">Azure portal as the [Account Admin](https://ms.portal.azure.com/) of the billing account that has the subscription you want to transfer</span></span>

- <span data-ttu-id="f8fb4-107">Pretraživanje za **Upravljanje troškovima + naplata** .</span><span class="sxs-lookup"><span data-stu-id="f8fb4-107">Search on **Cost Management + Billing** .</span></span> <span data-ttu-id="f8fb4-108">Odaberite **pretplate** iz lijevog okna.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-108">Select **Subscriptions** from left-pane.</span></span> <span data-ttu-id="f8fb4-109">Ovisno o pristupu, možda ćete morati odabrati opseg naplate, **a zatim pretplate** ili **Azure pretplate** .</span><span class="sxs-lookup"><span data-stu-id="f8fb4-109">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions** .</span></span>
- <span data-ttu-id="f8fb4-110">Odaberite prijenos vlasništva za naplatu za pretplatu koju želite prenijeti</span><span class="sxs-lookup"><span data-stu-id="f8fb4-110">Select Transfer billing ownership for the subscription you want to transfer</span></span>
- <span data-ttu-id="f8fb4-111">Unesite adresu e-pošte korisnika koji je administrator naplate računa koji će biti novi vlasnik pretplate, a zatim odaberite **Pošalji zahtjev za prijenos**</span><span class="sxs-lookup"><span data-stu-id="f8fb4-111">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="f8fb4-112">Korisnik će dobiti poruku e-pošte s uputama za pregled vašeg zahtjeva za prijenos.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-112">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="f8fb4-113">Da biste odobrili zahtjev za prijenos, korisnik će odabrati vezu u poruci e-pošte i slijediti upute.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-113">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="f8fb4-114">Pažnja: Ako prenesete vlasništvo nad pretplatom na korisnički račun u drugom servisu Azure AD, svi zadaci koji se [temelje na ulogama (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje resursima u pretplati trajno se uklanjaju.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-114">Note: If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="f8fb4-115">Samo novi vlasnik imat će pristup resursima u pretplati.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-115">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="f8fb4-116">Dodatne informacije potražite u članku [prijenos pretplate na korisnika u nekom drugom klijentu za Azure ad](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f8fb4-116">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f8fb4-117">**Prijenos vlasništva nad pretplatom**</span><span class="sxs-lookup"><span data-stu-id="f8fb4-117">**Transfer Ownership of Subscription**</span></span>

<span data-ttu-id="f8fb4-118">Preduvjet za prijenos vlasništva na pretplatničkim ulogama (RBAC) za upravljanje resursima u pretplati gube pristup.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-118">Subscription Ownership Transfer prerequisites role based access (RBAC) to manage resources in the subscription lose their access.</span></span> <span data-ttu-id="f8fb4-119">Dodatne informacije o dodavanju postojeće pretplate na korisnika potražite u članku [pridruživanje i dodavanje pretplate Azure u servisu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="f8fb4-119">For more information about adding an existing subscription to a tenant, see [Associate or add an Azure subscription to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

- <span data-ttu-id="f8fb4-120">Prijenos pretplate uz postojeći neplaćeni iznos iz tekućeg ciklusa naplate neće se prenijeti na novi instrument plaćanja u novom računu.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-120">Subscription Transfer with an existing outstanding amount from the current billing cycle will not be transferred to the new payment instrument in the new account.</span></span> <span data-ttu-id="f8fb4-121">Jedine informacije dostupne korisnicima u novom računu jesu troškovi posljednjeg mjeseca za vašu pretplatu.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-121">The only information available to the users in new account is the last month's cost for your subscription.</span></span> <span data-ttu-id="f8fb4-122">Ostatak povijesti upotrebe i naplate ne prenosi se pretplatom.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-122">The rest of the usage and billing history does not transfer with the subscription.</span></span>
- <span data-ttu-id="f8fb4-123">Prijenos vlasništva nad pretplatom na Enterprise Agreement (EA) trenutno je podržan samo na portalu za Enterprise sporazum</span><span class="sxs-lookup"><span data-stu-id="f8fb4-123">Transfer billing ownership of Enterprise Agreement (EA) subscriptions is currently supported in the Enterprise Agreement Portal only</span></span>
- <span data-ttu-id="f8fb4-124">Prijenos pretplate orijentiranog na kredit kao što je Visual Studio, BizSpark, Microsoftova mrežna mreža za novog korisnika mora imati licencu za Visual Studio/Microsoftovu partnersku mrežu da bi prihvatio zahtjev za prijenos</span><span class="sxs-lookup"><span data-stu-id="f8fb4-124">Transferring a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request</span></span>
- <span data-ttu-id="f8fb4-125">Svi resursi kao što su virtualni strojevi, diskovi i web-mjesta uspješno se prebacuju na novi račun.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-125">All resources like Virtual Machines, disks, and websites transfer to the new account successfully.</span></span> <span data-ttu-id="f8fb4-126">Sljedeći resursi mogu utjecati na prijenos pretplate na više korisnika:</span><span class="sxs-lookup"><span data-stu-id="f8fb4-126">The following resources could be affected in a cross-tenant subscription transfer:</span></span>

<span data-ttu-id="f8fb4-127">**Usluge servisa Azure AD Domain**</span><span class="sxs-lookup"><span data-stu-id="f8fb4-127">**Azure AD Domain Services**</span></span>

<span data-ttu-id="f8fb4-128">Sefovi za Azure</span><span class="sxs-lookup"><span data-stu-id="f8fb4-128">Azure Key Vaults</span></span>

- <span data-ttu-id="f8fb4-129">Moguće je utjecati na [korisnike i baze podataka vezanih uz SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , osobito ako klijent koristi provjeru autentičnosti povezanu s Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8fb4-129">[SQL related users and databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) could be impacted, especially if the customer uses an Azure Active Directory related authentication</span></span>
- <span data-ttu-id="f8fb4-130">**Aplikacijski servisi** konfigurirani uz provjeru autentičnosti servisa Azure Active Directory mogu se utjecati</span><span class="sxs-lookup"><span data-stu-id="f8fb4-130">**App Services** configured with Azure Active Directory authentication could be impacted</span></span>
- <span data-ttu-id="f8fb4-131">**Vizualni studijski tim** Računi servisa povezani s pretplatama na Azure mogu privremeno izgubiti Access kada se otkaže pretplata na Azure</span><span class="sxs-lookup"><span data-stu-id="f8fb4-131">**Visual Studio Team** Services accounts connected to Azure subscriptions may temporarily lose access when the connected Azure subscription is cancelled</span></span>

<span data-ttu-id="f8fb4-132">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="f8fb4-132">**Recommended Documents**</span></span>

<span data-ttu-id="f8fb4-133">Koraci nakon prihvaćanja vlasništva nad naplaćom:</span><span class="sxs-lookup"><span data-stu-id="f8fb4-133">Steps after accepting billing ownership:</span></span>

- <span data-ttu-id="f8fb4-134">Da biste zadržali vlasništvo nad naplaćivanju, ali promijenite vrstu pretplate, pogledajte: [prebacivanje pretplate na Azure na drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="f8fb4-134">To retain billing ownership, but change the type of your subscription, refer: [Switch your Azure subscription to another offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- [<span data-ttu-id="f8fb4-135">Prijenos Visual Studio, Microsoft partner Network (MPN) i pay kao što ste ići dev/test pretplate</span><span class="sxs-lookup"><span data-stu-id="f8fb4-135">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="f8fb4-136">Prijenos vlasništva nad pretplatama na Enterprise Agreement (EA)</span><span class="sxs-lookup"><span data-stu-id="f8fb4-136">Transfer billing ownership of Enterprise Agreement (EA) subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [<span data-ttu-id="f8fb4-137">Najčešća pitanja o prijenosu vlasništva</span><span class="sxs-lookup"><span data-stu-id="f8fb4-137">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="f8fb4-138">Otklanjanje poteškoća s vlasničkim prijenosom</span><span class="sxs-lookup"><span data-stu-id="f8fb4-138">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)