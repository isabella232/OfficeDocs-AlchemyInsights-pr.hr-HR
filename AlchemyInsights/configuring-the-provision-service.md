---
title: Konfiguriranje servisa za pružanje resursa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481344"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="b08ac-102">Konfiguriranje servisa za pružanje resursa</span><span class="sxs-lookup"><span data-stu-id="b08ac-102">Configuring the Provision service</span></span>

<span data-ttu-id="b08ac-103">Da bi automatizirani korisnici mogli funkcionirati, za Azure AD potrebna su valjana vjerodajnica koja omogućuje povezivanje s API-jem WORKDAY tkanje Services.</span><span class="sxs-lookup"><span data-stu-id="b08ac-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="b08ac-104">Nadalje, gumb Testiraj vezu na radni dan u aplikaciji za dodjelu korisničkih resursa oglašava se i potvrđuje ako se može povezati s agentom za dodjelu resursa za Azure AD Connect u domenu oglasa.</span><span class="sxs-lookup"><span data-stu-id="b08ac-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="b08ac-105">Ako se na portalu Azure vraća pogreška prilikom spremanja vjerodajnica, slijedite preporučene upute u nastavku:</span><span class="sxs-lookup"><span data-stu-id="b08ac-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="b08ac-106">Potvrdite da ste konfigurirali korisnički račun za sustav integracije WORKDAY kao što je navedeno u odjeljku udžbenik [konfigurirajte korisnika sustava integracija u radnom danu](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="b08ac-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="b08ac-107">Potvrdite da je servis Azure AD Connect agent za dodjelu resursa instaliran i pokrenut na lokalnom sustavu Windows Server pomoću konzole za upravljanje servisima.</span><span class="sxs-lookup"><span data-stu-id="b08ac-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="b08ac-108">Možete i provjeriti status agenta na portalu Azure tako da kliknete gumb Prikaz lokalnih agenata.</span><span class="sxs-lookup"><span data-stu-id="b08ac-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="b08ac-109">Uvjerite se da unosite vrijednost u polje "WORKDAY username" pomoću oblika username@workday-naziv korisnika.</span><span class="sxs-lookup"><span data-stu-id="b08ac-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="b08ac-110">Ako nedostaje radni dan-naziv korisnika, provjera autentičnosti radnog dana neće uspjeti.</span><span class="sxs-lookup"><span data-stu-id="b08ac-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="b08ac-111">Ako konfigurirate integraciju s klijentom za provedbu radnog dana, primjetite zakazane sate zastoja u svom radnom danu.</span><span class="sxs-lookup"><span data-stu-id="b08ac-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="b08ac-112">WORKDAY je zakazano vrijeme za provedbu stanara tijekom vikenda (obično od petka navečer do subote ujutro) i pogreške pri povezivosti tijekom ove pauze prozor je poznat problem koji automatski rješava čim se ponovno implementiraju stanari u mreži.</span><span class="sxs-lookup"><span data-stu-id="b08ac-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="b08ac-113">U rijetkim slučajevima možete vidjeti i ovu pogrešku ako je lozinka korisnika sustava integracije promijenjen zbog osvježavanja gosta ili ako je račun zaključan ili isteklog stanja.</span><span class="sxs-lookup"><span data-stu-id="b08ac-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="b08ac-114">Provjerite status korisnika sustava integracija sa svojim administratorom radne dane.</span><span class="sxs-lookup"><span data-stu-id="b08ac-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="b08ac-115">Dodatne informacije o konfiguriranju radnog dana za automatiziranu dodjelu resursa potražite u članku [Udžbenik: Konfiguriranje radnog dana za automatsku dodjelu korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="b08ac-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
