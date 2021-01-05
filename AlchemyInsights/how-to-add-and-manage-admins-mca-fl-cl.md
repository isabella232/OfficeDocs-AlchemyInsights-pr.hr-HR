---
title: Dodavanje administratori i upravljanje njima
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755431"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="6f6a8-102">Dodavanje administratori i upravljanje njima</span><span class="sxs-lookup"><span data-stu-id="6f6a8-102">How to add and manage admins</span></span>

<span data-ttu-id="6f6a8-103">Na temelju vašeg opisa problema, pronašli smo rješenje za vas.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="6f6a8-104">Većina je korisnika mogla samostalno riješiti svoj problem nakon praćenja naše dokumentacije.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="6f6a8-105">Da biste upravljali računom za naplatu za Microsoftov ugovor o kupcu (MCA), možete koristiti razne uloge uz željenu razinu programa Access.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="6f6a8-106">Te su uloge osim ugrađenih uloga servisa Azure koje vam pomažu pri kontroli resursa.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="6f6a8-107">**Da biste dodali uloge za naplatu na portalu Azure, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="6f6a8-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="6f6a8-108">Prijavite se na [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6f6a8-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6f6a8-109">Potražite *Upravljanje troškovima + naplata*.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="6f6a8-110">Odaberite Control Access (IAM) na opsegu kao što je račun za naplatu, Profil naplate ili odjeljak faktura u koju želite dati pristup.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="6f6a8-111">Stranica kontrole pristupa (IAM) sadrži popise korisnika i grupa koje su dodijeljene svakoj ulozi za taj opseg.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="6f6a8-112">Da biste dali pristup korisniku, odaberite **Dodaj** s vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="6f6a8-113">Na padajućem popisu *uloga* odaberite ulogu.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="6f6a8-114">Unesite adresu e-pošte korisnika kojem želite dati pristup.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="6f6a8-115">Odaberite **Spremi** da biste dodijelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="6f6a8-116">Da biste uklonili Access za korisnika, odaberite korisnika s dodjelom uloga koju želite ukloniti.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="6f6a8-117">Odaberite **Ukloni**.</span><span class="sxs-lookup"><span data-stu-id="6f6a8-117">Select **Remove**.</span></span>

<span data-ttu-id="6f6a8-118">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="6f6a8-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="6f6a8-119">Definicije uloga za naplatu</span><span class="sxs-lookup"><span data-stu-id="6f6a8-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="6f6a8-120">Uloge i zadaci računa za naplatu</span><span class="sxs-lookup"><span data-stu-id="6f6a8-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="6f6a8-121">Početak rada s računom za naplatu MCA</span><span class="sxs-lookup"><span data-stu-id="6f6a8-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="6f6a8-122">Provjera pristupa Microsoftovu ugovoru o klijentu</span><span class="sxs-lookup"><span data-stu-id="6f6a8-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
