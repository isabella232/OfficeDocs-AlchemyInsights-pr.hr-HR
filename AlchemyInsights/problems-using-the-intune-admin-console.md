---
title: Problemi pomoću konzole Intune admin
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728279"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="8d843-102">Problemi pomoću konzole Intune admin</span><span class="sxs-lookup"><span data-stu-id="8d843-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="8d843-103">**"Pristup je odbijen" prilikom navigacije putem portala Intune admin.**</span><span class="sxs-lookup"><span data-stu-id="8d843-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="8d843-104">Ako ste član prilagođene uloge u ugodi, provjerite je li vaš račun dodijeljen licencama za Intune ili Enterprise Mobility suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="8d843-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="8d843-105">Ako upraviteljem konfiguracije koristite za upravljanje uređajima, provjerite niste li dio zbirke dodatka user za Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="8d843-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="8d843-106">Provjerite jesu li vam dodijeljene dozvole za upravljanje administracijom na temelju uloga (RBAC) u oštrici Intune uloge.</span><span class="sxs-lookup"><span data-stu-id="8d843-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="8d843-107">Provjera korištene grupe nije popis za raspodjelu.</span><span class="sxs-lookup"><span data-stu-id="8d843-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="8d843-108">Intune na portalu Azure podržava samo korisničke račune koji spadaju u sigurnosne grupe servisa Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8d843-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="8d843-109">Pregledajte grupe na portalu Azure > **Intune**  >  **Groups**ili na portalu Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="8d843-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="8d843-110">**Korisnik ima previše dozvola za dodijeljenu ulogu Utune.**</span><span class="sxs-lookup"><span data-stu-id="8d843-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="8d843-111">Savjetujte korisniku da se otvori u odjeljku **Intune**  >  **Intune**za  >  **moje dozvole**  >  za**Izvoz** da biste pregledali dodijeljene dozvole.</span><span class="sxs-lookup"><span data-stu-id="8d843-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="8d843-112">**U ulogu sam dodao grupu opsega, no korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**</span><span class="sxs-lookup"><span data-stu-id="8d843-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="8d843-113">Grupe dosega ne filtriraju korisnike ni uređaje.</span><span class="sxs-lookup"><span data-stu-id="8d843-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="8d843-114">Grupe dosega:</span><span class="sxs-lookup"><span data-stu-id="8d843-114">Scope groups:</span></span>

- <span data-ttu-id="8d843-115">Ograničite osobe kojima korisnici mogu dodijeliti pravila ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="8d843-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="8d843-116">Dopusti samo određenim korisnicima pokretanje udaljenih zadataka na uređajima.</span><span class="sxs-lookup"><span data-stu-id="8d843-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="8d843-117">Dodatne informacije o grupama dosega potražite u članku  [kontrola pristupa utemeljenoj na ulogama (RBAC) pomoću aplikacije Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="8d843-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="8d843-118">**Dodao sam korisnika u željenu ulogu, ali i dalje imaju potpun pristup konzoli za administraciju Intune.**</span><span class="sxs-lookup"><span data-stu-id="8d843-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="8d843-119">Idite na Umetanje > **korisnika** na portalu Azure i provjerite nije li korisnik dodijeljen bilo kojoj od sljedećih uloga na portalu Azure:</span><span class="sxs-lookup"><span data-stu-id="8d843-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="8d843-120">Globalni administrator</span><span class="sxs-lookup"><span data-stu-id="8d843-120">Global administrator</span></span>
- <span data-ttu-id="8d843-121">Unos administratora usluge</span><span class="sxs-lookup"><span data-stu-id="8d843-121">Intune service administrator</span></span>
- <span data-ttu-id="8d843-122">Administrator sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="8d843-122">SharePoint administrator</span></span>

<span data-ttu-id="8d843-123">Dodatne informacije potražite u članku [kontrola pristupa utemeljenu na ulogama (RBAC) pomoću aplikacije Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="8d843-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="8d843-124">**Problemi s pristupom**</span><span class="sxs-lookup"><span data-stu-id="8d843-124">**Access Issues**</span></span>

<span data-ttu-id="8d843-125">Dodatne informacije potražite u članku [ne možete se prijaviti u Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="8d843-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>