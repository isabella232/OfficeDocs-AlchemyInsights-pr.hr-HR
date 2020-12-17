---
title: Dodavanje i upravljanje administratorima – preporučeni koraci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676976"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="8d93c-102">Dodavanje i upravljanje administratorima – preporučeni koraci</span><span class="sxs-lookup"><span data-stu-id="8d93c-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="8d93c-103">**Uređivanje administratora pretplate ili Suadministratora**</span><span class="sxs-lookup"><span data-stu-id="8d93c-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="8d93c-104">Administrator računa može uređivati obje uloge dok administrator pretplate može promijeniti samo suadministratore na [portalu Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="8d93c-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="8d93c-105">Dodavanje ili promjena administratora pretplate na Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="8d93c-106">**Ažuriranje administratora pretplate ili Co-Administrator za interne (emitiranja) pretplate**</span><span class="sxs-lookup"><span data-stu-id="8d93c-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="8d93c-107">Administrator servisa ili Suadministrator mogu samostalno služiti ovu akciju pomoću sljedećih koraka:</span><span class="sxs-lookup"><span data-stu-id="8d93c-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="8d93c-108">Prijavite se na [portal Azure](https://ms.portal.azure.com/#home) , a zatim kliknite **Upravljanje troškovima + naplata** u lijevoj oštrici.</span><span class="sxs-lookup"><span data-stu-id="8d93c-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="8d93c-109">Kliknite stavku na retku s pretplatom.</span><span class="sxs-lookup"><span data-stu-id="8d93c-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="8d93c-110">Time ćete otvoriti pregled pretplate.</span><span class="sxs-lookup"><span data-stu-id="8d93c-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="8d93c-111">Na kartici **Pretplata** kliknite **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="8d93c-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="8d93c-112">Kliknite gumb **administrator servisa** .</span><span class="sxs-lookup"><span data-stu-id="8d93c-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="8d93c-113">Unesite poruku e-pošte korisnika kojeg želite postaviti kao administratora servisa, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="8d93c-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="8d93c-114">**Dodavanje/promjena/uklanjanje Suadministratora**</span><span class="sxs-lookup"><span data-stu-id="8d93c-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="8d93c-115">Prijavite se na [portal Azure](https://ms.portal.azure.com/#home) kao administrator servisa.</span><span class="sxs-lookup"><span data-stu-id="8d93c-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="8d93c-116">Otvorite [pretplate](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) , a zatim odaberite pretplatu.</span><span class="sxs-lookup"><span data-stu-id="8d93c-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="8d93c-117">(Suadministratori se mogu dodijeliti samo u opsegu pretplate).</span><span class="sxs-lookup"><span data-stu-id="8d93c-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="8d93c-118">Pomaknite se do **kontrole Access (iam)**  >  **Classic administratori**  >  **dodatku** Dodaj  >  **suadministrator** da biste otvorili okno **Dodavanje suadministratora** (ako je mogućnost Dodaj suadministrator onemogućena, označava da nemate dozvole).</span><span class="sxs-lookup"><span data-stu-id="8d93c-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="8d93c-119">Odaberite korisnika kojeg želite dodati, a zatim kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="8d93c-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="8d93c-120">**uči više:**</span><span class="sxs-lookup"><span data-stu-id="8d93c-120">**Learn more:**</span></span>
- [<span data-ttu-id="8d93c-121">Dodavanje Suadministratora</span><span class="sxs-lookup"><span data-stu-id="8d93c-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="8d93c-122">Uklanjanje suadministratora</span><span class="sxs-lookup"><span data-stu-id="8d93c-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="8d93c-123">Promjena administratora servisa</span><span class="sxs-lookup"><span data-stu-id="8d93c-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="8d93c-124">Prikaz administratora računa</span><span class="sxs-lookup"><span data-stu-id="8d93c-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="8d93c-125">Upravljanje pristupom pomoću portala RBAC i Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="8d93c-126">**Dodavanje/brisanje korisnika pomoću servisa Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="8d93c-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="8d93c-127">Možete dodati nove korisnike ili izbrisati postojeće korisnike iz tvrtke ili ustanove za Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="8d93c-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="8d93c-128">Da biste dodali novog korisnika, prijavite se na [portal Azure](https://ms.portal.azure.com/#home) kao korisnik-administrator za tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="8d93c-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="8d93c-129">Odaberite **Azure Active Directory**, odaberite **korisnici** , a zatim kliknite **novi korisnik**.</span><span class="sxs-lookup"><span data-stu-id="8d93c-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="8d93c-130">Na stranici **korisnika** unesite potrebne podatke.</span><span class="sxs-lookup"><span data-stu-id="8d93c-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="8d93c-131">Kliknite **Stvori**.</span><span class="sxs-lookup"><span data-stu-id="8d93c-131">Click **Create**.</span></span> <span data-ttu-id="8d93c-132">Korisnik se stvara i dodaje u zakupac Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8d93c-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="8d93c-133">Dodatne **informacije**:</span><span class="sxs-lookup"><span data-stu-id="8d93c-133">**Learn more**:</span></span>

- [<span data-ttu-id="8d93c-134">Dodavanje novog korisnika</span><span class="sxs-lookup"><span data-stu-id="8d93c-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="8d93c-135">Brisanje korisnika</span><span class="sxs-lookup"><span data-stu-id="8d93c-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="8d93c-136">Dodavanje i ažuriranje korisničkih podataka o profilu pomoću servisa Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="8d93c-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="8d93c-137">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="8d93c-137">**Recommended documents**</span></span>

- [<span data-ttu-id="8d93c-138">Što je kontrola pristupa utemeljenih na ulogama (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="8d93c-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="8d93c-139">Razumijevanje raznih uloga u servisu Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="8d93c-140">Dozvole za administratorsku ulogu u servisu Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="8d93c-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="8d93c-141">Udžbenik: dodijelite pristup korisniku pomoću RBAC-a i portala Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="8d93c-142">Otklanjanje poteškoća s RBAC-om u servisu Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="8d93c-143">Organiziranje resursa pomoću grupa za upravljanje Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="8d93c-144">Kako zatražiti kopiju Azure fakture putem e-pošte</span><span class="sxs-lookup"><span data-stu-id="8d93c-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="8d93c-145">Dodavanje, ažuriranje ili uklanjanje kreditne ili debitne kartice iz servisa Azure</span><span class="sxs-lookup"><span data-stu-id="8d93c-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="8d93c-146">Upravljanje pretplatom (ponovno aktiviranje/otkazivanje/prebacivanje)</span><span class="sxs-lookup"><span data-stu-id="8d93c-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)


