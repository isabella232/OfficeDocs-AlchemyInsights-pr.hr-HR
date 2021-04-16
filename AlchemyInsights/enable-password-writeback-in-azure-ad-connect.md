---
title: Omogućivanje povratnog pisanja lozinke na servisu Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814004"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="06e23-102">Omogućivanje povratnog pisanja lozinke na servisu Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="06e23-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="06e23-103">Da biste omogućili samoposlužno vraćanje izvorne lozinke, najprije omogućite mogućnost povratnog pisanja na servisu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="06e23-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="06e23-104">Na poslužitelju azure AD Connect učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="06e23-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="06e23-105">Prijavite se na poslužitelj servisa Azure AD Connect i pokrenite čarobnjak za **konfiguraciju servisa Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="06e23-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="06e23-106">Na **stranici Dobro** došli kliknite **Konfiguriraj**.</span><span class="sxs-lookup"><span data-stu-id="06e23-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="06e23-107">Na **stranici Dodatni zadaci** odaberite **Prilagodba mogućnosti sinkronizacije**, a zatim **kliknite Dalje**.</span><span class="sxs-lookup"><span data-stu-id="06e23-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="06e23-108">Na **stranici Povezivanje sa servisom Azure AD** unesite vjerodajnicu globalnog administratora za klijent azure, a zatim kliknite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="06e23-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="06e23-109">Na stranicama **Za povezivanje direktorija** **i Filtriranje domene/OU** kliknite **Dalje.**</span><span class="sxs-lookup"><span data-stu-id="06e23-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="06e23-110">Na **stranici Neobavezne** značajke odaberite okvir pokraj mogućnosti **Vraćanje pisanja lozinkom pa** kliknite **Dalje**.</span><span class="sxs-lookup"><span data-stu-id="06e23-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="06e23-111">Na **stranici Spremno za** konfiguriranje kliknite **Konfiguriraj** i pričekajte da postupak završi.</span><span class="sxs-lookup"><span data-stu-id="06e23-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="06e23-112">Kada vidite završetak konfiguracije, kliknite **Izlaz**.</span><span class="sxs-lookup"><span data-stu-id="06e23-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="06e23-113">Kada je omogućeno vraćanje pisanja lozinkom na servisu Azure AD Connect, konfigurirajte Azure AD SSPR za povrat pisanja.</span><span class="sxs-lookup"><span data-stu-id="06e23-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="06e23-114">Da biste omogućili vraćanje pisanja lozinke u SSPR-u, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="06e23-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="06e23-115">Prijavite se na portal Azure pomoću globalnog administratorskog računa.</span><span class="sxs-lookup"><span data-stu-id="06e23-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="06e23-116">Potražite i odaberite **Azure Active Directory**, kliknite Ponovno postavljanje **lozinke**, a zatim **lokalnu integraciju**.</span><span class="sxs-lookup"><span data-stu-id="06e23-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="06e23-117">Postavite mogućnost za pisanje lozinki u **lokalni direktorij? na** **Da**.</span><span class="sxs-lookup"><span data-stu-id="06e23-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="06e23-118">Postavite mogućnost Dopusti **korisnicima otključavanje računa bez ponovnog postavljanja lozinke?** na **Da**.</span><span class="sxs-lookup"><span data-stu-id="06e23-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="06e23-119">Kada budete spremni, kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="06e23-119">When ready, click **Save**.</span></span>

<span data-ttu-id="06e23-120">Dodatne informacije potražite u članku [Omogućivanje samoposlužnog](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)vraćanja izvorne lozinke servisa Azure Active Directory u lokalno okruženje .</span><span class="sxs-lookup"><span data-stu-id="06e23-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="06e23-121">Kada administrator ponovno postavi korisničku lozinku na portalu Azure, ako je taj korisnik združen ili se sinkronizira s lozinkama, lozinka se ponovno zapisi na lokalno.</span><span class="sxs-lookup"><span data-stu-id="06e23-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="06e23-122">Za tu je funkciju potrebna licenca za Azure Premium (P1 ili P2) i trenutno nije podržana na portalu za administratore sustava Office.</span><span class="sxs-lookup"><span data-stu-id="06e23-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
