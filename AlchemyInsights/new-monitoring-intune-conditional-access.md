---
title: Praćenje neusklađeni uvjetni pristup
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427181"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="e0b6b-102">Praćenje neusklađeni uvjetni pristup</span><span class="sxs-lookup"><span data-stu-id="e0b6b-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="e0b6b-103">Korisnici usmjereni na uvjetni pristup primit će obavijest e-poštom ako ne zadovoljavaju preduvjete za pristup vaše tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e0b6b-104">Da biste riješili, preporučujemo vam jedno ili više sljedećih rješenja:</span><span class="sxs-lookup"><span data-stu-id="e0b6b-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="e0b6b-105">Ako se pretpostavlja da je uređaj upisan, savjetujte korisniku da otvori aplikaciju Portal tvrtke i provjerite prikazuje li se na portalu tvrtke.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e0b6b-106">Ako to ne učinite, korisnik mora upisati uređaj.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="e0b6b-107">**Na portalu** Azure potražite  >  **usklađenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="e0b6b-108">Da biste pregledali izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označenog kao kompatibilan, u odjeljku **Monitor** kliknite **usklađenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="e0b6b-109">**Na portalu** Azure potražite  >  **usklađenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="e0b6b-110">U odjeljku **Upravljanje** kliknite **pravila**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="e0b6b-111">Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e0b6b-112">Ako nijedan profil nije dodijeljen, zatim Intune neće moći potvrditi status usklađenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="e0b6b-113">Uredite korisnički zadatak uvjetnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="e0b6b-114">Na portalu Azure prijeđite na **unos** pravilnika o  >  **uvjetnom pristupu**  >  , odaberite pravilo na popisu, a zatim kliknite **Korisnici i grupe**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="e0b6b-115">Da biste neku određenu politiku usmjerili na nekoga, dodajte ih na **popis uvrštavanje**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="e0b6b-116">Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte ih na **popis za izuzimanje**.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="e0b6b-117">**Korisne veze:**</span><span class="sxs-lookup"><span data-stu-id="e0b6b-117">**Helpful links:**</span></span>

- [<span data-ttu-id="e0b6b-118">Pregled usklađenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="e0b6b-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="e0b6b-119">Otklanjanje poteškoća sa com</span><span class="sxs-lookup"><span data-stu-id="e0b6b-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="e0b6b-120">Pravilnik o otklanjanju poteškoća</span><span class="sxs-lookup"><span data-stu-id="e0b6b-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="e0b6b-121">Praćenje usklađivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="e0b6b-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="e0b6b-122">Ovi su koraci korisni samo u otklanjanju poteškoća s uvjetnim pristupom značajke Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e0b6b-123">Moguće je i karantensku napravu koja blokira pristup e-pošti putem pravilnika sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0b6b-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e0b6b-124">Dodatne informacije o upravljanju uređajima sustava Exchange možete pronaći [**ovdje**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="e0b6b-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
