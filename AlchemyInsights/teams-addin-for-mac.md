---
title: Teams dodatak za Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582062"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="d8e91-102">Teams dodatak za Mac</span><span class="sxs-lookup"><span data-stu-id="d8e91-102">Teams add-in for Mac</span></span>

<span data-ttu-id="d8e91-103">Da biste otklonili poteškoće s Teams dodatka za korisnike operacijskog sustava Mac, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="d8e91-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="d8e91-104">**Prvi korak:** Ako imate hibridnu Exchange (2016 CU3 ili noviju) koristite alat za Test-HMA.ps1 da biste potvrdili da je hibridna moderna provjera autentičnosti pravilno konfigurirana.</span><span class="sxs-lookup"><span data-stu-id="d8e91-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="d8e91-105">Dodatne informacije potražite u članku Provjera [valjanosti hibridnog modernog postavljanja provjere autentičnosti za Outlook za iOS i Android](https://aka.ms/TestHMAEAS).</span><span class="sxs-lookup"><span data-stu-id="d8e91-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="d8e91-106">**Napomena** Koristite oblik UPN adrese (npr. [username@contoso.com](mailto:username@contoso.com)), a ne domena\korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="d8e91-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="d8e91-107">Učinite to čak i za korisnike s Exchange Online poštanskim sandučićima.</span><span class="sxs-lookup"><span data-stu-id="d8e91-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="d8e91-108">**Drugi korak:** Neka korisnik ode na **Alati**  >  **računi**... u Outlook za Mac pa pronađite i odaberite račun.</span><span class="sxs-lookup"><span data-stu-id="d8e91-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="d8e91-109">Potvrdite da je korisničko ime navedeno u upn obliku (npr. [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="d8e91-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="d8e91-110">**Treći korak:** Potvrdite da je korisnik licencirani Microsoft Teams korisnik.</span><span class="sxs-lookup"><span data-stu-id="d8e91-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="d8e91-111">Korisnik mora koristiti pretplatu na Office 365 Mac, verziju proizvoda 16.24 ili noviju.</span><span class="sxs-lookup"><span data-stu-id="d8e91-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>