---
title: Problemi s vjerodajnicama
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063599"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="4560b-102">Problemi s vjerodajnicama</span><span class="sxs-lookup"><span data-stu-id="4560b-102">Issues with credentials</span></span>

<span data-ttu-id="4560b-103">[Microsoftova platforma za identitete i tijek vjerodajnica oauth 2,0 klijent](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje kako se program izravno protivi protoku dodjele klijentske vjerodajnice oauth 2,0.</span><span class="sxs-lookup"><span data-stu-id="4560b-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="4560b-104">**Kako upravljati lozinkom ili vjerodajnicama za certifikat?**</span><span class="sxs-lookup"><span data-stu-id="4560b-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="4560b-105">U servisu Azure CLI možete koristiti [credencijalnu aplikaciju AZ ad](https://docs.microsoft.com/cli/azure/ad/app/credential) za brisanje, popis ili vraćanje izvornih vjerodajnica aplikacija ili certifikata.</span><span class="sxs-lookup"><span data-stu-id="4560b-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="4560b-106">**Kako korisnici mogu ponovno postaviti lozinke?**</span><span class="sxs-lookup"><span data-stu-id="4560b-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="4560b-107">Korisnici se moraju [registrirati za samoposlužnu izvornu lozinku](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) da bi mogli ponovno postaviti lozinke.</span><span class="sxs-lookup"><span data-stu-id="4560b-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="4560b-108">Kada se korisnik registrira, možete pratiti upute u ovom članku da biste ponovno postavili lozinku: [ponovno postavite lozinku za rad ili školu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="4560b-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="4560b-109">**Kako korisnici mogu promijeniti svoje lozinke?**</span><span class="sxs-lookup"><span data-stu-id="4560b-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="4560b-110">Korisnici mogu pratiti korake u ovom članku da bi promijenili svoje lozinke: [kako promijeniti lozinku](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="4560b-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="4560b-111">Mogu upravljati i [lozinkama za aplikacije za provjeru u dva koraka](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="4560b-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="4560b-112">**Prilikom promjene ili ponovnog postavljanja lozinke moj korisnik dobiva pogrešku**</span><span class="sxs-lookup"><span data-stu-id="4560b-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="4560b-113">Ta će vam veza pružiti informacije o uobičajenim problemima koji se mogu pojaviti kada korisnik pokuša ponovno postaviti lozinku: [Česti problemi i njihova rješenja](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="4560b-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="4560b-114">**Problem s ponovnim postavljanjem lozinke korisnika**</span><span class="sxs-lookup"><span data-stu-id="4560b-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="4560b-115">Provjerite jeste li ovlašteni za ponovno postavljanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="4560b-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="4560b-116">*Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.*</span><span class="sxs-lookup"><span data-stu-id="4560b-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="4560b-117">Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.</span><span class="sxs-lookup"><span data-stu-id="4560b-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="4560b-118">Provjerite razumijete li licencne preduvjete:</span><span class="sxs-lookup"><span data-stu-id="4560b-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="4560b-119">U vašoj tvrtki ili ustanovi mora biti dodijeljena najmanje jedna Licenca:</span><span class="sxs-lookup"><span data-stu-id="4560b-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="4560b-120">**Samo oblak korisnici** -bilo koji Office 365 (O365) Paid SKU ili Azure ad Basic</span><span class="sxs-lookup"><span data-stu-id="4560b-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="4560b-121">**Cloud i/ili lokalni korisnici** -Azure ad Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure produktivnost Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="4560b-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="4560b-122">Dodatne informacije o preduvjetima za licenciranje potražite u članku [Licencne preduvjete za ponovno postavljanje lozinke za Azure ad samoposlužno](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="4560b-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="4560b-123">Da biste ponovno postavili korisnikovu lozinku, pronađite korisnika u servisu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4560b-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="4560b-124">Zatim na kartici Pregled za tog korisnika kliknite gumb "Vrati izvornu lozinku".</span><span class="sxs-lookup"><span data-stu-id="4560b-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="4560b-125">**Gumb za ponovno postavljanje lozinke je zasivljen**</span><span class="sxs-lookup"><span data-stu-id="4560b-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="4560b-126">Niste ovlašteni za ponovno postavljanje lozinki **ovog** korisnika.</span><span class="sxs-lookup"><span data-stu-id="4560b-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="4560b-127">*Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.*</span><span class="sxs-lookup"><span data-stu-id="4560b-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="4560b-128">Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.</span><span class="sxs-lookup"><span data-stu-id="4560b-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="4560b-129">**Ne vidim oštricu za vraćanje izvorne lozinke**</span><span class="sxs-lookup"><span data-stu-id="4560b-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="4560b-130">Niste ovlašteni za ponovno postavljanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="4560b-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="4560b-131">*Samo globalna, lozinka i korisnički administratori mogu ponovno postaviti korisničke lozinke.*</span><span class="sxs-lookup"><span data-stu-id="4560b-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="4560b-132">Globalni administratori mogu i ponovno postaviti lozinke za druge privilegirane administratore.</span><span class="sxs-lookup"><span data-stu-id="4560b-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="4560b-133">**U odjeljku reset lozinke ne vidim članak o lokalnoj integraciji**</span><span class="sxs-lookup"><span data-stu-id="4560b-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="4560b-134">Naziv lokalne integracije prikazuje se samo u hibridnim okruženjima, što znači da koristite lozinku nepotvrđenim da biste manipulirali lokalnim korisničkim lozinkama.</span><span class="sxs-lookup"><span data-stu-id="4560b-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="4560b-135">Ovu oštricu ne vidite ako:</span><span class="sxs-lookup"><span data-stu-id="4560b-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="4560b-136">Ne koristite lozinku nepotvrđenim</span><span class="sxs-lookup"><span data-stu-id="4560b-136">You are not using password writeback</span></span>
  - <span data-ttu-id="4560b-137">Došlo je do problema s vašom instalacijom/povezivanjem lozinke za nepotvrđenim</span><span class="sxs-lookup"><span data-stu-id="4560b-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="4560b-138">Došlo je do problema s instalacijom/povezivanjem servisa Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="4560b-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="4560b-139">Dodatne upute za otklanjanje poteškoća s lozinkama za lozinke potražite u članku [Otklanjanje poteškoća s lozinkom nepotvrđenim](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="4560b-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="4560b-140">**Ne znam kako ponovno postaviti korisnikovu lozinku**</span><span class="sxs-lookup"><span data-stu-id="4560b-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="4560b-141">Prijavite se na portal Azure kao odgovarajući administrator.</span><span class="sxs-lookup"><span data-stu-id="4560b-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="4560b-142">Idite na sječivo **korisnika i grupe** , odaberite **Svi korisnici**.</span><span class="sxs-lookup"><span data-stu-id="4560b-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="4560b-143">Na popisu odaberite korisnika.</span><span class="sxs-lookup"><span data-stu-id="4560b-143">Select a user from the list.</span></span>
4. <span data-ttu-id="4560b-144">Za odabranog korisnika odaberite **Pregled**, a zatim na naredbenoj trakasti odaberite **ponovno Postavi lozinku**.</span><span class="sxs-lookup"><span data-stu-id="4560b-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="4560b-145">Odaberite gumb **Vrati izvornu lozinku** i slijedite upute na zaslonu.</span><span class="sxs-lookup"><span data-stu-id="4560b-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="4560b-146">U servisu **Azure portal** podržava se samo ponovno setovi za lozinku.</span><span class="sxs-lookup"><span data-stu-id="4560b-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="4560b-147">**Resetirao sam lozinku lokalnog korisnika na portalu za administratore sustava Office 365 ili mobilne aplikacije sustava Office 365, no korisnik se i dalje ne može prijaviti**</span><span class="sxs-lookup"><span data-stu-id="4560b-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="4560b-148">Na ovom portalu nije podržana lozinka writeback.</span><span class="sxs-lookup"><span data-stu-id="4560b-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="4560b-149">Ponovno postavite korisnikovu lozinku na portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="4560b-149">Reset the user's password again in the Azure portal.</span></span>
