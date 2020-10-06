---
title: Praćenje uvjetnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366420"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="d7e6c-102">Praćenje uvjetnog pristupa za Exchange</span><span class="sxs-lookup"><span data-stu-id="d7e6c-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="d7e6c-103">Korisnici usmjereni na uvjetni pristup primit će obavijest e-poštom ako ne zadovoljavaju preduvjete za pristup vaše tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="d7e6c-104">Da biste riješili, preporučujemo vam jedno ili više sljedećih rješenja:</span><span class="sxs-lookup"><span data-stu-id="d7e6c-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="d7e6c-105">Ako se pretpostavlja da je uređaj upisan, savjetujte korisniku da otvori aplikaciju Portal tvrtke i provjerite prikazuje li se na portalu tvrtke.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="d7e6c-106">Ako se to ne dogodi, korisnik bi trebao upisati uređaj.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="d7e6c-107">Na portalu Azure idite na Intune > usklađenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="d7e6c-108">U odjeljku monitor kliknite usklađenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="d7e6c-109">Prikažite izvješće o usklađenosti uređaja da biste provjerili je li korisnikov uređaj označenog kao usklađen.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="d7e6c-110">Na portalu Azure idite na Intune > usklađenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="d7e6c-111">U odjeljku Upravljanje kliknite pravila.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-111">Under Manage, click Policies.</span></span> <span data-ttu-id="d7e6c-112">Na popisu pravilnika o usklađenosti provjerite je li profil dodijeljen vašem korisničkom uređaju.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="d7e6c-113">Ako nijedan profil nije dodijeljen, zatim Intune neće moći potvrditi status usklađenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="d7e6c-114">Uredite korisnički zadatak uvjetnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="d7e6c-115">Na portalu Azure idite na umetanje **Intune**  >  pravilnika o**uvjetnom pristupu**  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="d7e6c-116">Na popisu odaberite pravilo.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="d7e6c-117">Kliknite Korisnici i grupe.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-117">Click Users and groups.</span></span>
4. <span data-ttu-id="d7e6c-118">Da biste neku određenu politiku usmjerili na nekoga, dodajte ih na popis uvrštavanje.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="d7e6c-119">Da biste bili sigurni da je osoba izostavljena iz pravilnika, dodajte ih na popis za izuzimanje.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="d7e6c-120">Korisne veze:</span><span class="sxs-lookup"><span data-stu-id="d7e6c-120">Helpful links:</span></span>

[<span data-ttu-id="d7e6c-121">Pregled usklađenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="d7e6c-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="d7e6c-122">Otklanjanje poteškoća sa com</span><span class="sxs-lookup"><span data-stu-id="d7e6c-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d7e6c-123">Pravilnik o otklanjanju poteškoća</span><span class="sxs-lookup"><span data-stu-id="d7e6c-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="d7e6c-124">Praćenje usklađivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="d7e6c-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="d7e6c-125">Pažnja: ovi su koraci korisni samo u otklanjanju poteškoća s uvjetnim pristupom značajke Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="d7e6c-126">Moguće je i karantensku napravu koja blokira pristup e-pošti putem pravilnika sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7e6c-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="d7e6c-127">Dodatne informacije o upravljanju uređajima sustava Exchange možete pronaći [ovdje](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="d7e6c-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
