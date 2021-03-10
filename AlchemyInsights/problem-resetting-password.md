---
title: Problem s ponovnim postavljanjem lozinke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692888"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="be2c2-102">Problemi s ponovnim postavljanjem lozinke</span><span class="sxs-lookup"><span data-stu-id="be2c2-102">Problems resetting password</span></span>

<span data-ttu-id="be2c2-103">Slijede neki od problema s kojima se možete suočiti prilikom ponovnog postavljanja lozinke i mogućih rješenja:</span><span class="sxs-lookup"><span data-stu-id="be2c2-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="be2c2-104">**Imam problem s resetiranju lozinki koje nisu obuhvaćene drugim kategorijama**</span><span class="sxs-lookup"><span data-stu-id="be2c2-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="be2c2-105">Provjerite jeste li ovlašteni za ponovno postavljanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="be2c2-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="be2c2-106">Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.</span><span class="sxs-lookup"><span data-stu-id="be2c2-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="be2c2-107">Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.</span><span class="sxs-lookup"><span data-stu-id="be2c2-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="be2c2-108">Provjerite razumijete li licencne preduvjete:</span><span class="sxs-lookup"><span data-stu-id="be2c2-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="be2c2-109">U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna licenca</span><span class="sxs-lookup"><span data-stu-id="be2c2-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="be2c2-110">Samo oblak korisnici-bilo koji Office 365 (O365) Paid SKU ili Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="be2c2-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="be2c2-111">Cloud i/ili lokalni korisnici-Azure AD Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="be2c2-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="be2c2-112">Dodatne informacije o zahtjevima za licenciranje potražite u članku [Licencne preduvjete za ponovno postavljanje lozinke za Azure ad samoposlužno](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="be2c2-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="be2c2-113">**Imam problema s testiranjem pravilnika za ponovno postavljanje lozinki koje sam postavio**</span><span class="sxs-lookup"><span data-stu-id="be2c2-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="be2c2-114">Nedavno primijenjena pravila mogu potrajati nekoliko minuta da biste replicirali sve podatkovne centre i krajnje toиke.</span><span class="sxs-lookup"><span data-stu-id="be2c2-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="be2c2-115">Fizička Udaljenost iz podatkovnog centra također će utjecati na brzinu primjene promjena.</span><span class="sxs-lookup"><span data-stu-id="be2c2-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="be2c2-116">Testirajte s krajnjim korisnikom, a ne administratorom i pilotom s malim skupom korisnika.</span><span class="sxs-lookup"><span data-stu-id="be2c2-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="be2c2-117">Pravila konfigurirana na portalu Azure primjenjuju se samo na krajnje korisnike, a ne za administratore.</span><span class="sxs-lookup"><span data-stu-id="be2c2-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="be2c2-118">Microsoft nameće snažan zadani pravilnik o ponovnom postavljanju lozinki za bilo koju ulogu Azure administratora (primjerice: globalni administrator, administrator servisa Helpdesk, administrator lozinke itd.)</span><span class="sxs-lookup"><span data-stu-id="be2c2-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="be2c2-119">Saznajte više o [pravilima za administratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="be2c2-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="be2c2-120">**Želim implementirati izvornu lozinku, ali ne želim da moji korisnici registriraju dodatne sigurnosne informacije**</span><span class="sxs-lookup"><span data-stu-id="be2c2-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="be2c2-121">Unaprijed ispunite podatke za korisnike da ne bi morali!</span><span class="sxs-lookup"><span data-stu-id="be2c2-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="be2c2-122">-Kao administrator možete postaviti svojstva telefona i e-pošte za svoje korisnike prije ponovnog postavljanja lozinke u svoju tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="be2c2-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="be2c2-123">To možete učiniti pomoću API-ja, PowerShell ili Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="be2c2-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="be2c2-124">Dodatne informacije:</span><span class="sxs-lookup"><span data-stu-id="be2c2-124">More information here:</span></span>
- [<span data-ttu-id="be2c2-125">Implementacija ponovnog postavljanja lozinke bez zahtjeva korisnika za registraciju</span><span class="sxs-lookup"><span data-stu-id="be2c2-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="be2c2-126">Koje podatke koristi ponovno postavljanje lozinke</span><span class="sxs-lookup"><span data-stu-id="be2c2-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="be2c2-127">**Gumb za ponovno postavljanje lozinke je zasivljen**</span><span class="sxs-lookup"><span data-stu-id="be2c2-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="be2c2-128">Niste ovlašteni za ponovno postavljanje lozinki ovog korisnika.</span><span class="sxs-lookup"><span data-stu-id="be2c2-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="be2c2-129">Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.</span><span class="sxs-lookup"><span data-stu-id="be2c2-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="be2c2-130">Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.</span><span class="sxs-lookup"><span data-stu-id="be2c2-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="be2c2-131">**Ne vidim oštricu za vraćanje izvorne lozinke**</span><span class="sxs-lookup"><span data-stu-id="be2c2-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="be2c2-132">Niste ovlašteni za ponovno postavljanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="be2c2-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="be2c2-133">Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.</span><span class="sxs-lookup"><span data-stu-id="be2c2-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="be2c2-134">Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.</span><span class="sxs-lookup"><span data-stu-id="be2c2-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="be2c2-135">**U odjeljku reset lozinke ne vidim članak o lokalnoj integraciji**</span><span class="sxs-lookup"><span data-stu-id="be2c2-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="be2c2-136">Naziv lokalne integracije prikazuje se samo u hibridnim okruženjima, što znači da koristite lozinku nepotvrđenim da biste manipulirali lokalnim korisničkim lozinkama.</span><span class="sxs-lookup"><span data-stu-id="be2c2-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="be2c2-137">Ovu oštricu ne vidite ako:</span><span class="sxs-lookup"><span data-stu-id="be2c2-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="be2c2-138">Ne koristite lozinku nepotvrđenim</span><span class="sxs-lookup"><span data-stu-id="be2c2-138">You are not using password writeback</span></span>
    - <span data-ttu-id="be2c2-139">Došlo je do problema s vašom instalacijom/povezivanjem lozinke za nepotvrđenim</span><span class="sxs-lookup"><span data-stu-id="be2c2-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="be2c2-140">Došlo je do problema s instalacijom/povezivanjem servisa Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="be2c2-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="be2c2-141">Dodatne upute za otklanjanje poteškoća s lozinkama za lozinke potražite u odjeljku [Otklanjanje poteškoća s lozinkom nepotvrđenim](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="be2c2-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="be2c2-142">**Ne znam kako ponovno postaviti korisnikovu lozinku**</span><span class="sxs-lookup"><span data-stu-id="be2c2-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="be2c2-143">Prijavite se na portal Azure kao odgovarajući administrator.</span><span class="sxs-lookup"><span data-stu-id="be2c2-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="be2c2-144">Idite na sječivo korisnika i grupe, odaberite **Svi korisnici**.</span><span class="sxs-lookup"><span data-stu-id="be2c2-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="be2c2-145">Na popisu odaberite korisnika.</span><span class="sxs-lookup"><span data-stu-id="be2c2-145">Select a user from the list.</span></span>
1. <span data-ttu-id="be2c2-146">Za odabranog korisnika odaberite **Pregled**, a zatim na traci naredbi kliknite **ponovno Postavi lozinku**.</span><span class="sxs-lookup"><span data-stu-id="be2c2-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="be2c2-147">Slijedite upute na zaslonu.</span><span class="sxs-lookup"><span data-stu-id="be2c2-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="be2c2-148">U servisu Azure portal podržava se samo ponovno setovi za lozinku.</span><span class="sxs-lookup"><span data-stu-id="be2c2-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="be2c2-149">**Resetirao sam lozinku lokalnog korisnika na portalu za administratore sustava Office 365 ili mobilne aplikacije sustava Office 365, no korisnik se i dalje ne može prijaviti**</span><span class="sxs-lookup"><span data-stu-id="be2c2-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="be2c2-150">Na ovom portalu nije podržana lozinka writeback.</span><span class="sxs-lookup"><span data-stu-id="be2c2-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="be2c2-151">Ponovno postavljanje korisničke lozinke na portalu Azure-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="be2c2-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

