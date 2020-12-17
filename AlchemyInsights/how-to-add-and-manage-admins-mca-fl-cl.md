---
title: Dodavanje i upravljanje administratorima-MCA FL/CL
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
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691961"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="20ce5-102">Dodavanje i upravljanje administratorima-MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="20ce5-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="20ce5-103">Da biste upravljali računom za naplatu za Microsoftov ugovor o kupcu (MCA), možete koristiti razne uloge uz željenu razinu programa Access.</span><span class="sxs-lookup"><span data-stu-id="20ce5-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="20ce5-104">Te su uloge osim ugrađenih uloga servisa Azure koje vam pomažu pri kontroli resursa.</span><span class="sxs-lookup"><span data-stu-id="20ce5-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="20ce5-105">**Da biste dodali uloge za naplatu na portalu Azure, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="20ce5-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="20ce5-106">Prijavite se na [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="20ce5-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="20ce5-107">Potražite *Upravljanje troškovima + naplata*.</span><span class="sxs-lookup"><span data-stu-id="20ce5-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="20ce5-108">Odaberite Control Access (IAM) na opsegu kao što je račun za naplatu, Profil naplate ili odjeljak faktura u koju želite dati pristup.</span><span class="sxs-lookup"><span data-stu-id="20ce5-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="20ce5-109">Stranica kontrole pristupa (IAM) sadrži popise korisnika i grupa koje su dodijeljene svakoj ulozi za taj opseg.</span><span class="sxs-lookup"><span data-stu-id="20ce5-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="20ce5-110">Da biste dali pristup korisniku, odaberite **Dodaj** s vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="20ce5-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="20ce5-111">Na padajućem popisu *uloga* odaberite ulogu.</span><span class="sxs-lookup"><span data-stu-id="20ce5-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="20ce5-112">Unesite adresu e-pošte korisnika kojem želite dati pristup.</span><span class="sxs-lookup"><span data-stu-id="20ce5-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="20ce5-113">Odaberite **Spremi** da biste dodijelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="20ce5-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="20ce5-114">Da biste uklonili Access za korisnika, odaberite korisnika s dodjelom uloga koju želite ukloniti.</span><span class="sxs-lookup"><span data-stu-id="20ce5-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="20ce5-115">Odaberite **Ukloni**.</span><span class="sxs-lookup"><span data-stu-id="20ce5-115">Select **Remove**.</span></span>

<span data-ttu-id="20ce5-116">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="20ce5-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="20ce5-117">Definicije uloga za naplatu</span><span class="sxs-lookup"><span data-stu-id="20ce5-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="20ce5-118">Uloge i zadaci računa za naplatu</span><span class="sxs-lookup"><span data-stu-id="20ce5-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="20ce5-119">Početak rada s računom za naplatu MCA</span><span class="sxs-lookup"><span data-stu-id="20ce5-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="20ce5-120">Provjera pristupa Microsoftovu ugovoru o klijentu</span><span class="sxs-lookup"><span data-stu-id="20ce5-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)