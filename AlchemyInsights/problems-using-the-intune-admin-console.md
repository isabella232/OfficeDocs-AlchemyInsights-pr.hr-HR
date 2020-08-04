---
title: Problemi s korištenjem konzole administratora Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554881"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="1cc0e-102">Problemi s korištenjem konzole administratora Intune</span><span class="sxs-lookup"><span data-stu-id="1cc0e-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="1cc0e-103">**"Pristup je odbijen" prilikom navigacije intune admin portalom.**</span><span class="sxs-lookup"><span data-stu-id="1cc0e-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="1cc0e-104">Ako ste član prilagođene uloge Intune, provjerite je li vaš račun dodijeljena licenca Intune ili Enterprise Mobility Suite (EMS).</span><span class="sxs-lookup"><span data-stu-id="1cc0e-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="1cc0e-105">Ako koristite Upravitelj konfiguracije za upravljanje uređajima, provjerite niste li dio zbirke korisnika Intune za Upravitelj konfiguracije MDM.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="1cc0e-106">Provjerite jesu li vam dodijeljene odgovarajuće dozvole kontrole administracije temeljene na ulogama (RBAC) u oštrici uloga Intune.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="1cc0e-107">Provjerite da korištena grupa nije popis raspodjele.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="1cc0e-108">Intune na portalu Azure podržava samo korisničke račune koji pripadaju sigurnosnim grupama servisa Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="1cc0e-109">Pregledajte grupe na portalu Azure > **Intune**  >  **Groups**ili na portalu Azure > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="1cc0e-110">**Korisnik ima previše dozvola za dodijeljenu ulogu Intune**</span><span class="sxs-lookup"><span data-stu-id="1cc0e-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="1cc0e-111">Savjetovati korisnika da ide **na Intune**  >  **Intune uloge**  >  **Moje dozvole**  >  **Izvoz** pregledati odobrene dozvole.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="1cc0e-112">**Dodala sam grupu dosega ulozi, ali korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**</span><span class="sxs-lookup"><span data-stu-id="1cc0e-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="1cc0e-113">Grupe dosega ne filtriraju korisnike ili uređaje.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="1cc0e-114">Grupe dosega:</span><span class="sxs-lookup"><span data-stu-id="1cc0e-114">Scope groups:</span></span>

- <span data-ttu-id="1cc0e-115">Ograničite kome korisnici mogu dodijeliti pravila ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="1cc0e-116">Dopustite samo određenim korisnicima pokretanje daljinskih zadataka na uređajima.</span><span class="sxs-lookup"><span data-stu-id="1cc0e-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="1cc0e-117">Dodatne informacije o grupama dosega [potražite u odjeljku Kontrola pristupa utemeljena na ulogama (RBAC) s programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="1cc0e-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="1cc0e-118">**JA dodani korisnik to Intune uloga ali oni pa ipak imati pun pristup to Intune admin utješiti.**</span><span class="sxs-lookup"><span data-stu-id="1cc0e-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="1cc0e-119">Idite na Intune > **korisnici na** portalu Azure i provjerite nije li korisnik dodijeljen nijednoj od sljedećih uloga na portalu Azure:</span><span class="sxs-lookup"><span data-stu-id="1cc0e-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="1cc0e-120">Globalni administrator</span><span class="sxs-lookup"><span data-stu-id="1cc0e-120">Global administrator</span></span>
- <span data-ttu-id="1cc0e-121">Intune administrator usluga</span><span class="sxs-lookup"><span data-stu-id="1cc0e-121">Intune service administrator</span></span>
- <span data-ttu-id="1cc0e-122">Administrator sustava SharePoint</span><span class="sxs-lookup"><span data-stu-id="1cc0e-122">SharePoint administrator</span></span>

<span data-ttu-id="1cc0e-123">Dodatne informacije [potražite u odjeljku Kontrola pristupa temeljena na ulogama (RBAC) s programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="1cc0e-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="1cc0e-124">**Problemi s pristupom**</span><span class="sxs-lookup"><span data-stu-id="1cc0e-124">**Access Issues**</span></span>

<span data-ttu-id="1cc0e-125">Dodatne informacije [potražite u odjeljku Ne možete se prijaviti u Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="1cc0e-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>