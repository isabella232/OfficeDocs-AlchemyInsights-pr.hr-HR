---
title: Napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398546"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="330e5-102">Napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="330e5-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="330e5-103">Slijede napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="330e5-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="330e5-104">**Proaktivna provjera autentičnosti**</span><span class="sxs-lookup"><span data-stu-id="330e5-104">**Proactive Authentication**</span></span>

<span data-ttu-id="330e5-105">Kada omogućite [pravilnik ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge će pokušati proaktivno provjeriti autentičnost prijavljenih korisnika putem Microsoftovih servisa.</span><span class="sxs-lookup"><span data-stu-id="330e5-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="330e5-106">U pravilnim vremenskim razmacima koristit će internetski servis za provjeru ažuriranog manifesta koji sadrži konfiguraciju koja uređuje proaktivnu provjeru autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="330e5-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="330e5-107">Prednosti: proaktivna provjera autentičnosti omogućuje provjeru autentičnosti ključnim servisima, kao što je stranica nove kartice sustava Office.</span><span class="sxs-lookup"><span data-stu-id="330e5-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="330e5-108">Osim toga, ako se Bing koristi kao tražilica, proaktivna provjera autentičnosti poboljšava performanse adresne trake i pridonosi generiranju rezultata pretraživanja personaliziranih potrebama vaše tvrtke.</span><span class="sxs-lookup"><span data-stu-id="330e5-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="330e5-109">**Windows Hello CredUI za provjeru autentičnosti NTLM-om**</span><span class="sxs-lookup"><span data-stu-id="330e5-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="330e5-110">Ako jedinstvena prijava (SSO) nije dostupna kada se web-mjesto pokuša prijaviti na korisnika putem mehanizma NTLM ili Negotiate, ta će značajka korisniku omogućiti zajedničko korištenje vjerodajnica operacijskog sustava s web-mjestom i zadovoljavanje izazova provjere autentičnosti pomoću korisničkog sučelja za Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="330e5-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="330e5-111">Taj će se tijek prijave prikazivati samo u sustavu Windows 10 i samo za korisnike koji ne primaju SSO tijekom NTLM-a ili izazova za pregovore.</span><span class="sxs-lookup"><span data-stu-id="330e5-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="330e5-112">**Automatska prijava pomoću spremljenih lozinki**</span><span class="sxs-lookup"><span data-stu-id="330e5-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="330e5-113">Korisnici koji spremaju lozinke u pregledniku Microsoft Edge mogu omogućiti automatsku prijavu na web-mjesta na kojima su spremili vjerodajnice.</span><span class="sxs-lookup"><span data-stu-id="330e5-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="330e5-114">Korisnici tu značajku mogu uključiti ili isključiti u edge://settings/passwords, a možete je konfigurirati u pravilima [upravitelja lozinkom.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="330e5-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
